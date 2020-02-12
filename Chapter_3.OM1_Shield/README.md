# Chapter 3. OM1 Shield

Arduino shields allow functionalities to be added to the basic microprocessor.  DIY-NAMIC boxes require this because of the additional voltage needed for the solenoid components (anove what the ATMEGA328P microprocessor can handle).  The build protocol described here starts with a printed circuit board onto which necessary components are soldered on.  The OpenMaze.org OM1 shield (designed by [openmaze.org](http://openmaze.org/)) is used here.

### Components added to the OM1 Shield

1)	7 pins broken out to Power-Ground-Input-Output (PGIO) ports (red box)  
> **IMPORTANT:** Breakout pins 7,8,9,10 are not connected to normal Arduino power. In order to supply 5V power to these 4 breakout pins, you must connect the pink circle (arrow) with the other pink circle with a jumper wire. For 12V power, connect the pink circle (arrow) with the green circle (refer to PCB connection diagram for explanation).  
2)	socket for the H-bridge chip (green box)  
3)	4 pins broken out for solenoid valves (blue box)  
4)	a connector for MPR121 capacitive touch sensor (yellow box) - not used in this version of DIY-NAMIC boxes  

<p align="center">
    <img title = "figure1" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_3.OM1_Shield/imgs/Figure_1.png?raw=true" align=center width=300/> <br><br>
    <b><i>Figure 1:</b> Diagram of the OM1 Shield. Source: <a href="http://www.openmaze.org/ "> Link </a> </i>

</p>

Note that the picture above is the bare printed circuit board (PCB) on to which the necessary components must be attacehd! This section will detail the steps to solder on the necessary components.

<p align="center">
    <img title = "figure2" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_3.OM1_Shield/imgs/Figure_2.png?raw=true" align=center width=300/><br><br>
    <b><i>Figure 2:</b> Small version of all the electrical connections within the OM1 Shield. Red and blue lines are used just to differentiate connections. They do not carry any meaning.
</p>

### Components

Below is a picture of the components which are soldered on to the OM1 shield.

<p align="center">
    <img title = "figure3" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_3.OM1_Shield/imgs/Figure_3.png?raw=true" align=center width=300/><br><br>
    <b><i>Figure 3:</b> List of components needed to make a functioning OM1 Shield.</i>
</p>

Components for building shield:
For more details and where to purchase them, refer to the [Bill of Materials](https://github.com/jhl0204/AIM-Hardware-Documentations/wiki/Bill-of-Materials)

- OM1 Shield Printed Circuit Board
- pushbutton
- 2.1mm DC Barrel Jack
- Stacking Headers (1x10 (1) / 1x8 (2) / 1x6 (1))
- Chip Socket + H Bridge**
- Female + Male Headers

##### **What is a H-Bridge? 

> H-bridges are electric circuits that “amplify” low power signals. Since Arduinos have a 5V limit, H-bridges are used to power solenoids which require 9V input. H-bridges are also commonly used to drive motors using Arduinos. The H-bridge we are using is a dual H-Bridge motor driver (L293D) that can run four solenoids at once with a limit of 600mA per channel.

Links for more learning:   
1) [Making H-Bridge on a Breadboard](https://www.instructables.com/id/H-Bridge-on-a-Breadboard/)  
2) [Basics of H-Bridge](http://www.modularcircuits.com/blog/articles/h-bridge-secrets/h-bridges-the-basics/)  
3) [Driving a DC Motor using H-Bridge](http://hades.mech.northwestern.edu/index.php/Driving_a_high_current_DC_Motor_using_an_H-bridge)  

### Soldering Diagram

Components are soldered to the OM1 shield according to the diagram below. For best solder results however, refer to tips in [Essential Tips and Tricks](https://nbviewer.ipython.org/github/jhl0204/DNAMIC-Hardware-Documentations/blob/master/Chapter_1.Getting_Started-Essential_Tips_and_Tricks/1_Essential_Tips_and%20Tricks_vF.ipynb) before starting.

<p align="center">
    <img title = "figure4" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_3.OM1_Shield/imgs/Figure_4.png?raw=true" align=center width=500/><br><br>
    <b><i>Figure 4:</b> The physical components are color coded with red, stacking headers with dark blue, and female headers with green. When soldering on any components, make sure to adjust the pins if necessary so that they would fit into the holes on the board.</i>
</p>

### Note on the Chip Socket

The chip socket and the H-bridge chip have directionality. When soldering on the chip socket and inserting the H-bridge chip, make sure the semicircle is aligned according to the arrow. The semicircle in the chip determines the location of pin 1. As can be seen from **Figure 6**, pin 1 starts from the upper left corner where the semicircle is located. For more details on how the H-bridge connects to the solenoid, see the diagram below While the socket doesn’t actually have directionality (only H-Bridges do), it is recommened to align the socket to ensured proper H-bridge directionality.

<p align="center">
    <img title = "figure5" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_3.OM1_Shield/imgs/Figure_5.png?raw=true" align=center width=300/><br><br>
    <b><i>Figure 5:</b> Note how the half circle in the chip socket is aligned in the direction of the yellow arrow. Red box is explained in detail in <b> Figure 6. </b></i>
</p>

<p align="center">
    <img title = "figure6" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_3.OM1_Shield/imgs/Figure_6.png?raw=true" align=center width=300/><br><br>
    <b><i>Figure 6:</b> Diagram of H-bridge used in OM1 Shield. <a href="http://www.openmaze.org/"> Source </a> </i>
</p>

### Attaching the shield to the Ardunino UNO
Once the components are soldered to the OM1 PCB shield, the shield is attached to the Arduino via the stacking headers

<p align="center">
    <img title = "figure7" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_3.OM1_Shield/imgs/Figure_7.png?raw=true" align=center width=300/><br><br>
    <b><i>Figure 7:</b> Top view of the finished OM1 Shield </i>
</p>

<p align="center">
    <img title = "figure8" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_3.OM1_Shield/imgs/Figure_8.png?raw=true" align=center width=300/><br><br>
    <b><i>Figure 8:</b> OM1 Shield stacked on top of the Arduino. </i>
</p>

<p align="center">
    <img title = "figure9" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_3.OM1_Shield/imgs/Figure_9.png?raw=true" align=center width=300/><br><br>
    <b><i>Figure 9:</b> Side view of the Arduino + OM1 Shield </i>
</p>

<p align="center">
    <img title = "figure10" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_3.OM1_Shield/imgs/Figure_10.png?raw=true" align=center width=300/><br><br>
    <b><i>Figure 10:</b> Front view of the Arduino + OM1 Shield </i>
</p>

###### END OF CHAPTER
