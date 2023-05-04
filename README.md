# STM32-With-74HC595
Using STM32F103C8 to display 8 led-7-segments by 74HC595

# Project Overview
Note: This is just a simple sample code file, you can refer to it and customize it for your own purposes.

The software for this project consists of 3 files:
* main.c: this is the main file that control led-7-seg using 74HC595.
* Print_Number_74HC595.ioc: this is the file config for STM32 using CubeMX.
* STM32F103C8_74HC595.pdsprj: this is the simulation file using Proteus Professional. I'm using Proteus version: 8.12.

In the main.c file I have designed to display integer numbers from -999 9999 to 9999 9999 on 8 led-7-seg using 8 74HC595 IC

To display integers:
First, I created an LEDCODE array of numbers 0-9 written in hexadecimal, along with LED_OFF and LED_MINUS.

Second, I created a function CLK to clock and Led_Display to display numbers on each led-7-seg.

Finally, I created a function Print_Number to print the input number to 8 led-7-seg.
* If it is a negative number, the led will show a minus sign.
* If less than 8 numbers are displayed, the remaining led-7-seg will turn off.

To do the simulation, you can create a new project using Proteus Professional or use the file I uploaded. Note, my Proteus file is only for version 8.12 and above.

Here are some pictures of the configuration steps for the STM342F103Cx, you can refer to it for more information.

* Using STM32F103Cx.
![step1](https://user-images.githubusercontent.com/131508098/236132058-4b04d5b9-d201-408a-af31-172c0e070058.jpg)

* In SYS, Select Serial Wire.
![serial_wire](https://user-images.githubusercontent.com/131508098/236132171-b543bcfd-f0bc-4d93-a5a4-aa43795c0ad6.jpg)

* Pins_Configuration.
![pin_cofig](https://user-images.githubusercontent.com/131508098/236132393-0c03870e-3701-4fc9-984e-3d643b6e86f4.jpg)

* Select MDK_ARM and generate code.
![mk_arm](https://user-images.githubusercontent.com/131508098/236132506-eafabb17-536a-408d-9ec6-1d610bd2a354.jpg)

* Proteus Simulation.
![simu](https://user-images.githubusercontent.com/131508098/236132598-5ee9a6f9-e6d9-4dd6-8ca1-5229b24a40b9.jpg)

* Proteus Running.
![example](https://user-images.githubusercontent.com/131508098/236132991-52daaf3c-c20b-4552-bac2-098f1dbb97ba.jpg)


# Feedback
If you have any contribution to improve the project, please contact me by email: quynh.nm1808@gmail.com

I will acknowledge and edit to make the project more complete.
