Functions of the PIC16F883:
- Count the amount of individual coins inputted.
- Count the currency value of said coins
- Display the value of currency balance that was summed as well as the total amount of indivual coins, cycle through the two three times
- Display the data through a (at least four digit) 7-segment display
- Disable the display after a certain amount of time has elapsed to save power (10 seconds?)
- Put the PIC16F883 to sleep until an interrupt occurs when coin input, push-button for display, or the optional RS232 communication (does not activate display)
- Ability to remote in and acces the data through a serial (RS232) terminal (Optional)

Peripherals and tasks:
- Use internal RC Oscillater (8MHz) with prescaler of 8 for 1MHz clock or 0.25MIPS
  Or for faster or more accurate Baud rate, use the optional external crystal (8-20MHz) through the Internal to External clock Switch Option (IESO) controlled by software
  (OSCCON.SCS bit coontrols switching between internal oscillator and the CONFIG1 oscillator setting if IESO is enabled)
- Use Timers to count the time that has elapsed and/or tell the current time (TMR1)
- Use Interrupt On Change (IOC) on PORTB to detect which and how many coins were inputted
  Use the internal Weak Pullups (WPUB) on PORTB
  Use a General Purpose register to keep track on how many coins were inputted when IOC on PORTB was detected
  
----OPTIONAL----
- Utilize the EUSART peripheral with a BAUD rate of 300 for external communication, (SYNC = 0, BGRH = 0, BGR16 = 0)
  Or a BAUD rate of 9600 (default on many devices) with a clock rate of 2MHZ, prescaler of 4, (SYNC = 0, BGRH = 1, BGR16 = 0)
-Using a RS232 interface such as a MAX232 or equivalent for voltage conversion of +-8V
