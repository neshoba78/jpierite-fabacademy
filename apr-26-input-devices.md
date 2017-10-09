# Input Devices {#input-devices}

#### Have you:

* [ ] Described your design and fabrication process using words/images/screenshots.

* [ ] Explained the programming process/es you used and how the microcontroller datasheet helped you.

* [ ] Explained problems and how you fixed them

* [ ] Included original design files and code


#### Class Review 2016

João Leão from Fab Lab Barcelona tried to do the step from Matt. The problems that he encountered were centered around libraries that needed to be installed. The attempt was around trying to run functions that were included in Node.js, which was a different version from his local installation. Neil reminded him to include design files for repo uploads. One comment that Neil made was that the black plastic connector on the FTDI connector should be mounted on the board. If this is not included in the design, every time the cable is connected to the board it will bend the solder joints.

Roman Kutyin from Fab Lab WOMA (Paris, France) proposed a project that would make an oxymeter glow, which is a device that regulates breathing in life threatenting situations. Neil asked if the blood oxygen would be measured by IR reflection? This was the proposed solution for Roman. There was a specific module discussed which Neil was concerned about in regards to price point. He then suggested to Roman to shop at a vendor like Digikey to be able to pick the frequency of emitters and detectors. In my personal experience, I select parts at Digikey but then take the manuafacturer part number and enter it into Octopart. The second site gives the availability of parts for a range of websites. Neil asked a follow up to Roman about the example of synchronous detection. Neil's solution is a scale down of a lock-in amplifier which is $1000s. The LED sends light out. The detector measures ambient light and the emitted light from the LED which is bounced off a finger. In the code, Neil measures the difference of the wave signal when the light is on versus when it is off. The smoothing filter is calculated by _=(1 - E)*filteredReading + E*newReading_. Discussing his input devices project, Roman mentioned using assembly for the code. Neil advocated for the use of C, due to Roman's concern about speed. GCC-AVR, according to Neil, is a very good compiler and C has many single cycle hardware instructions that alleviate the concern of processing speed (with the caveat of dealing with data types that aren't primitive or multi-byte numbers).

#### Class Notes 2017