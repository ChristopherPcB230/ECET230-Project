LOG BOOK


As of 9/9/2025
- Idea was established (harvesting mechanical power to electrical; bike generator).
- Determined the basic functions.
- Determined basic power structures needed for the project.
- display (speed, power gen meter, total distance, time elapsed).

Known problems
* type of display
* tachometer?? Through ac wave? Or through halleffect?
* should the BMS handle both input and output?
* power bank for BMS?
*Where to get the motor?
AC or DC motor?
* do we need 2 DC/DC for both output and input? Or does BMS handle them?


As of 9/11/2025
- Block diagram made (rough outline) 

Known Problems
* does the Battery need a Dc/dc For output?
* IF AC motor used.. The tachometer can be electrically driven using a comparator and evaluate the ‘highs’...
* IF DC motor is used, not a lot of electromagnetic field .: hall-effect counter can be used
*regulator needed after Dc/Dc and generator?


As of 9/16/2025
Github Repository made
Some components selected, DC motor and battery components
Schematic started
Design decisions narrowed

Known Problems

* Find a way to write firmware for I2C communication with the BMS peripheral
* LCD screen communication 8bit parallel or 4bit parallel communication?
* Instead of tachometer and hall effect sensor, what if shunt resistor is used in series with op amp and comparator to find the rotation from human uneven pulses when operating the device. As well as computing the power that is generated with minimal power loss from the shunt.
* Peripherals need to be purchased if not designed from scratch.
