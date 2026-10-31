# bmxRandomStart
Overview

This project uses an Arduino Uno R3, a micro speaker, with a potentiometer in series to control the volume, a MOSTFET transistor, 
and LED lights to simulate the random start sequence that is used at the start of every BMX race, and test reaction time, with results
being sent to a LCD display.

Hardware Used
* Arduino Uno R3
* BS170 MOSFET Transistor
* 10kΩ Potentiometer
* 2W 4Ω Micro-Ppeaker
* LED Lights (1 Red, 2 Yellow, 1 Green)
* 220Ω Resistors
* Breadboard
* Jumper Wires
* 12C LCD 1602 display
* E-switch push button

Skills Demonstrated
* Embedded C++
* Circuit design
* Use of transistors, resistors, and potentiometers
* Writing digital outputs
* Troubleshooting and debugging
* LCD displays

How it works

Upon start up, the Arduino will read an analog input from an analog pin with nothing connected, giving a pseudo random output for the random seed.
A random time from 0.1 seconds to 2.7 seconds will be delayed before starting the sequence. The program then follows a sequence of 3 60ms beeps with 60ms
of silence between each one, followed by a forth longer beep, at 2.25s. At the same time each tone statement executes, a digitalWrite statement
lights up an LED light. After the sequence of lights, the user pressed a button. Their reaction time is then displayed on the LCD display.

Results

The sequence following the random delay follows the exact timing and tone of the random start gates defined by USABMX regulations, as well as what
is used in the Olympic BMX races. Having the ability to practice your reflexes to the exact sequence while not at the track can give users an
advantage over other racers.

Images

<img width="344" height="214" alt="bmxpracticefullcircuit" src="https://github.com/user-attachments/assets/efdda539-4033-49cd-9dd5-2b2a0b71e09b" />

<img width="399" height="452" alt="ezgif-cropped" src="https://github.com/user-attachments/assets/89f6151f-0e8f-45d6-8499-be1ee1be4ae6" />

<img width="363" height="336" alt="bmxpracticemicro" src="https://github.com/user-attachments/assets/0d711e9a-2d02-4091-a2f1-28dabc30fa8b" />




