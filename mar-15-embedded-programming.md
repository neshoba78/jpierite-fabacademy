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

Ilia

Alberto

Damaris


