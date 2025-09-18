Scope:
This is as of Prototype Alpha stage.
Demonstrates power generation from a DC motor that will be stored for later use in a battery.

Microcontroller
Atmega328P, PDIP .

Programming through Arduino USB Link.

Battery Management System: SparkFun Battery Babysitter 
(BQ24075 Charger) & (BQ27441-G1 Fuel Gauge)
Communicates with the atmega328P through I2C communication

Buck-boost converter: TPS63060
Allows for controlling the voltage going into the battery charger, giving a more stable input than directly from the motor.
A second one will be used to regulate the output when discharging the battery
Can be enabled or disabled by the atmega328P by GPIO

Display: 1602 LCD Display (datasheet). 
Display will need to be fitted with enclosure
Communicates through 8bit parallel communication with the atmega328P GPIO

Firmware
Needs to be created

Future Improvements
A stronger motor can be implemented for higher power generation
With a larger battery, we could store more energy giving the opportunity to output even more power.


Decisions made:

DC motor selected for easier use
Atmega328P microcontroller selected to control the operation
Two buck-boost converters will be used
I2C, 8bit parallel communication from microcontroller and peripherals
Internal comparator and external op amp used for reading motor rotation and power generation for cost reduction.
All active components will be powered by the internal battery to not draw power from the unfiltered DC generated power.
Soft latch circuit to turn on the device or off
1602 LCD screen selected for ease of programming
SparkFun Battery Babysitter and Adafruit TPS63060 selected for the battery charging
Hand crank with gear ratio for proof of concept prototype for the power generation
