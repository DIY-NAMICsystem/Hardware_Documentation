# Final Assembly

#### What you will learn:

How to build and assemble the box with the finished components.
___

### Introduction

With the modified cage, OM1 shield, and soldered components to the wires, they can now be assembled. 

### Materials

<p align="center">
    <img title = "figure1" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_9.Final_Assembly/imgs/Figure_1.png?raw=true" align=center width=450/><br><br>
    <b><i>Figure 1</b></i>
</p>

#### Components:


Components | Arduino | Others
------|:-------:| -----
LEDs (attached to noseport) | Arduino | Cage + Plexiglass
IR photo interrupters | OM1 Shield| Manifold + Syringe  
Solenoids + Tubing | Type A/B USB Cable | Screwdriver
 | Power Adapter | Screws (Phillips 4-40 x 5/16")

 ### 1) Assemble customized nose ports to Plexiglass

 <p align="center">
     <img title = "figure2" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_9.Final_Assembly/imgs/Figure_2.png?raw=true" align=center width=350/><br><br>
     <b><i>Figure 2:</b> Materials Needed for noseport - plexiglass assembly</i>
 </p>

 Once the nose ports have the components attached, they can be screwed to the plexiglass. The ront-plate should look something like this:

 <p align="center">
     <img title = "figure3" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_9.Final_Assembly/imgs/Figure_3.png?raw=true" align=center width=350/><br><br>
     <b><i>Figure 3:</b> Front view of plexiglass (mice will face this side) </i>
 </p>

 <p align="center">
     <img title = "figure4" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_9.Final_Assembly/imgs/Figure_4.png?raw=true" align=center width=350/><br><br>
     <b><i>Figure 4:</b> Back view of plexiglass (we will face this side) </i>
 </p>

 Remember that the rodents will be facing the flush side of the plexiglass. The wires will be on the back side, since we don’t want mice interacting and possibly chewing up all the wires.

 ### 2) Slide in the IRs into the nose port

 <p align="center">
     <img title = "figure5" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_9.Final_Assembly/imgs/Figure_5.png?raw=true" align=center width=350/><br><br>
     <b><i>Figure 5:</b> Make sure that the IR LEDs go into the right (blue circle) and the phototransistor goes into the left (red circle) </i>
 </p>

 Both parts of the IR (LED and phototransistor) will fit snugly into the nose port. However, make sure that the IR LED goes into the right (blue circle – 2 wires) and that the phototransistor goes into the left (red circle – 3 wires). This will help with wiring later when we connect them to the shield.

 ### 3)	Assemble the solenoids with the manifold and the syringe

 <p align="center">
     <img title = "figure6" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_9.Final_Assembly/imgs/Figure_6.png?raw=true" align=center width=350/><br><br>
     <b><i>Figure 6:</b> Picture of solenoids, manifold, and syringe after final assembly </i>
 </p>

 The solenoid valves assembled with the tubing are attached to the manifold, and the manifold is attached to the syringe with the larger tubing. See [Bill of Materials](https://github.com/jhl0204/AIM-Hardware-Documentations/wiki/Bill-of-Materials))

Also note that the solenoids valves don’t have the wires soldered on. Original female – male wires can be used for the solenoids since the solenoid valve leads are thick and the female encasings stay on. 

### 4) Screw in the manifold encasing

<p align="center">
    <img title = "figure7" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_9.Final_Assembly/imgs/Figure_7_1.png?raw=true" align=center width=350/><br><br>
    <b><i>Figure 7:</b> Screwing in the manifold encasing (white rectangular box) </i>
</p>

<p align="center">
    <img title = "figure8" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_9.Final_Assembly/imgs/Figure_8.png?raw=true" align=center width=350/><br><br>
    <b><i>Figure 8: </b> After set-up. Notice the manifold on top of the manifold encasing </i>
</p>

Screw in the manifold encasing into the plexiglass. 

<p align="center">
    <img title = "figure9" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_9.Final_Assembly/imgs/Figure_9.png?raw=true" align=center width=350/><br><br>
    <b><i>Figure 9: </b> Note that the solenoid valves are fitted with normal female wires (red circle). </i>
</p>

### 5) Wiring to the OM1 Shield

Once all the components are attached to the plexiglass, they can be wired to the shield. For the LEDs and IRs, the GND should be connected to the GND rails on the shield. For the solenoids, the polarity does not matter. **Figure 10** shows where the components should go on the shield. The wiring is as follows: **pins 4, 5, 6 for solenoids** / **pins 8, 9, 10 for LEDs** and **pins 11, 12, 13 for IRs.**

<p align="center">
    <img title = "figure10" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_9.Final_Assembly/imgs/Wiring.png?raw=true" align=center width=400/><br><br>
    <b><i>Figure 10: </b> Schematic showing where the components go on the shield </i>
</p>

### 6) Components completed
<p align="center">
    <img title = "figure11" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_9.Final_Assembly/imgs/Figure_10.png?raw=true" align=center width=350/><br><br>
    <b><i>Figure 11: </b> Front View of the completed DNAMIC box </i>
</p>

<p align="center">
    <img title = "figure12" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_9.Final_Assembly/imgs/Figure_11.png?raw=true" align=center width=350/><br><br>
    <b><i>Figure 12: </b> Top View of the completed DNAMIC box </i>
</p>

<p align="center">
    <img title = "figure13" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_9.Final_Assembly/imgs/Figure_12.png?raw=true" align=center width=350/><br><br>
    <b><i>Figure 13: </b> Side View of the completed DNAMIC box </i>
</p>

###### END OF CHAPTER
