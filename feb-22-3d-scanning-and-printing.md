# 3D Scanning and Printing

Last year, I spent Halloween dressed as Bernie Sanders while I 3D printed toys and treats for kids. I got a good workflow going from designing pixel art in GIMP, to converting the designs in vector in Inkscape, and then extruding the models in blender. There was just one problem: the models that I was printing were subtractive and not additive.

I found that the difference between additive vs. subtractive processes were difficult to articulate in design. The actual part from the Halloween activity was additive by how the model was rendered in Makerware or Cura. The part is hollow, aside from a honeycomb interior supported by external walls. That said, a subtractive method such as machining wax on the mini-mill could achieve the same external shape.

So, I thought about it for a year…

One day, I decided to search for additive design which led me to Danish architect Jørn Utzon and his work on “Additive Architecture.” Utzon observed the “growth principle in nature” which inspired a belief that buildings should be organized freely. Instead of starting with a box and subdividing the interior with partition walls, an additive method starts with components that could range in variety yet assembles them in such a way to achieve harmony.

Those were some pretty thoughts, but I didn’t have an “Aha!” moment until I saw a video in my Facebook feed…

A red ball rolled down the streets of Toledo, Ohio. It was part of an exhibit for the Toledo Museum of Art. Wind and rain from a storm freed the giant 15-foot wide ball and sent it fleeing museum staff members that hoped to capture and return it.

Seeing this ball reminded me of Katamari Damacy, a video game about rolling balls along any scale of surface. You start small by rolling pencils, pins, and mice; ultimately the ball becomes so large that you can roll up: cows, whales and Godzilla. The clump of animals, vehicles, and buildings is then judged by the King of the Cosmos. He decides whether the product is big and impressive enough to become a star. Seems like the perfect metaphor for Fab Academy.

And so I set out to make a Katamari wrapped in a paperclip chain…

NOT SO FAST: you forgot to wrestle with machines and troubleshoot

Ah yes, my first set up of an Ultimaker 2 came from Fab Lab Roxbury @ The Impact Studio. We had two printers from FAB11 which were donated to local labs after the conference. The printers were packed and stored until they were ready for delivery. One of the printers still had filament loaded while it was packed and stored. What happened in that situation is that the PLA became brittle inside the Bowden Tube. It was difficult to extract the material without snapping inside the curved tube. I managed to push the trapped material through the tube with material that was still on the spool. I was still very careful not to break the spool material as both pieces were subject to the elements while in storage.

##### PLA Problems

At FAB@CIC, we experienced similar problems with the PLA filament. Indoors, during the Summer in Boston, we ran the central air conditioning to cool rooms and larger spaces. Most of our filament was stored under workstations for 3D printers and became brittle at a time when we were printing prosthetic hands for the eNable Hand-a-thon. We solved the problem by buying an indoor humidifier.

PLA presents a problem for deployment and storage. It’s not due to regulations. Rather, we have to carefully balance the nature of the material with the environmental challenges of prospective or existing Fab Labs. A lack of humidity causes the material to dry and break up. Too much humidity and the material could expand in the Bowden Tube and lead to clogs. Sending filament to India, for example, we have to consider the heat and humidity. We decided to ship and store filament in air tight buckets with silica inserts.

When a clog happens in the print head, there is a method of unclogging known as the “Atomic Pull.” On the Ultimaker 2, we heated up the nozzle to 220 C. A piece of filament long enough to protrude out of the print head was inserted and left to melt for ten seconds. Once melted, we lowered the temperature of the nozzle to 90 C. This allows for the material to cool and mold into the shape of the nozzle. A good firm tug resulted in the tip of the filament to come out in the shape of the nozzle. We were then able to see through the nozzle to the build plate below which indicated that the clog was removed.

Of course, I could just source PLA from New Zealand. I hear Diamond Age Solutions is pretty good…

##### Leveling with the Ultimaker

The goal of FDM \(Fused Deposition Modeling\) is to allow molten material to be extruded and consistently laid onto the build plate. Ultimaker provides some good visuals as to what is and what isn’t a good first layer. What I noticed from my first few attempts at printing was that material just barely made an impression on the build plate. It took some layers for the part to show up at all. This was due to our build plate being too close to the nozzle. Ultimaker does have on-screen instructions to help with leveling. Still, when you live in a country in which people live and die without knowing the metric system; you can easily mess up a process that starts with “make sure the nozzle is 1 mm away from the build plate.” The best way to eyeball the process that I found was to think of the materials diameter which then gets extruded through the diameter of the nozzle.

##### Going Straight to the Ulti-Source

I spent time with Luis Rodriguez of Ultimaker to go through basic warranty and service training for their line of printers. We went over tips and tricks for proper maintenance of the printers as well as workflow within Cura to send jobs to the printers.

The current model, Ultimaker 2+, has several revisions to the Ultimaker 2. An upgrade kit is available for those with the previous model. The U2+ has a geared feeder, a swappable nozzle, and optimized airflow. This allows for improved freedom of choice for materials in terms of diameter. The first tip was to wipe and keep surface clean and free from dust. In terms of fixturing, Luis and his team have seen users spray hairspray onto the build plate which works. The problem comes about when the user sprays the build plate inside the printer and the spray goes on to rails and pulleys. There is grease packed in with the printer. This is only intended for the Z-axis threaded rod. For the X and Y axis, Luis suggested machine oil. A brass brush was best for keeping the nozzle clean. Nylon was the suggested material for the Atomic Pull method. Luis also suggested clipping the end of the filament at an angle before inserting in the feeder. It’s similar to trimming a threading before pushing through a needle’s eye.

As far as workflow in Cura, once a model is loaded the steps are to select the nozzle and the material. Layer view can simulate how the part will print. Luis also demonstrated taking individual models and doing modification per model in Cura. Then, the multiple models can be merged into one and a single gcode can be exported from Cura.

I also learned about another type of filament known as PVA. This is a water-soluble material that can provide support for FDM additive structures. In the future with an improved FDM dual extrusion process, more complex parts can be printed with a combination of build and support material. With PVA, the parts can be weeded out with a bath that will dissolve the support material and leave the model. This would improve my results of printing a clump of paper clips that surround a sphere.

##### Scanning the Columbus Lion

Last year while taking Fab Academy at the South End Technology Center, I spotted a cool lion statue two blocks down Columbus Avenue. I wanted to capture it using 123D Catch on my iPhone.

With the app, I took a series of pictures around the subject which are assigned different angles. The app uses the device’s accelerometer to sense the different angles.

I tried a couple times to capture the lion. As a free app, there’s not much support and the model can take several hours to process once loaded to Autodesk’s service. In order to completely scan the statue, I would have to take more pictures from consistent distances and angles.

