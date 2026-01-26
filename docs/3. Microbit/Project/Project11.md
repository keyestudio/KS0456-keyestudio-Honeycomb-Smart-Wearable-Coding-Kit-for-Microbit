### Project 11 Microphone

![](media/image-20260126123149920.png)

**1.Project Description**

The Micro: Bit main board V2 is built with a microphone which can test the volume of ambient environment. When you clap, the microphone LED indicator will turn on. Since it can measure the intensity of sound, you can make a noise scale or disco lighting changing with music. The microphone is placed on the opposite side of the microphone LED indicator and in proximity with holes that lets sound  pass.When the board detects sound, the LED indicator lights up.

**2.Components Needed**

-   Micro:bit main board V2 \*1

-   Micro USB cable\*1

**3.Test Code 1**

Link computer with micro:bit board by micro USB cable, and program in MakeCode editor.

( 1 ) Delete block“on start”and“forever”;

( 2 ) Enter“Input”module to find and drag“on loud sound”;

Enter“Basic”module to find and drag “show number”into “on loud sound”block ;

![](media/image-20260123104441084.png)

( 3 )Copy![](media/image-20260123104454388.png)once; Click the little triangle of “lond” to choose”quiet”; Click the little triangle of “![](media/image-20260123104507585.png)” to choose”![](media/image-20260123104521594.png)";

![](media/image-20260123104543565.png)

Complete Program：

![](media/image-20260123104555448.png)

Select“JavaScript" and“Python”to switch into JavaScript and Python language code:

![](media/image-20260123104606617.png)

![](media/image-20260126134953059.png)

**4.Test Results 1**

Uploading test code to micro:bit main board V2 and powering the board via the USB cable, the LED dot matrix displays pattern![](media/image-20260123104638734.png)when you claps and pattern![](media/image-20260123104650635.png)when it is quiet around.

**5.Test Code 2**

Link computer with micro:bit board by micro USB cable, and program in MakeCode editor.

( 1 )Enter“Advanced”module→ choose“Serial”to find and drag“serial redirect to USB”into “on start”block ;

![](media/image-20260123104734037.png)

( 2 )Enter“Variables”module→ choose“Make a Variable”→ input “maxSound”→click “OK”,variable ”maxSound”is established;

Enter“Variables”module to find and drag“set maxSound to 0”into “on start”block ;

![](media/image-20260123104750025.png)

( 3 )Enter“Logic”module to find and drag“if true then...else”into “forever” block ; Enter“Input”module to find and dragbutton A is pressed”into “then” ;

![](media/image-20260123105019078.png)

( 4 )Enter“Basic”module to find and drag“show number”into “then” ; Enter“Variables”module to find and drag“maxSound”into “0” ;

![](media/image-20260123105029598.png)

( 5 )Establish variable“soundLevel”;

Enter“Variables”module to find and drag“set soundLevel to 0”into “else”;

Enter“Input”module to find and drag“sound level” into “0”;

![](media/image-20260123105044876.png)

( 6 )Enter“Led”module to find and drag“plot bar graph of 0 up to 0” into “else”;

Enter“Variables”module to find and drag“soundLevel”into the “0”behind “of”;

Change the “0”behind “up” to “255”;

![](media/image-20260123105100648.png)

( 7 )Enter“Logic”module to find and drag“if true then”into “else”block ;

Enter“Logic”module to find and drag“0 \> 0”into “then” ;

Enter“Variables”module to find and drag“soundLevel”into “0”on the left side of “0-0” ;

Enter“Variables”module to find and drag“maxSound” into “0” on the right side;

![](media/image-20260123105113917.png)

( 8 )Enter“Variables”module to find and drag“set maxSound to 0”into the second “then” ;

Enter“Variables”module to find and drag“soundLevel”into the “0” ;

![](media/image-20260123105126408.png)

Complete Program：

![](media/image-20260123105136210.png)

Select “JavaScript" and“Python”to switch into JavaScript and Python language code:

![](media/image-20260123105148963.png)

![](media/image-20260123105155381.png)

**6.Test Results 2**

Upload test code to micro:bit main board V2, power the board via the USB cable and click “Show console Device”as shown below.

![](media/image-20260123105216856.png)

When the sound is louder around, the sound value shows in the serial port is bigger as shown below.

![](media/image-20260123105233068.png)

What’s more, when pressing the button A, the LED dot matrix displays the value of the biggest volume( please note that the biggest volume can be reset via the Reset button on the other side of the board ) while when clapping, the LED dot matrix shows the pattern of the sound.