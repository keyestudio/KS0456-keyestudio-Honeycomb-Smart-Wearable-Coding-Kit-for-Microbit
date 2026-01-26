### Project 4 Programmable Buttons

![](media/image-20260122152910906.png)

**1.Project Description**

Buttons can be used to control circuits. In an integrated circuit with a button, the circuit is connected when pressing the button and it is open the other way around.

Micro: Bit main board V2 boasts three buttons, two are programmable buttons(marked with A and B), and the one on the other side is a reset button. By pressing the two programmable buttons can input three different signals. We can press button A or B alone or press them together and the LED dot matrix shows A,B and AB respectively. Let’s get tarted.

**2.Components Needed**

-   Micro:bit main board V2 \*1

-   Micro USB cable\*1

**3.Test Code 1**

Link computer with micro:bit board by micro USB cable, and program in MakeCode editor.

（1）Delete“on start”and“forever”firstly，then click“Input”→“on button A pressed”.

（2）A. Click“Basic”→“show string”;

B. Then place it into“on button A pressed”block, change “Hello!”into“A”.

![](media/image-20260122153157831.png)

(2)Copy code string![](media/image-20260122153212815.png)once, tap the drop-down button“A”to select“B”and modify,character“A”into“B”.![](media/image-20260122153303935.png)

(3)Copy![](media/image-20260122153326242.png)once，and set to“on button A+B pressed”and“show string “AB”![](media/image-20260122153344937.png).

Complete Code:

![](media/image-20260122153420799.png)

Select “JavaScript" and“Python”to switch into JavaScript and Python language code:

![](media/image-20260122153433645.png)

![](media/image-20260122153439666.png)

**4.Test Results 1**

After uploading test code 1 to micro:bit main board V2 and powering the main board via the USB cable, the 5\*5 LED dot matrix shows A if button A is pressed, B if button B pressed, and AB if button A and B pressed together.

**5.Test Code 2**

(1) A. Click“Led”→“more”→“led enable false”.

B. Put it into the block“on start”，click drop-down triangle button to select“true”![](media/image-20260122153532133.png) .

(2) A. Tap“Variables”→“Make a Variable...”→“New variable name：”

B. Enter“item”in the dialog box and click“OK”，then variable“item”is produced. And move“set item to 0”into“on start”block![](media/image-20260126115154933.png).

(3)A. Click“Input”→“on button A pressed”.

B. Go to“Variables”→“ change item by 1 ”.

C. Place it into“on button A pressed”and 1 is modified into![](media/image-20260122171424057.png).

(4) Duplicate![](media/image-20260122171444050.png)code string once, click the drop-down button to select“B”，then set“change item by -5”.

![](media/image-20260122171456256.png)

(5)A. Enter“Led”→“plot bar graph of 0 up to 0”.

B. Keep it into“forever”block.

C. Go to“Variables”to move“item”into 0 box，change 0 into 25.

![](media/image-20260122171524329.png)

(6) A. Go to“Logic”to move out “if...true...then...”and “=”blocks.

B. Keep“=”into“true”box and set to “\>”.

C. Select“item”in the “Variables” and lay it down at left box of “\>”，change 0 into 25；Enter “Variables” to drag “set item to 0” block into “if...true..then...”, alter 0 into 25.

D. Enter“Variables”to drag“set item to 0”block into“if...true..then...”, alter 0 into 25.

![](media/image-20260122171628747.png)

(7)A. Replicate code string![](media/image-20260122171638835.png)once .

B. “\>” is modified into “\<” and 25 is changed into 0.

C. Leave it beneath![](media/image-20260122171711986.png)code string.

![](media/image-20260122171737745.png)

Complete Program：

![](media/image-20260122171748259.png)

Select “JavaScript" and“Python”to switch into JavaScript and Python language code:

![](media/image-20260122171800667.png)

![](media/image-20260122171809191.png)

**6.Test Results 2**

Uploading test code 2 to micro:bit main board V2 and powering the main board via the USB cable, when pressing the button A the LEDs turning red increase while when pressing the button B the LEDs turning red reduce.