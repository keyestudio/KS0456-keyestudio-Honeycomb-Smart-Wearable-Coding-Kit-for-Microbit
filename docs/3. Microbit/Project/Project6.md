### Project 6 Geomagnetic Sensor

![](media/image-20260122172823201.png)

**1.Project Description**

This project aims to explain the use of the Micro: bit geomagnetic sensor, which can not only detect the strength of the geomagnetic field, but also be used as a compass to find bearings. It is also an important part of the attitude heading reference system (AHRS). 

Micro: Bit main board V2 uses LSM303AGR geomagnetic sensor, and the dynamic range of magnetic field is ±50 gauss. In the board, the magnetometer module is used in both magnetic detection and compass. In this experiment, the compass will be introduced first, and then the original data of the magnetometer will be checked.

The main component of a common compass is a magnetic needle, which can be rotated by the geomagnetic field and point toward the geomagnetic North Pole (which is near the geographic South Pole) to determine direction.

**2.Components Needed**

-   Micro:bit main board V2 \*1

-   Micro USB cable\*1

**3.Test Code 1**

Link computer with micro:bit board by micro USB cable, and program in MakeCode editor.

（1）A. Click“Input”→“more”→“calibrate compass”.

B. Lay down it into block“on start”.

![](media/image-20260122173013531.png)

（2）A. Go to“Input”→“on button A pressed”.

B. Enter“Basic”→“show number”, put it into“on button A pressed”block;

C. Tap“Input”→“compass heading(℃)”， and place it into“show number”.

![](media/image-20260122173038830.png)

Complete Program：

![](media/image-20260122173049989.png)

Select“JavaScript" and“Python”to switch into JavaScript and Python language code:

![](media/image-20260122173102591.png)

![](media/image-20260122173108390.png)

**4.Test Results 1**

After uploading test code to micro:bit main board V2 and powering the board via the USB cable, and pressing the button A, the board asks us to calibrate compass and the LED dot matrix shows “TILT TO FILL SCREEN”. Then enter the calibration page. Rotate the board until all 25 LEDs are on red as shown below.

![](media/image-20260122173134326.png)

After that, a smile pattern ![](media/image-20260122173148875.png)appears, which implies the calibration is done. When the calibration process is completed, pressing the button A will make the magnetometer reading display directly on the screen. And the direction north, east, south and west correspond to 0°, 90°, 180° and 270°.

**5.Test Code 2**

![](media/image-20260122173220228.png)

This module can keep reading data to determine direction, so does point to the current magnetic North Pole by arrow.

![](media/image-20260122173235744.png)

For the above picture, the arrow pointing to the upper right when the value ranges from 292.5 to 337.5. Since 0.5 can’t be input in the code the values we get are 293 and 338.

Link computer with micro:bit board by micro USB cable, and program in MakeCode editor.

(1)

A. Enter“Input”→ “more”→“calibrate compass”.

B. Move“calibrate compass”into“on start”![](media/image-20260122173424450.png).

(2)

A. Click“Variables”→“Make a Variable...”→“New variable name：”

B. Input“x”in the blank box and click“OK”, and the variable “x” is generated.

C. Drag out“set x to”into“forever”block![](media/image-20260122173509222.png).

(3)

A. Go to“Input”→“compass heading(℃)”, and keep it into“0”box![](media/image-20260122173522597.png).



B. Tap“Logic”→“if...then...else”, leave it below block“sex x to compass heading”, then click![](media/image-20260122173535179.png)icon for 6 times.

(4)

A. Place“and”into“true”block,.

B. Then move“=”block to the left box of “and” .

C. Click“Variables”to drag“x”to the left “0”box, change 0 into 293 and set to “≥”; 

D. Then copy“x≥293”once and leave it to the right “0”box and set to“x\<338”![](media/image-20260122173602355.png).

(5)

A. Go to“Basic”→“show leds” .

B. Lay it down beneath ![](media/image-20260122173619559.png)block, then click“show leds”and the pattern ![](media/image-20260122173913687.png)appears.

![](media/image-20260122173926917.png)

(6)

A. Duplicate ![](media/image-20260122173945352.png)for 6 times. 

B. Separately leave them into the blank boxes behind “else if”. 

C. Set to“x≥23 and x\<68”,“x≥68 and x\<113 ”,“x≥113 and x\<158 ”,“x≥158 and x\<203 ”,“x≥203 and x\<248 ”,“x≥248 and x\<293 ”respectively.

D. Then copy “show leds”for 7 times and keep them below the “else if.......then” block respectively. Click the blue boxes to form the pattern“![](media/image-20260122174200792.png)","![image-20260122174218298](media/image-20260122174218298.png)","![](media/image-20260122174228767.png)","![](media/image-20260122174237741.png)","![](media/image-20260122174258207.png)","![](media/image-20260122174313815.png)"and"![](media/image-20260122174328753.png)".

Complete Program：

![](media/image-20260126122245102.png)

![](media/image-20260126122253030.png)

![](media/image-20260126122306062.png)

![](media/image-20260126122312169.png)

Select“JavaScript" and“Python”to switch into JavaScript and Python language code:

![](media/image-20260122174348726.png)

![](media/image-20260122174355284.png)

![](media/image-20260122174400775.png)

![](media/image-20260122174406472.png)

**6.Test Results 2**

Upload code 2 and plug micro:bit to power. After calibration, tilt micro:bit board, the LED dot matrix displays the direction signs. 

 