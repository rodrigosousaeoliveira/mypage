---
layout: post
title: 'CNC ROUTER: 1000mm x 1500mm Aluminium Frame'
description: 'Probably the coolest project yet'

---
<img alt="Cutting my Prusa I3 frame" src="/mypage/assets/images/cnc/cnc1.jpg" >

I was an intern at Metrum Equipamentos de Medição e Testes Ltda for 15 months and the biggest project I developed there (and the one I am the most proud of) was this beautiful CNC Router. I had great guidance from Kayran, a brilliant guy who unfortunately passed away during the project. 

## Mechanical Design

I made the entire CAD assembly using Autodesk Inventor, which looked a lot like Solidworks. The router uses aluminium extrusions (30 x 60 and 30 x 30) and 1/4 inch thick aluminium plates for structure, which makes it really stiff. For the movement, the NEMA23 motors are attached to 12mm trapezoidal screws. We would prefer to use ballscrews, but the prices were really a barrier and in the end the trapezoidal ones ended up doing the job pretty well.

## The brains

The brain of the machine is an [Arduino Nano](https://www.arduino.cc/), believe it or not. Assembly was mostly connecting the drivers and endstops to their correct pins on the Arduino, but in that process I got to route my first PCB, which is harder than it seems! The VFD that controlled the Spindle used a 10 - 0 V signal to determine the motor speed (3000 - 18000rpm) so we ended up using an RC filter to turn the PWM signal coming from the Arduino into an usable analog signal. 

The firmware we used is called [GRBL](https://github.com/grbl/grbl) and it is the "father" of the [Marlin](https://github.com/MarlinFirmware/Marlin) firmware, which runs on many of the modern 3D printers. It is really well documented and, for a standard assembly such as this one, not many modifications are necessary. It is really versatile and people have done all kinds of crazy things with it, I plan on making a laser engraver with it in the future.

## Operation

When I finished assembling the machine, I started testing it. At first, doing some homing sequences to check if the endstops were plugged in ok and the usual drawings with a pen instead of an 18000rpm cutting tool. After some drawings I slowly tried some other materials. Most of the times it would be used for MDF parts, but I also had to mill some aluminium parts. Aluminium is tricky: it needs cooling and a lot of tuning. I believe there can be some problems with resonance also and breaking bits is not uncommon during the tuning part, but getting to the right settings is a matter of time and patience. To level the bed, we would use a facing bit and check alignment with a dial indicator every once in a while, as well as lubricating the linear rails with oil and the screws with lithium grease.

### If you are interested in making a CNC router, there are lots and lots of information online. Youtube has some great tips and opensource software is everywhere. It is a great learning experience and in the end you get a very useful and precise machine.

Here a short video I made while cutting a Prusa I3 frame out of MDF:

[<img alt="Video" src="/mypage/assets/images/cnc/cnc2.JPG">](https://drive.google.com/file/d/17NHyL_Y4tJYJK0ooy7x6y6hQLPyWXaQm/view?usp=sharing)
