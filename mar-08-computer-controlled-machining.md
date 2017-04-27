# Computer-Controlled Machining {#computer-controlled-machining}

#### Have you:

* [ ] Explained how you made your files for machining \(2D or 3D\)

* [ ] Shown how you made something BIG \(setting up the machine, using fixings, testing joints, adjusting feeds and speeds, depth of cut etc\)

* [ ] Described problems and how you fixed them

* [ ] Included your design files and ‘hero shot’ photos of final object

![](/assets/cnc-fab-lab.gif)

**This week's "Invention Exchange"**

Oh. My God. It's like I've always thought. [Mystery Science Theater 3000](http://splitsider.com/2017/03/building-on-sacred-ground-with-the-new-cast-of-mst3k/) is a parody of my work at The Fab Foundation!

**Visiting MIT's Center for Bits and Atoms**

There's a tutorial for this assignment on The Center for Bits and Atoms site, [here](http://fab.cba.mit.edu/content/tools/shopbot/index.html). I didn't know that in 2015. So, what ended up happening is that I went to the CBA shop and bothered the "Spiciest Meme Lord" Tom Lutz.

![](/assets/IMG_3858.JPG)
_They're not playing around in the CBA Shop. Oh yeah, cause you can lose limbs or die..._

He walked me through the process of using Partworks, setting up the ShopBot, and not losing eyes or fingers in the process. With those surviving eyes and fingers, I took copious notes.

![](/assets/SHOPBOT NOTES FROM CBA.jpg)
_#Copious_

With Tom's assistance, I was able to design and cut out a monogram plaque which I keep by my work desk to this day.

[![April 7, 2015 ](https://img.youtube.com/vi/MdH7EsKkzcI/0.jpg)](https://www.youtube.com/watch?v=MdH7EsKkzcI "April 7, 2015 ")

[![April 7, 2015 ](https://img.youtube.com/vi/ysspIwxeKBs/0.jpg)](https://www.youtube.com/watch?v=ysspIwxeKBs "April 7, 2015 ")

**Trouble at The Southend Technology Center**

After taking that nice lesson, I returned to the South End Technology Center to wrestle with the first ShopBot ever purchased for a Fab Lab. What a bear that thing was. First off, the control box looked like a hollowed out desktop tower with an emergency stop.

![](/assets/IMG_3908.JPG)
_What the Hell is this??_

It took a visit from Bill Young and an email to Ed Baafi to figure out what the mystery of the setup was. According to Ed, the big e-stop on the PC case is a hardware e-stop which cuts power. The big e-stop on the spindle controller is a software e-stop that stops a running program.

Bill Young's visit gave us a little history on the "first ShopBot ever purchased for a Fab Lab":
* We did not know when was the last time the pinion gears were changed, if ever
* Dianne Reynolds from ShopBot found the specs on the tool. It's a PRSstandard96-48-6 4/2007 with a 4hp 1 phase spindle (This is actually important to remember when loading the settings file in the ShopBot software)
* We also needed a surfacing bit for leveling the sacrificial board and stock.
* The spindle control that had the software e-stop is a V7-4X VFD. We wanted to replace that, but another visit from Ryan Patterson resolved any bugs by updating the firmware

**Steps for Machining**

Ale Diaz de Leon has a nice summary of work flow on her page that I will adapt and integrate with the tutorials and CBA lesson:

* Prepare the file on the ShopBot software. The result is three layers:
   * Holes for fixturing the stock
   * Inside pieces
   * Outlines with tabs with tabs to keep pieces attached to the board while it's cutting
   
![](/assets/IMG_3860.JPG)
_An example of setting up the file from Tom's walk through_

* Put the stock on the sacrificial board on the machine. The surface should be clean and smooth

![](/assets/IMG_3863.JPG)
_Stock is fixtured on four corners, instead of points set in software_

* Find the home points for X, Y, Z
* _#EmmasTips_ Emma Pareschi, (If the machine stops) the XYZ calibration should still be the same so always check if the machine kept it.

![](/assets/IMG_3862.JPG)
_Homing the spindle from the ShopBot software_

* Send the file from the ShopBot software to find the holes
* Drill the screws on the stock to fixture. That way, the stock will not move during the machining
* Send the file and wait for it to finish cutting.
* _#EmmasTips_, if during the milling job the machine stops (it can happen for several reason like electric drop or comunication problems with the computer) it's important to take note of the line where the job ended. Then you can start the same job with the option: "start from the line" from the File menu. I suggest to move the bit close to the working area and start the job from two lines before the one you wrote down. For istance if the line stopped at line 200, I would start the new job from line 198.

[![April 7, 2015 ](https://img.youtube.com/vi/RaRJE4wzvX0/0.jpg)](https://www.youtube.com/watch?v=RaRJE4wzvX0 "April 7, 2015 ")
_ShopBot file running and sending tool paths to the machine_

* Remove the tabs using a chisel and a hammer.
* Remove the pieces and the excess stock

**Tooling**

The week of DigiFabCon 2017, I met Ted Hall at Center for Bits and Atoms. His first words to me were, "Oh, so you're Jean-Luc. I heard everything about you." Followed up by, "I hear you've been spending a lot of time with my wife." Bill Young chuckled, "Well, that's one way to start a conversation." Sallye Coyle is a good friend and a great teacher. We've been on two Fab Lab installs together and two FABx meetings.

Before I met Sallye, I would create Fab Lab pro forma based solely on the Fab Lab Inventory curated by MIT. The what's and why's were normally answered by, "this is what MIT recommends" or "this is what is needed to take Fab Academy." That said, I don't think we ever got around to explaining 5 gallons of machine oil or the $84 USD 1/2" two flute downcut end mill. I received a spreadsheet on tooling from Sallye that was very helpful in explaining what was the right tool for specific, common applications in a Fab Lab: [Right Click + Save](/uploads/bit-inventory.csv)

**Materials**


**Designing files for Machining**


**Building up a ShopBot**

![](/assets/IMG_0783.JPG)

![](/assets/IMG_0795.JPG)

**Sources**

Baafi, Ed "A couple of quick questions on the ShopBot at SETC" Message to Jean-Luc Pierite. 30 April 2015. E-mail.

Coyle, Sallye "Bit inventory for Bakersfield" Message to Jean-Luc Pierite. 20 July 2016. E-mail.

Diaz De Leon Lastras, A. \(n.d.\). Computer-Controlled Machining. Retrieved April 19, 2017, from [http://fabacademy.org/archives/2014/students/diazdeleon.alejandra/8.Computer-ControlledM.html](http://fabacademy.org/archives/2014/students/diazdeleon.alejandra/8.Computer-ControlledM.html)

Pareschi, E. (n.d.). Emma's note. Retrieved April 19, 2017, from http://fabacademy.org/archives/2014/students/pareschi.emma/classes_wk7.html

Young, Bill "a couple of things for the SETC ShopBot" Message to Jean-Luc Pierite. 20 April 2015. E-mail.

