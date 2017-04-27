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

He walked me through the process of using Partworks, setting up the ShopBot, and not losing eyes or fingers in the process. With those surviving eyes and fingers, I took copious notes.

![](/assets/SHOPBOT NOTES FROM CBA.jpg)

With Tom's assistance, I was able to design and cut out a monogram plaque which I keep by my work desk to this day.

[![April 7, 2015 ](https://img.youtube.com/vi/MdH7EsKkzcI/0.jpg)](https://www.youtube.com/watch?v=MdH7EsKkzcI "April 7, 2015 ")

[![April 7, 2015 ](https://img.youtube.com/vi/ysspIwxeKBs/0.jpg)](https://www.youtube.com/watch?v=ysspIwxeKBs "April 7, 2015 ")



**Trouble at The Southend Technology Center**

After taking that nice lesson, I returned to the South End Technology Center to wrestle with the first ShopBot ever purchased for a Fab Lab. What a bear that thing was. First off, the control box looked like a hollowed out desktop tower with an emergency stop.

![](/assets/IMG_3908.JPG)

It took a visit from Bill Young and an email to Ed Baafi to figure out what the mystery of the setup was. According to Ed, the big e-stop on the PC case is a hardware e-stop which cuts power. The big e-stop on the spindle controller is a software e-stop that stops a running program.

Bill Young's visit gave us a little history on the "first ShopBot ever purchased for a Fab Lab":
1. We did not know when was the last time the pinion gears were changed, if ever
2. Our sales representative, Dianne found the specs on the tool. It's a PRSstandard96-48-6 4/2007 with a 4hp 1 phase spindle (This is actually important to remember when loading the settings file in the ShopBot software)
3. We also needed a surfacing bit for leveling the sacrificial board and stock.
4. The spindle control that had the software e-stop is a V7-4X VFD. We wanted to replace that, but another visit from Ryan Patterson resolved any bugs by updating the firmware

**Steps for Machining**

Ale Diaz de Leon has a nice summary of work flow on her page that I will adapt and integrate with the tutorials and CBA lesson:

1. Prepare the file on the ShopBot software. The result is three layers:
   1. Holes for fixturing the stock
   2. Inside pieces
   3. Outlines with tabs with tabs to keep pieces attached to the board while it's cutting
   
![](/assets/IMG_3860.JPG)
_An example of setting up the file from Tom's walk through_

2. Put the stock on the sacrificial board on the machine. The surface should be clean and smooth

![](/assets/IMG_3863.JPG)
_Stock is fixtured on four corners, instead of points set in software_

3. Find the home points for X, Y, Z

![](/assets/IMG_3862.JPG)
_Homing the spindle from the ShopBot software_

4. Send the file from the ShopBot software to find the holes
5. Drill the screws on the stock to fixture. That way, the stock will not move during the machining
6. Send the file and wait for it to finish cutting.

[![April 7, 2015 ](https://img.youtube.com/vi/RaRJE4wzvX0/0.jpg)](https://www.youtube.com/watch?v=RaRJE4wzvX0 "April 7, 2015 ")
_ShopBot file running and sending tool paths to the machine_

7. Remove the tabs using a chisel and a hammer.
8. Remove the pieces and the excess stock

**Sources**

Baafi, Ed "A couple of quick questions on the ShopBot at SETC" Message to Jean-Luc Pierite. 30 April 2015. E-mail.

Diaz De Leon Lastras, A. \(n.d.\). Computer-Controlled Machining. Retrieved April 19, 2017, from [http://fabacademy.org/archives/2014/students/diazdeleon.alejandra/8.Computer-ControlledM.html](http://fabacademy.org/archives/2014/students/diazdeleon.alejandra/8.Computer-ControlledM.html)

Young, Bill "a couple of things for the SETC ShopBot" Message to Jean-Luc Pierite. 20 April 2015. E-mail.







![](/assets/IMG_0783.JPG)

![](/assets/IMG_0795.JPG)

