# bmxRandomStart
Overview

This project uses an Arduino Uno R3, a micro speaker, with a potentiometer in series to control the volume, a MOSTFET transistor, 
and LED lights to simulate the random start sequence that is used at the start of every BMX race.

Hardware Used
* Arduino Uno R3
* BS170 MOSFET Transistor
* 10kΩ Potentiometer
* 2W 4Ω Micro-Ppeaker
* LED Lights (1 Red, 2 Yellow, 1 Green)
* 220Ω Resistors
* Breadboard
* Jumper Wires

Skills Demonstrated
* Embedded C++
* Circuit design
* Use of transistors, resistors, and potentiometers
* Writing digital outputs
* Troubleshooting and debugging

How it works

Upon start up, the Arduino will read an analog input from an analog pin with nothing connected, giving a pseudo random output for the random seed.
A random time from 0.1 seconds to 2.7 seconds will be delayed before starting the sequence. The program then follows a sequence of 3 60ms beeps with 60ms
of silence between each one, followed by a forth longer beep, at 2.25s. At the same time each tone statement executes, a digitalWrite statement
lights up an LED light.

Results

The sequence following the random delay follows the exact timing and tone of the random start gates defined by USABMX regulations, as well as what
is used in the Olympic BMX races. Having the ability to practice your reflexes to the exact sequence while not at the track can give users an
advantage over other racers.

Images

<img width="398" height="412" alt="BMXRaceGateImage" src="https://github.com/user-attachments/assets/c38f0f23-883c-4312-b592-803401ccba55" />
<img width="400" height="435" alt="BMXPracticeGateGIF" src="https://github.com/user-attachments/assets/5888c2c7-42f0-4640-9af3-857cbade5293" />


