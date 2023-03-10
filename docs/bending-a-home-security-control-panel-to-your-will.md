# 随心所欲地弯曲家庭安全控制面板

> 原文：<https://hackaday.com/2012/07/27/bending-a-home-security-control-panel-to-your-will/>

你的家有一个安全系统，但你没有订阅监控服务，使其工作？把那个宝贝从墙上扯下来，用它做点什么，或者只是围绕它建立你自己的系统。如果你有一个 DSC PC1500RK 控制面板[caitth2]向我们展示了[控制按钮、led 和蜂鸣器](http://www.youtube.com/watch?v=uVkr_SiPJ_0)是多么容易。如果你有一个不同的模型，这仍然是一个很好的起点，开始你自己的逆向工程。

只需要建立四个连接。[caitth2]正在使用 Arduino 进行演示。他将红线连接到电压，黑线连接到地，黄线(时钟)连接到数字引脚 3，绿线(数据)连接到数字引脚 2。一个通信周期从将数据线设为高电平开始，然后输出 8 位来捕捉按键。然后输入 16 位来设置 led 并驱动蜂鸣器。这显示在休息后的视频中，也记录在[他的样本代码](http://pastebin.com/sN7JnJHM)中。我们在休息后嵌入了草图，以保存它，以防将来 pastebin 代码丢失。

[https://www.youtube.com/embed/uVkr_SiPJ_0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/uVkr_SiPJ_0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

```
/*
	The code is to interface a DSC PC1500RK alarm keypad.
        It has 15 keys, 11 LEDs, and a Beeper that can be controlled.
        This code cycles through all the LEDs in a top-down fashion.
        The beeper is used to acknowledge that a key has been pressed.
        If the key was pressed successfully, its character is output on the serial line, at 115200 bps.

        Wiring is simple.  Red is Vcc, hooked to 5V
        Black is Gnd.
        Yellow is the Clock line. In this configuration, it is on Digital Pin 3.
        Green is Data, and is on Digital Pin 2.
*/

void setup() {
  //Pin 2 is Data, and is bidirectional.
  //Pin 3 is Clock, and is an output.
  pinMode(2, OUTPUT);
  pinMode(3, OUTPUT);
  Serial.begin(115200);
}

int readdata(int control)
{

  int i,j=0,k=control;
  int bitcount=0;

  for(i=0;i&lt;8;i++)
  {
    j&lt;&lt;=1;
    digitalWrite(2,HIGH);
    digitalWrite(3,LOW);
    delay(2);
    if(digitalRead(2)==HIGH)
      j|=1;
    digitalWrite(3,HIGH);
    delay(2);
  }
  for(i=0;i&lt;16;i++)
  {
    if(k&amp;0x8000)
      digitalWrite(2,HIGH);
    else
      digitalWrite(2,LOW);
    digitalWrite(3,LOW);
    delay(2);
    digitalWrite(3,HIGH);
    delay(2);
    k&lt;&lt;=1; } j^=0xFF; switch(j&amp;0x70) { case 0x10: case 0x20: case 0x40: switch(j&amp;0x8F) { case 0x80: case 0x08: case 0x04: case 0x02: case 0x01: return j; default: return 0; } default: return 0; } return 0; } void printchar(char A, char B, char C, int D) { switch(D) { case 1: Serial.println(C); break; case 2: Serial.println(B); break; case 4: Serial.println(A); break; } } void loop() { int i; static unsigned int j=0x80; static int k=0,l; static int m=0; digitalWrite(13, HIGH); // set the LED on i=readdata(j | l); m++; if(m==4) { m=0; j&gt;&gt;=1;
    if(j==4)
      j=0x8000;
    if(j==0x0200)
      j=0x80;
  }

  if(k==0)
  {
    switch(i&amp;0x8F)
    {
      case 0x80:
        printchar('F','E','P',(i&amp;0x70)&gt;&gt;4);
        break;
      case 0x08:
        printchar('*','0','#',(i&amp;0x70)&gt;&gt;4);
        break;
      case 0x04:
        printchar('7','8','9',(i&amp;0x70)&gt;&gt;4);
        break;
      case 0x02:
        printchar('4','5','6',(i&amp;0x70)&gt;&gt;4);
        break;
      case 0x01:
        printchar('1','2','3',(i&amp;0x70)&gt;&gt;4);
        break;

    }
  }
  if((k!=i)&amp;&amp;(k==0))
    l=1;
  else
    l=0;
  k=i;

  delay(20);
}

/*
if(Serial.available()) {
    int inByte = Serial.read();
    if(inByte == 'H')
    {
        digitalWrite(2,HIGH);
        digitalWrite(3,LOW);
        delay(3);
    }
    else
    {
       digitalWrite(2,LOW);
        digitalWrite(3,LOW);
        delay(3);
    }
    if(digitalRead(2)==LOW)
          Serial.println(&quot;LOW&quot;);
        else
          Serial.println(&quot;HIGH&quot;);
   digitalWrite(3,HIGH);
        delay(3);
  }
  */
```