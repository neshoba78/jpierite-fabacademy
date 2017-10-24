# Embedded Programming {#embedded-programming}

#### Have you:

* [ ] Documented what you learned from reading a microcontroller datasheet.

* [ ] What questions do you have? What would you like to learn more about?

* [ ] Programmed your board

* [ ] Described the programming process/es you used

* [ ] Included your code


[![Embedded programming](https://img.youtube.com/vi/wdKsoC5_NIc/0.jpg)](https://www.youtube.com/watch?v=wdKsoC5_NIc "Embedded programming")

#### 2017 Class Review

[André Rocha](http://archive.fabacademy.org/archives/2017/fablabfct/students/329/week1a.html), FCTFabLab (Portugal), was trying to send a "bootloader" to his ISP. Neil interjected André was misusing the term "bootloader". Going to Neil's "helloEcho" example code, Neil demonstrated that it was just a program that was loaded by a programmer. A bootloader is something different, there are multiple bootloaders available. The processor is designed to be programmed through the ISP interface. It is not directly designed to be programmed from the serial interface. A bootloader is a program that takes a program through the serial interface. An ISP rewrites the whole memory on a processor, but a bootloader will sit on the processor and load programs over itself. In this way, the ISP is no longer needed to program the processor. It's two routes, either you use an ISP to program and rewrite the whole memory of the processor; or you use a bootloader program to load programs and communicate with the board directly.

[Birkir Thor](http://archive.fabacademy.org/archives/2017/fablabhornafjordur/students/201/week8.html), Fab Lab Hornafjordur (Iceland), had a final project to make a guitar. Neil searched for Alex Schaub's [documentation](http://academy.cba.mit.edu/classes/applications_implications/musical_instruments/index.html), and Emma Pareschi reminded him where it was linked. Jens Dyvik had Alex in his lab, they all discussed the final project and the developments on mtm projects at [Fellesverkstedet](https://www.fablabs.io/labs/fellesverkstedet). Returning to Birkir, Neil remarked that his documentation was exactly what should be uploaded to the repository. Birkir outlined the workflow for using the Arduino IDE and an ISP to send a sketch to a board. Arduino IDE was not originally able to program ATTiny. David Mellis demonstrated that it was straight forward to do. To go further with the assignment and demonstrate multiple methods, Neil suggested to burn a bootloader using the Arduino IDE and to try using C to load the program directly.

[Ilia Feldshtein](http://archive.fabacademy.org/archives/2017/fablabisrael/students/104/week8.html), Fab Lab Israel (Israel), at the first plugin, his board got heated. Neil explained that heat means power is going where it shopuldn't. If the board is getting hot. Then, it's "fried". Neil asked if Ilia left off the external pull up resistor on the example board. Ilia said that he left one off between the ATTiny and the button. Neil explained that you do not need a pull up resistor to the button. There is a pull up resistor in the ATTiny that can be turned on. Looking at the datasheet, Neil referred to the I/O port. The pin can be an input or an output. It has an onboard pull up resistor. Logically, you write a 0 or 1 to the pin. If you write a 1 to the pin, it turns on the pull up. Ilia experienced problems with USB identification. The example board, Neil explained, has an FTDI and ISP connection. On the ISP, there is a pin labeled V, this is an output to tell the programmer what voltage the board is operating at. The FTDI header has a VCC pin and it's a power supply. Commercial programmers expect the V pin on the ISP to be an output. If the board is connected through the ISP and not the FTDI. Then, it shouldn't work because the FTDI is the power supply. After trying with the designed board, Ilia tried with a Photon board to practice coding. He then tried coding with an Arduino commercial board. Referring back to Birkir's documentation, Neil reminded Ilia of the workflow that was discussed. While Ilia's back up to the assignment was good, the bill of materials for the example boards are $1's. Once mastered, the goal is to be able to pick a processor, pick the form factor, and pick the peripherals. 

[Javi Burongarcia](http://archive.fabacademy.org/archives/2017/fablabmadridceu/students/257/8-week-embedded-programming.html), Fab Lab Madrid CEU (Spain), had the programmer and the echoboard. He demonstrated both the Arduino IDE and directly with C code. Javi milled away the excess copper from the PCB, Javi is "an aesthetic person". For high frequency or low noise circuit boards, this is important to do. It's optional for this assignment. Javi was a little confused by the code. Neil walked through both the sketch and the C code. In the sketch for the example board, a function called _digitalWrite()_ sends arguments and "magically" writes to a pin. In the C code, Neil uses macros. Going back to the datasheet, Neil explains that each section ends with a description of registers. Direction register (DDR) says do you talk out or in. Port send data out. Pin listens in. In the C code, Neil moves a 1 on to Pin 5. Looking at the clock system, the clock system has its own register. The register says that the processor should click every time the clock ticks. Then, we are telling the register that the LED is an output. The point of the C code is to demonstrate that you only need one line of code to talks to pins or ports. In this way, you are not buffered by a library. Javi has a beautiful example of a baby walker and had a simplified final project "Fab Window" that can be applied in any house.

[Tomás Martín agudo](), Fab Lab Barcelona (Spain), 

Alberto

Damaris


