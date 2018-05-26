# Interface and Application Programming {#interface-and-application-programming}

#### Have you:

* [ ] Described your process using words/images/screenshots

* [ ] Explained the the GUI that you made and how you did it

* [ ] Outlined problems and how you fixed them

* [ ] Included original code

#### 2018 Class Notes

This week is about desktop applications. The assignment is to write an application that interface with an input or output device. The assumption is that the data will be read through a serial port.

A Hello World started as the shortest program to produce an output. We have been using C to control the microcontroller. In C, we compile. In Java, we compile to a byte code and that can run on any platform. Anroid is sort of based on Java, and there is a sensitive legal discussion. Processing, if you like the Arduino IDe, then you will like this. p5 is Javascript with the spirit of Processing. For visual model-based programming, there is LabView, Scratch, and those sort of environments. AppInventor is also visual data flow. Bash is a standard Unix shell. Python builds to a great extent on APL. It is well-documented. Perl and Ruby are related in spirit, as script languages. There are tools to compile them, but you can run them through an interpreter. Javascript started as simple scripting for web pages. Mozilla runs MDN which is a good repo for documentation. There is a whole development suite for Javascript built-in to browsers like Firefox. Mods, written by Neil, is also a visual model-based programming environment.

We have been using the FTDI cable to do seral communications. Python has a library to talk to serial ports. `import serial` tells the program how to talk to serial. A browser can not talk to serial, but Node can. python-ftdi and node ftdi let you talk to individual pins, but it won't be necessary for this week. GPIB, VISa, PyVISA are ways to talk to test equipment. MOTT, XMPP, IFTT help to talk to groups of devices. Sockets are how you talk to the Internet. With sockets, you can send messages to anywhere on the Internet. For security, browsers cannot do that. There are web sockets that can send messages to anywhere on the Internet. Node has a web socket server.

In order to store data, you can use flat files. It is perfectly fine to store data in file, and then read the data into memory.

For user interface, if we look at the distance interface from input week, then we will see that Python uses Tk which is a standard for graphics. wx is another platform of widget libraries. Qt is another set of widgets for Python. HTML forms is another set of widgets that is older, but it can be called from Java. jQuery is another widget set. Because of the economics and ease, there are many ways to organize multiple Java apps. Meteor and many other examples are frameworks for Javascript development. 

In terms of graphics, you may want to do visual representations of what is happening. Web standards support multiple graphical elements. Canvas elements in HTML are bitmaps. To talk to web pages directly, you need a web socket. The difference between canvas and SVG is that you can create objects directly on webpages that can be manipulated. With canvas, frame by frame you need to redraw. Three.js uses WebGL to use Javascript to talk to the GPU. The GPU talks to the browser efficiently. WebVR is a maturing standard for talking to virtual reality devices. THREE.VRController is a bridge between Three.js and virtual reality devices. OpenGL is under the hood but can be used in C and Python. For game engines, you can use Unity and Unreal to talk to serial devices

For sound, SDL is a standard. PyGame is a Python binding for SDL. HTML5 is a grab bag for multimedia features. HTML5 added media, such as with the Web Audio API. 



#### 2018 Class Review

Carolina Portugal, she did not have any background in programming. Her interface was a basic happy or sad face when a button is pressed. 

Solomon Embafrash, had problems with Python. His interface was detailed in his Final Project documentation.

Rutvij Pathak, his main motive was to have an interface for his photogrammetry final project. He was using a commercial Arduino. He started to work in Processing, but ultimately opted for Python.

Alec Mathewson, used Max patch to connect his interface. Max was named for Max Matthews who worked on digital music and was a mentor to Neil at Bell Labs.

Shefa Jaber, built the graphical interface with Processing. Irbid used an Arduino and breadboard for the electronics as they were waiting for an order from Fab Foundation.

Joris Navarro, used Xamarin to create a cross platform mobile app. It can create a native iOS and Android application. It is also 

Jari, used Unity to create an interface. He went to the Unity asset store to create a game level that talks to his Fabduino. When a character in the game world touches a powr up, an LED will light up on the board.

Antonio Garosi, used Unity to create a 2D game that talked to an Arduino commercial board and a breadboard.

Marcello, used Open CV to do facial recognition that then manipulated a stepper motor.

Hasan, used Node, Plotly, and JSONP to create a Real-Time sinewave graph. He needed to interface to a microcontroller.