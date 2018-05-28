# Embedded Networking and Communications {#embedded-networking-and-communications}

#### Have you:

* [ ] Described your design and fabrication process using words/images/screenshots.

* [ ] Explained the programming process/es you used.

* [ ] Outlined problems and how you fixed them

* [ ] Included original design files and code

#### 2018 Class Notes

The assignment for this week is to design and build a wired or a wireless network connecting at least two processors. 

Why network? Location is an obvious motive to send . Parallelism, devices with big processors can do many things at once. You can do a parallel system in which each processor has a separate thread. Modularity, helps to develop modules separately for development and debugging purposes. Interference, current from big processors can affect multiple components. Separate modules cut down on the possibility of interference.

The example boards employ a simple serial bus. The host board has single Tx/Rx lines that nodes in the network can use to talk to each other. The important distinction is that each board is addressed. In Neil's example, he hard codes addresses for each board. I2C is a standard that used to be proprietary but is now widely supported. In Input week, the accelerometer employs I2C. SPI, this is used in the in the in system programmer. SD Cards support SPI. In SPI, you write from the host to the target. If you want the target to talk to you, then you have to talk to it. V-USB is a software implementation of USB that can run down to ATTiny45. It is USB 1, but for interfacing you shouldn't have to care about that. These adaptively clock by listening to the host. The difference between a bus and a network, there are nodes hanging off of a bus where as a network does not care where you are in the wold.

> OSI layers
> 7: application (HTTP) - the actual application
> 6: presentation (SSL) - how you present the data
> 5: session (RPC) - how you set the conservations
> 4: transport (TCP, UDP) - what goes when
> 3: network (IP) - how you make addresses
> 2: data link (MAC) - who gets to talk
> 1: physical (PHY) - physcial media


#### 2018 Review Notes

Aitor Aloa, is using Gitbook like me. He is considering migrating his repo to MK dot. He did the Hello Bus 45 and two nodes. He used Neil's code to program the board. Neil suggested that Aitor change the code just a little bit.

Abdulla, he only did research this week, due to being in a competition. He proposes to do two boards that will use Bluetooth. Neil suggested Fastel as a vendor for good Bluetooth modules.

Georges Hanna, his final project is an interactive lamp. He was behind on the weekly assignments. Neil showed a Bluetooth component at DigiKey which is "trivially compatible" with the ATTiny45. The component acts as a serial connection and similar to a text terminal.

Murad Saadeh, he used a ESP8266 and was able to send packets.

Coral, she worked on the I2C. Neil stated that I2C is a bit more complex for a networking beginner. Coral tried going through a tutorial on Sparkfun on why I2C is better than asynchronous.

Jari Uusitalo, he used board created in previous weeks. He created an Rx/Tx hub that talks to the boards from previous weeks. He demonstrated how modules can be connected by an external master board to create a system.

Tanvir Khorajiya, used bluetooth to sendthe data. He is broadcasting data to the boards through Bluetooth over a mobile app.

