# 通过直接编辑 XML 在 Eagle CAD 中重命名零件

> 原文：<https://hackaday.com/2013/01/18/renaming-parts-in-eagle-cad-by-editing-the-xml-directly/>

![eagle-xml-find-and-replace-script](img/baeb9d37ab728dfed7d3b23ca0163e89.png)

在设计 PCB 时，有很多方法可以消耗你的时间，但重命名元件可能是最令人沮丧的方法之一。[Joe Pinzone]写了他对这个问题的解决方案。他不是一次一个地寻找原理图上的每一个部分来改变它们，而是制作一个替换列表，然后使用一个脚本在 XML 文件中进行所有的改变。他没有发表关于他的工作的帖子，但你会在休息后找到他写的源代码。

压垮骆驼的最后一根稻草是一个包括大约 200 个组件的项目，这些组件似乎没有一个命名顺序，与组件的实际值没有任何关系。该脚本是用 C++编写的(适用于 Windows，但[Joe]说这也应该很容易移植到其他系统)。为了使用它，他创建了一个 CSV 文件，在第一列中包含当前组件的名称。然后他在第二列输入他想要的新名字。然后，这个 CSV 文件以及 BRD 和 SCH 文件作为脚本的输入(通过选择所有文件并拖动到脚本或作为 CLI 参数)，它会自动进行更改。

当然，这只是可能的，因为 Cadsoft 在 Eagle 6 中过渡到使用 XML 文件。

```
/*
  Title: EagleCAD XML Batch Component Renamer
  Author: Joe Pinzone, Newbury Ohio
  License: Free (&quot;beer&quot;), with acknowledgement of original author
  Date: January, 2013

  Description:
    * Designed to use a CSV to perform batch renaming of EagleCAD schematic/board components
    * Works only on new Eagle XML format schematic and board files

  To generate CSV file with original component name list:
    * Simply drag ONLY your SCH file or BRD onto the EXE. partsList.csv is automatically generated from that file.

  To perform batch renaming:
    * Generate a CSV with original part names in first column, and replacement names in the second
    * Click and drag your SCH, BRD, and CSV file onto the EXE (use multi-select)
    * ^Alternatively, enter in the file paths as arguments from the command prompt

  Notes:
     * If the entry in the second column of the CSV row (replacement name) is blank, that entry will be skipped,
         and the component will retain it's original name
     * To prevent accidental replacement of identical character strings within the XML file, the program
          looks for the specific XML tags that correspond to component names. Edit the list in the
          &quot;Handy things you can modify&quot; section if Eagle changes things, or if you want to play around.
     * You can only load ONE schematic and ONE board file at a time.
     * You can only have 1000 entries in the CSV file. All others are ignored.
        However, you can increase this by setting the value of #define MAX_CSV_ROWS in the source file.
        I didn't want to take up too much memory unnecessarily, and 1000 is plenty for most people.
     * Live long and prosper
*/

#include &lt;cstring&gt;
#include &lt;string&gt;
#include &lt;iostream&gt;
#include &lt;fstream&gt;

using namespace std;

// Handy things you can modify -----------------------------------------------------------------------------------

   /*
       Path and file name to use when generating a name list
   */
   #define MAX_CSV_ROWS 1000 // change this to allow more entries in the CSV find/replace file if necessary.
                             // The program fails nicely, though - it just ignores entries after row 1000.

   char* partsListGenFile = &quot;./partsList.csv&quot;;       // the directory and name of the generated parts list CSV file (if no find/replace CSV file is specified)

   /*
     This is the list of XML entries/tags that contain component names after them (from both SCH and BRD Eagle XML files)
     This list is used to make sure that ONLY component names are modified, and coincidental string matches
        elsewhere in the XML aren't accidentally changed. It happened once to me. It wasn't fun. True story.

     Add/remove tags to this list if Eagle changes their standard, or you decide to adapt this for some other purpose.

     The value of 'numTags' should match the number of elements in the 'xmlTags' array below - make sure they match if you change something!
   */
   int numTags = 5;
   string xmlTags[] = { &quot;part name&quot;, \
                        &quot;instance part&quot;, \
                        &quot;pinref part&quot;, \
                        &quot;element name&quot;, \
                        &quot;contactref element&quot; \
                      };

   /*
      When generating the CSV list, we only want one copy of each component name.
      The &lt;part name&gt; XML entries in the schematic files, or the &lt;element name&gt; XML entries in the board files
         only contain one entry per part, so we use those as the lookup strings when generating the CSV.
   */
   string schemXMLTag_part = &quot;part name&quot;;
   string boardXMLTag_part = &quot;element name&quot;;

// (Global) Variable Declarations  -------------------------------------------------------------------------------

	bool schemFound = false;       // used by parseArguments, marks if schematic file was found in the files loaded
	bool boardFound = false;       // used by parseArguments, marks if board file was found in the files loaded
	bool listFound = false;        // used by parseArguments, marks if find/replace csv file was found in the files loaded

	char* path_schem;              // the file path (full or relative) of the schematic file
	char* path_board;              // the file path (full or relative) of the board file
	char* path_list ;              // the file path (full or relative) of the csv find/replace list

	string list[1000][2];          // The storage array for the find/replace list. FIND string is element 0, REPLACE string is element 1
	int listLength = 0;            // number of populated entries in the list array above (set by the loadList function's return value)

// Function Prototypes	-------------------------------------------------------------------------------------------

	int parseArguments(int argc, char* args[]);    // loads the program arguments (file paths of schematic/board/csv files)

	int processFile(char* XMLFilePath);            // assuming that 'list' is populated, goes line-by-line through specified file and replaces component names
	string processLine(string original);           // used by processFile to process an individual line of text
	string processPart(string original);           // used by processLine to change the part name based on the find/replace list

	int loadList(char* listFilePath);              // parses/loads the list file into memory (into the 'list' array)
	void generateList(char* XMLPath, char* outPath, string xmlReferenceTag); // generates a new CSV component name list from the specified SCH or BRD file

// Program --------------------------------------------------------------------------------------------------------

int main(int argc, char* args[]){

    cout &lt;&lt; &quot;EagleCAD XML Batch Component Renamer...\n\n&quot;;
    if(!parseArguments(argc, args)) { system(&quot;pause&quot;); return 0;} // parse program arguments, pause and close on error

    if(listFound == false){ // if no list was specified, assume that we should generate a parts list instead of doing find/replace
         if(schemFound == true){ generateList(path_schem, partsListGenFile, schemXMLTag_part);} // if schematic file is available, generate the list from that
         else if (boardFound == true){ generateList(path_board, partsListGenFile, boardXMLTag_part);} // if schematic file is not available, generate from board file
    }
    else if (listFound == true){ // if the user specified a find/replace list, do the find/replace
         listLength = loadList(path_list);
         if(schemFound == true){ cout &lt;&lt; &quot;Changed &lt;&quot; &lt;&lt; processFile(path_schem) &lt;&lt; &quot;&gt; lines in schematic.\n&quot;; }
         if(boardFound == true){ cout &lt;&lt; &quot;Changed &lt;&quot; &lt;&lt; processFile(path_board) &lt;&lt; &quot;&gt; lines on board.\n&quot;; }
    }
    cout &lt;&lt; endl;
    system(&quot;pause&quot;);
    return 0;
}

int parseArguments(int argc, char* args[]){
    /*
         Load the file paths from the program arguments into memory
    */
    for(int index = 1; index &lt; argc; index++){
            string buffer = args[index];
            if(buffer.find(&quot;.sch&quot;) != -1){
                if(schemFound == false){
                    path_schem = args[index];
                    schemFound = true;
                }
                 else{
                      cout &lt;&lt; &quot;You may only load ONE schematic file.\n\n&quot;;
                      return 0;
                 }
            }

            else if(buffer.find(&quot;.brd&quot;) != -1){
                 if(boardFound == false){
                     path_board = args[index];
                     boardFound = true;
                 }
                 else{
                      cout &lt;&lt; &quot;You may only load ONE board file.\n\n&quot;;
                      return 0;
                 }
            }

            else if(buffer.find(&quot;.csv&quot;) != -1){
                 if(listFound == false){
                     path_list = args[index];
                     listFound = true;
                 }
                 else{
                      cout &lt;&lt; &quot;You may only load ONE CSV file.\n\n&quot;;
                      return 0;
                 }
            }

            else{
                 cout &lt;&lt; &quot;Unknown file: &quot; &lt;&lt;  buffer &lt;&lt; endl &lt;&lt; endl;
                 return 0;
            }
    }
    if(schemFound == false &amp;&amp; boardFound == false){
         cout &lt;&lt; &quot;You must specify a schematic (SCH) or board (BRD) file.\n\n&quot;;
         return 0;
    }

	return 1;
}

int processFile(char* XMLFilePath){

     ifstream source; // pointer to source file
     ofstream dest;   // pointer to destination file
     int modifiedLines = 0;

     string newPath = XMLFilePath;
     newPath += &quot;.new&quot;;

     source.open(XMLFilePath); // i.e. file.sch
     dest.open(newPath.c_str()); // i.e. file.sch.new

     string buffer = &quot;&quot;;

     while(!source.eof()){
          getline(source, buffer);
          string temp = processLine(buffer);
          dest &lt;&lt; temp &lt;&lt; endl;
          if(temp != buffer){ modifiedLines++;}

     }

     source.close();
     dest.close();

     return modifiedLines;
}

string processLine(string original){

    /*
      Things to look for in a schematic file
    */
    string beginning = &quot;&quot;;
    string end = &quot;&quot;;
    string partName = &quot;&quot;;

    for(int tagNum = 0; tagNum &lt; numTags; tagNum++){
        if(original.find(&quot;&lt;&quot;+xmlTags[tagNum]+&quot;=\&quot;&quot;) != -1){     // look for lines that contain the part names
            beginning = &quot;&lt;&quot;+xmlTags[tagNum]+&quot;=\&quot;&quot;;              // this is technically always the same, but I want to be explicit
            break; // shouldn't need this if the line contains only one valid XML tag
        }
    }

    // if there is a name to replace, replace it. Otherwise, return the original string
    if(beginning != &quot;&quot;){ // 'beginning' will still be empty (&quot;&quot;) if there isn't a valid tag to be processed
        end = original.substr(beginning.length(),original.length()); // remove the beginning, whatever it may be
        partName = end.substr(0,end.find(&quot;\&quot;&quot;));                  // clear out the trailing XML, leaving just the name
        end = end.substr(end.find(&quot;\&quot;&quot;),end.length());               // clear the part name from the 'end'
        return beginning + processPart(partName) + end;              // return the new line with replaced part name
    }
    // we only get here if there was nothing to replace in the 'if' block above
    return original;
}

string processPart(string original){
       for(int index = 0; index &lt; listLength; index++){
           if(original == list[index][0] &amp;&amp; list[index][1] != &quot;&quot;){ // don't process lines with no replacement
                return list[index][1];
           }
       }
       return original;
}

int loadList(char* listFilePath){

     ifstream source;
     source.open(listFilePath);
     string buffer = &quot;&quot;;
     int entryCount = 0;

     while(!source.eof() &amp;&amp; entryCount &lt; MAX_CSV_ROWS){
         buffer = &quot;&quot;;
         getline(source, buffer);
         list[entryCount][0] = buffer.substr(0,buffer.find(&quot;,&quot;));
         list[entryCount][1] = buffer.substr(buffer.find(&quot;,&quot;)+1,buffer.length());
         entryCount++;

     }

     source.close();
     return entryCount;
}

void generateList(char* XMLPath, char* outPath, string xmlReferenceTag){
     cout &lt;&lt; &quot;Generating components list from: \n&quot; &lt;&lt; XMLPath &lt;&lt; endl &lt;&lt; endl;
     ifstream source;
     ofstream dest;

     source.open(XMLPath);
     dest.open(outPath);

     string buffer = &quot;&quot;;
     string XMLPretext = &quot;&lt;&quot;+xmlReferenceTag+&quot;=\&quot;&quot;; // gotta add the extra characters to look for an actual tag
     int elementCount = 0;
     int lineCount = 0;
     while(!source.eof()){
          buffer = &quot;&quot;;
          getline(source, buffer);
          lineCount ++;
          if(buffer.find(XMLPretext) != -1){ // look for lines that contain the part names
               buffer = buffer.substr(XMLPretext.length(),buffer.length()); // clear out the leading XML
               buffer = buffer.substr(0,buffer.find(&quot;\&quot;&quot;)); // clear out the trailing XML, leaving just the name
               dest &lt;&lt; buffer &lt;&lt; endl;
               elementCount++;
          }

     }
     source.close();
     dest.close();

     return;
}	// generates CSV parts list from SCH or BRD XML files
```