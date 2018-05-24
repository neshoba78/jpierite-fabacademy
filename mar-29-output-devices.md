# Output Devices {#output-devices}

#### Have you:

* [x] Described your design and fabrication process using words/images/screenshots.

* [ ] Explained the programming process/es you used and how the microcontroller datasheet helped you.

* [ ] Outlined problems and how you fixed them

* [x] Included original design files and code

* Design files:[ Right click + Save As](/uploads/hello.RGB.45.zip)

#### Fabricating the Board

![](/assets/Screenshot from 2018-05-24 15-44-38.png)

Copying the traces by connections via GIMP. Process detailed in [Feb 28: electronics design](mar-01-electronics-design.md).

![](/assets/Screenshot from 2018-05-24 17-21-17.png)

Routing the board in Eagle. Process detailed in [Feb 28: electronics design](mar-01-electronics-design.md).

**2018 Class Notes**

Types of output devices covered in this class: lights, video, sound, and motors. On electrical safety, it doesn't take much current to do serious harm. Outside of the body, it takes a M ohm to go internal. A kilovolt per millimeter leads to dielectric breakdown, which discharges through skin or wires.

Big power supply capacitors stay charged for a long time. Inductive flyback can happen in solenoid when you switch them on and off.

For the homework, use power supplies. Open frame supplies come in two kinds. Switching makes noisy power. Linear supplies make cleaner power, but they are more expensive and generate more heat. Benchtop supplies are regulated. The group assignment is to measure the power consumption of your output device. A regulated power supply has a knob which sets the voltage or current. A sense resistor at .1 ohm can be used to measure with an oscilloscope.

For RGB LED, the part has three light emitting diodes and cathodes with a common anode. Current is alphabetical, it goes from anode to cathode. For the board each cathode has a resistor going to a pin. A pin on the processor can sink ~50 mA. The resistors set the current. The blue cathode is less efficient than the other two cathodes. Therefore, a smaller resistor is set on that pin.

For LED array, you can use a trick called Charlieplexing. LEDs can only conduct in one direction. Wires can go to rows and columns. Pins can be disconnected. Pins can be low which means current goes in. When the pins are high, current goes out. For n pins, you can drive n x n - 1 LEDs. This can be done additively with a combination of NC mini milling and vinyl (epoxy and copper tape).

For LCD modules, four pins are for data the others are for controlling the LCD. In the code, the process is to initialize the LCD. There is a very particular sequence. To talk to the module, there is a very particular sequence to toggle. `PROGMEM` accesses the Flash memory. Organic LEDs are creeping down in price and give you more pixels. 


