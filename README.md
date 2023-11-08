# Deere-8x00-WAS

A wheel angle sensor (WAS) assembly using the Delphi ER100XX sensor for John Deere 8x00 tractors. Intended for use with  [AgOpenGPS](https://github.com/farmerbriantee/AgOpenGPS "github.com/farmerbriantee/AgOpenGPS"), but the 0-5v sensor may be used with some other autosteer systems also. The assembly includes a fabricated plate part, 3d printed parts, and some small hardware parts. I am using this assembly on an 8100 and an 8300, one set to 60" spacing and one set to 90" spacing (different steering stops). The assembly may also work on other tractors with the 1300 series front axle.

<img src="https://github.com/WildBuckwheat/Deere-8x00-WAS/blob/main/Images/Assembled1.JPG" width="820">
<img src="https://github.com/WildBuckwheat/Deere-8x00-WAS/blob/main/Images/Assembled2.JPG" width="820">
<img src="https://github.com/WildBuckwheat/Deere-8x00-WAS/blob/main/Images/Assembled3.JPG" width="820">
<img src="https://github.com/WildBuckwheat/Deere-8x00-WAS/blob/main/Images/AssembledLeftLock.JPG" width="820">
<img src="https://github.com/WildBuckwheat/Deere-8x00-WAS/blob/main/Images/AssembledRightLock.JPG" width="820">



# Design goals
My goals in designing this WAS assembly
- Work with or without fenders
- Have as close to 1:1 ratio with kingpin rotation as possible
- Require no heavy machining or major modifications to axle
- Shield the sensor from operators climbing the axle, for example to check radiator
- Shield the sensor from stalks and mud
- Be able to be mounted on the left or right side

I believe I was able to meet these design goals with exception of the left/right side mounting. The sensor arm included will work on the right side only. To make the sensor arm work on the left side the sensor screw holes will need to be modified (rotated). All the other parts are ambidextrous and will work on either the left or right side. Mounting on the right side will allow the sensor's internal spring to keep the linkages in tension which is arguably slightly better than keeping the linkages in compression.



# BOM
These are the parts required. Some of the parts are expanded on below.
- Knuckle Plate
- 5/16" x 1-1/2" bolt, nut, and washers. Or M8x40mm bolt, nut, washers 
- M3x32mm SHCS, M3x12mm SHCS, M3 brass insert or M3 nut. Or 4-40 x 1-1/4" screw, 4-40 x 1/2" screw, 4-40 nut.
- Tie sensor rod. See below for parts breakdown
- 3d printed DelphiSensorArm
- 3d printed TopSensorMount
- 3d printed Standoff
- Delphi ER100XX sensor
- 6-1/2" x 1/2" wide hose clamp. Stainless recommend,


# Knuckle Plate
The knuckle plate mounts under the fender bracket using the existing M12x35 fender bracket bolts. The plate features a clearance hole for the kingpin grease nipple and several holes for mounting the sensor tie rod. One of the middle holes should work, but there are other holes in case you need them.

I had my plates plasma cut by a local fab shop from 1/4" steel plate. You can use the .dxf file to have your own plates plasma cut or laser cut. Alternatively, you can print the .pdf files at a 1:1 scale and use them as a paper template to fabricate a plate with hand tools. The template will not fit on one sheet of letter size paper. Double check the dimensions once printed to ensure that the printing is at 1:1 scale.

You will require a plate approx 8.5" x 11" (215 mm x 280 mm). I recommend at least 1/8" thickness steel but the thickness and material are not crucial. Consider that someone may step on the edge of the plate to access the radiator cap or to clean a window.

<img src="https://github.com/WildBuckwheat/Deere-8x00-WAS/blob/main/Images/KnucklePlates.JPG" width="820">
<img src="https://github.com/WildBuckwheat/Deere-8x00-WAS/blob/main/Images/KnucklePlateTestFit1.JPG" width="820">
<img src="https://github.com/WildBuckwheat/Deere-8x00-WAS/blob/main/Images/KnucklePlateTestFit2.JPG" width="820">



# Delphi ER100XX Sensor
The Delphi ER100XX sensor is a spring loaded ride height sensor used by many different GM vehicles. The sensor typically comes with a stamped steel mounting bracket, stamped steel sensor arm, and a small linkage. There are many different part numbers to reflect these different bracket assemblies, but they all use the same sensor and screws. All that is used for this WAS assembly are the sensor and screws, the brackets are discarded. The least expensive option that I was able to find is the ER10031 front right (passenger side) ride height level sensor for Chevrolet Corvette 2005-2013 and Cadillac XLR 2004-2009. Reference numbers 89047643, 926-789, 926789.

The plug for this sensor is a 3 pin Aptiv Metripack 150. You may find a pigtail at your local auto parts suppliers or online by searching for GM 12085538, GM 88862227, ACDelco PT148, ACDelco PT2308, Car-Pak, 96-7571, Pico 5606PT, SMP S577, or by searching for a GM Camshaft sensor pigtail.

<img src="https://github.com/WildBuckwheat/Deere-8x00-WAS/blob/main/Images/DelphiAmazon.JPG" width="820">
<img src="https://github.com/WildBuckwheat/Deere-8x00-WAS/blob/main/Images/DelphiSensor.JPG" width="820">
<img src="https://github.com/WildBuckwheat/Deere-8x00-WAS/blob/main/Images/DelphiSensorDisassembled.JPG" width="820">
<img src="https://github.com/WildBuckwheat/Deere-8x00-WAS/blob/main/Images/DelphiDimensions.JPG" width="820">
<img src="https://github.com/WildBuckwheat/Deere-8x00-WAS/blob/main/Images/DelphiPigtailGM12085538.JPG" width="820">
<img src="https://github.com/WildBuckwheat/Deere-8x00-WAS/blob/main/Images/DelphiPlug.JPG" width="820">



# 3d printed parts
3d print the parts out of an appropriate plastic like PETG or ABS. I would not use PLA because I do not believe it will hold up to hot summer days. Use at least 4 perimeters and a heavy infill. I recommend printing spares, but with a few hundred hours of operation I have not required a spare yet. Print the parts in the orientation shown. The SensorArm requires support. The Standoff and TopSensorMount do not require supports.

The SensorArm is sized for a brass M3 insert to be inserted with a soldering iron, but you can use a longer screw and nut instead.

The TopSensorMount attaches to the axle with a hose clamp. The bottom part of the TopSensorMount fits tightly into the axle recess and the 3/8" square of the axle retaining screw.

<img src="https://github.com/WildBuckwheat/Deere-8x00-WAS/blob/main/Images/3dPrintedPartsAssembled.JPG" width="820">
<img src="https://github.com/WildBuckwheat/Deere-8x00-WAS/blob/main/Images/3dPrintOrientation.JPG" width="820">
<img src="https://github.com/WildBuckwheat/Deere-8x00-WAS/blob/main/Images/AxleRetainingScrewHole.JPG" width="820">



# Sensor Tie Rod
I made my Sensor tie rod using Traxxas 5347 Rod Ends. These are rod ends for an RC car that you should be able to buy on Amazon or your local RC hobby store. The holes in the balls work with M3 or 4-40 screws. The plastic ends tap well with 8-32 or M4.

I made my rod from 113.25mm of 1/4" aluminum rod. I drilled and tapped the ends of the aluminum rod to 8-32 thread, then used small sections of 8-32 threaded rod to attach the rod ends.

If you are using the Traxxas rod ends then you could also use 8-32 threaded rod sleeved with 1/4" x 0.049 wall aluminum tubing. The sleeving is optional but looks nice. M4 threaded rod could also be used.

The important thing about this sensor tie rod is that it measures 145.5 mm center to center. You can fabricate something different with available materials. The Delphi sensor has a spring that wil take up any slack in your assembly.



# Linkage bolt
I used a 5/16 x 1-1/2" bolt. I drilled and tapped the end of the bolt to M3. You could also use an M8x40mm bolt. You could tap to 4-40 instead of M3. 



# Axle Retaining Screw
Here is the torque spec for the axle retaining screws in case you require them. Do not overtighten the screws or the inner sleeve may be damaged. I recommend that you leave the screws alone.

<img src="https://github.com/WildBuckwheat/Deere-8x00-WAS/blob/main/Images/AxleRetainingScrewTorque.JPG" width="820">
<img src="https://github.com/WildBuckwheat/Deere-8x00-WAS/blob/main/Images/AxleRetainingScrewCrossSectional.JPG" width="820">