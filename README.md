# Gaui X3L Speed
 
 <img src="https://github.com/AlCormack/GauiX3L/blob/master/images/x3l.jpeg" width="800"><br />
 
A little video of it during a speed pass:
 [![IMAGE ALT TEXT](http://img.youtube.com/vi/dyuTX_kXLzM/0.jpg)](http://www.youtube.com/watch?v=dyuTX_kXLzM "Gaui Speed X3L")
 
After getting my Gaui R5, I got the bug for speed. The R5 is a fantastic heli but I was looking for something even smaller for quick trips to the field. As it obviously had to be a Gaui heli the choice was simplified as the X3L had a fuselage and would support a motor that was much larger than a 325-380mm heli would normally use. The next decision was two or three blades. Never had a three blade heli and have fancied one but also liked the idea of greater stability on a small size heli. So got the: 

* Gaui X3L Basic Kit 3 blade - X3L Basic Kit

The tail is never highly loaded on a speed heli and the 3 blade tail setup would just cause more drag therefore reduce the max speed. So ordered the required 2 blade tail parts:

* X3 Tail Pitch Slider Set
* X3 Tail Rotor Grip Assembly

For servos I wanted to run a high voltage setup. As I was in Taiwan the little Align servos looked good and had nice red fins to match the body colour (had to find some reason to justify them here):

* Align DS455M servo
* Align DS450M servo

For the motor there was only one choice. The monster Scorpion HK-3226, and to support the top of the motor shaft I added the: 

* Engine second bearing mount(for X3L)   

<img src="https://github.com/AlCormack/GauiX3L/blob/master/images/side.jpeg" width="800">

Also to support the blades I added the:

* X3 Main Blade Grips Parts Upgrade Pack (for 3 Blade)

For esc I tried the Hobbywing 50 but the telemetry setup is not great on it as it required a j-log to get the info I needed on PWM, and head speed. It also did not have a current sensor, so a MUI50 was needed too. A lot of extra electronics to fit in a small heli! YGE came out with their telemetry line. So I took out the Hobbywing (it has now gone in a standard X3 since) and put in a Yge 65lvt esc. This outputs directly to the Jeti RX and has a current sensor built in. Really nice esc, that also has an anti-spark setup. I use 5mm bullets as there is not much space for connector choice and this allows the positive to go one side and the negative the other of the frame. Since its launch Scorpion has now added an 80amp Tribunus, and I have had great success with the 200amp version on my R5 (destroyed 2 other brand esc's previously). If this was out at the time, I would have picked this as I am a huge fan of Georges, Tony and Scorpion as a whole, for all the fantastic support they provide in this hobby.

For main blades I have tried the Rail 326's but they did not max out the esc/motor even with a high pitch setup. I then tried the RotorTech 360mm 3 blade's. They were ok but I got a couple of very bad pitch ups and the heli was not stable at high speed. I then ordered two pairs of 363mm XBlades and used three of them. They turned out to really nice at high velocity, high RPM(3650) and high pitch angles (15 deg). For the tail blades I am using the Switch 60mm blades.

To get the head speed I wanted I needed a 14 tooth pinion, with a 5mm hole. Turned out this was not easy to find. Lynx had some end-of-line ones still in stock but they had the smaller 3mm hole. So ordered a bunch of them and got some 5mm drills and got my dad to use his lathe to drill out the centre. 

Getting the pitch of all three blades was not simple so ended up making my own turnbuckles. So ordered up some 3mmx25 titanium turnbuckles from a RC Car supplier. Drilled and Tapped Gaui ball ends to cope with 3mm thread (left and right threads). I use the Soko heli tool to get the setup all spot on (with the phone app to hand-hold me through all the setup steps. 

<img src="https://github.com/AlCormack/GauiX3L/blob/master/images/Turnbuckle.jpg" width="256">

Given the very high loads on the main gears I use Dryfluid Gear on both the gears and thrusts.

For flight packs I started with my favourite OptiPowers but getting stock of them is really tricky. I took a shot at the new Turnigy Graphenes:

* TURNIGY GRAPHENE 1500MAH 6S 65C LIPO

Amazingly they are incredible during a speed flight. Really shocked. The telemetry shows they keep their voltage even under huge load. One issue is that they are heavy but given how much power I have.. its not such a big deal.

For the flybarless the choice was simple: 
* BavarianDEMON 3SX with a Jeti Rex3 rx ([setup file](https://github.com/AlCormack/GauiX3L/blob/master/BD3SX/20190209%20Gaui%20X3L.hcx)) 

To measure the average speed I added my [speed GPS](https://github.com/AlCormack/SpeedGPS) and I use the [MHSFA speed application](https://github.com/AlCormack/JetiLua/tree/master/MHSFAApp) for the Jeti.

Given the high amp loads I have always had a worry about loosing power to the rx. So for safety I added a:
* R2 3x25 buffer.

The only problem that I have had so far is the radius arm breaking (on the three blade there is only one, unlike the two on the two blade). This had done over 100 flights. So now I am changing it every 50 flights (and the belt every 100)
<img src="https://github.com/AlCormack/GauiX3L/blob/master/images/BrokenLink.jpg" width="256">

Now for some further slight optimisation. The tail was something that needed a bit of work. The gain I had to run to keep it all straight was more in the realms of a 3D setup (49 on the 3SX). Whereas on my R5 it was about 10 points less. The proper speed fuse helps on the R5 but also on my V1 the tail is adjustable, so like the big 700 speed machines you can build in some angle of attack on the rear fin. So out came the CAD software (Fusion 360 for me) and the 3D printer. I made a custom tail setup that has adjustable wedges to build in some tail wing angle. I have ended up using a 10degree wedge setup and have:
* lost about 10 points in the tail gain
* gained sever kph in average pass speed
* gone to a smaller tail blade length

The final setup is pieced together as follows:<br />
<img src="https://github.com/AlCormack/GauiX3L/blob/master/images/AngleOfAttack.jpeg" width="512"><br />

I have provided a jig to enable to holes to be drilled in the correct locations (use double sided tape to hold the carbon sheet on while drilling). The jig also forms a good template for the adaptor to be cut out of 1mm carbon fibre sheet:<br />
<img src="https://github.com/AlCormack/GauiX3L/blob/master/images/Jig.jpeg" width="512"><br />
The adaptor is mounted as follows:<br />
<img src="https://github.com/AlCormack/GauiX3L/blob/master/images/Adaptor.jpeg" width="512"><br />


I have added all the files for this in this GitHub project for all of you to use. This includes [a pdf file](https://github.com/AlCormack/GauiX3L/blob/master/Fin%20Drawing%20v1.pdf) for the fin to be cut out of 1mm carbon fibre sheet. You can print this onto paper and cut it out to form a template or if you have a vinyl cutter I have added the [silhouette studio file](https://github.com/AlCormack/GauiX3L/blob/master/fin.studio3)  too.

<img src="https://github.com/AlCormack/GauiX3L/blob/master/images/3DParts.jpeg" width="256">

<img src="https://github.com/AlCormack/GauiX3L/blob/master/images/Finished.jpeg" width="512">
 
