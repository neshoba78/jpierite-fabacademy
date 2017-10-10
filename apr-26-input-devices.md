# Input Devices {#input-devices}

#### Have you:

* [ ] Described your design and fabrication process using words/images/screenshots.

* [ ] Explained the programming process/es you used and how the microcontroller datasheet helped you.

* [ ] Explained problems and how you fixed them

* [ ] Included original design files and code


#### Class Review 2016

João Leão, Fab Lab Barcelona, tried to do the step from Matt. The problems that he encountered were centered around libraries that needed to be installed. The attempt was around trying to run functions that were included in Node.js, which was a different version from his local installation. Neil reminded him to include design files for repo uploads. One comment that Neil made was that the black plastic connector on the FTDI connector should be mounted on the board. If this is not included in the design, every time the cable is connected to the board it will bend the solder joints.

Roman Kutyin, Fab Lab WOMA (Paris, France), proposed a project that would make an oxymeter glow, which is a device that regulates breathing in life threatenting situations. Neil asked if the blood oxygen would be measured by IR reflection? This was the proposed solution for Roman. There was a specific module discussed which Neil was concerned about in regards to price point. He then suggested to Roman to shop at a vendor like Digikey to be able to pick the frequency of emitters and detectors. In my personal experience, I select parts at Digikey but then take the manuafacturer part number and enter it into Octopart. The second site gives the availability of parts for a range of websites. Neil asked a follow up to Roman about the example of synchronous detection. Neil's solution is a scale down of a lock-in amplifier which is $1000s. The LED sends light out. The detector measures ambient light and the emitted light from the LED which is bounced off a finger. In the code, Neil measures the difference of the wave signal when the light is on versus when it is off. The smoothing filter is calculated by _=(1 - E)*filteredReading + E*newReading_. Discussing his input devices project, Roman mentioned using assembly for the code. Neil advocated for the use of C, due to Roman's concern about speed. GCC-AVR, according to Neil, is a very good compiler and C has many single cycle hardware instructions that alleviate the concern of processing speed (with the caveat of dealing with data types that aren't primitive or multi-byte numbers). Aside from the concern about code, the design of the board was related to Roman's final project proposal.

Luca Giacolini, Fab Lab Toscana (Italy), did not have an input device for his final project. He designed a sensor breakout board which was based on previous board layouts in the repository. Neil liked the board as part of a breakout system, similar to an Arduino header. Luca not only milled PCB. He also used a Trotec fiber laser to etch into PCB, using a one micron fibre. Luca could not get the smoothest results, as he attempted to etch Daniele Ingrassia's satshakit. Neil said that this documentation was a good example of system architecture. Instead of making a monolithic system, Luca broke it apart and made modular components. In this way, Luca could incrementally debug subsystems. As a follow up, Neil reviewed capacitance. He covered two versions of capacitance. One was just loading. It measures whatever is in the vicinity out to the room ground, but that is a measurement of all loading. The other version includes a transmitter and a receiver. This is the preferred version as it allows the user to control, rather than relying on the room to help return. That second version creates a field which can sense when someone is pressing a button, but also when someone is going to press a button.

Diego Bustos, Fab Lab Yachay (Ecuador), started with the example on the class page. He encountered problems with the server connection to the Arduino and the PCB board. Previoulsy, he did make boards that work. What seemed to happen is that he was using the Arduino IDE to program the board, but Neil suggested that Diego use only the C code that was posted on the class page.

Dmitry Ershov, Fab Lab Polytech (Russia), etched onto a glass reinforced board. Neil reminded people of FR1 in the inventory. Milling of boards works with the FR1, but would break glass reinforced boards. Etching is fine, but creates a chemical waste that is an environmental concern. It also requires extra steps for the lithography.

Cindy Kohtala, Fab Lab Aalto (Finland), was not current; but she was working on a PhD dissertation and still managing to particiapate.

Bas Withagen asked a question about the DHT11 humidity sensor and the getting the component to work/fit with the ATTiny45. Fiore Basile said that the sensor does work. There are up to a dozen libraries to support. Neil advocated for capacitance as a way to DIY a humidity sensor.

Fiore Basile asked a question about the digital version of the MEMS microphone. This introduced the I2S protocol which seemed to be a "non-trivial" threshold for microcontrollers. Neil supposed that you may need to use an XMega board vs. an ATTiny. Working with the specific protocol would involve developing a codec. It is much simpler to use the analog version of MEMS and ust do the A to D conversion. Bas added that I2S is a fairly old protocol which was used for 52 speed CD-ROM players.

#### Class Notes 2017

The goal is to take a microcontroller board that is an original design, add a sensor, and measure something. This can be used toward the final project.

We started by reviewing the ATTiny45 which is an eight pin AVR microcontroller. In the ATTiny45, there are multiple kinds of inputs. There are pins that read logic, high and low level. There's a comparator that reads the difference between two voltages. There's an A to D convertere that measures absolute voltage. There's a counter that measures time and events. To understand the assignment, a comprehensive review is required.

Device communication is done through a serial interface. Installation on a host computer is required. PySerial through Node.js there are seevral options for a serial interface. Knowledge of bit timing is essential. Serial communication needs a 1% tolerance. To debug bit timing, the use of an oscilloscope is recommended.

Time delay can be set in the C code. In the clocks section of the microcontroller datasheet, there is detail regarding the OSCAL register. You can send values to that register to make time go faster or slower. The simpler solution is to set values in the C code. In the example of a switch, resistors pull up on the signal while a switch pulls the signal down.

For motion detection, there are pyroelectric sensors which measuring thermoradiation. A human body emits thermoradiation. Alternatively, Doppler radar is scaling down and can measure radio waves.

Sonar detection, requires a good reflective surface. Fuzzy or angled surfaces will cause a fault. Applications for distance measuring can be found in sinks and toilets. An alternative to sonar is time-of-flight detection which measures the reflection of light back fr4om a relfective surface. Sonar can be good for measuring heights of liquids. Further reading into this subject, I found examples of trade off in regards to the Kinect sensor. Kinect I uses structured light. Kinect II uses time-of-flight which has a trade off between angled and dark surfaces. I thought of this because of recent articles about the applications of sensors and differing results with darker skinned people. The issue is with LED emission and whether or not a surface will reflect or absorb light which would cause a fault in detection.




#### Sources

Pöhlmann, Stefanie T. L. et al. “Evaluation of Kinect 3D Sensor for Healthcare Imaging.” Journal of Medical and Biological Engineering 36.6 (2016): 857–870. PMC. Web. 10 Oct. 2017.

Smith, Adam. “These automatic soap dispensers don't work for black people.” Metro, 13 July 2017, metro.co.uk/2017/07/13/racist-soap-dispensers-dont-work-for-black-people-6775909/.