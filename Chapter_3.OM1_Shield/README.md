# Chapter 3. OM1 Shield (soldering the components)

#### What you will learn:

Soldering on the necessary components to make a functioning OM1 Shield
____

One of the great things about Arduinos is that you can add various functionalities on top of the bare-bone Arduino. You can do this with Arduino shields, which you can stack on top of the Arduino to add new functionalities. These shields allow the Arduino to connect to WiFi, Ethernet, and even power up components that require more voltage than its microprocessor (ATMEGA328P) can normally handle. Shields usually come shipped ready to be used with Arduinos, but if you're building one from scratch (from printed circuit boards), you'll have to add some components. Our lab ordered PCBs to build a compatible shield from scratch and in this section, we will go through the steps on how to attach the necessary components to make a functioning OM1 shield (designed by [openmaze.org](http://openmaze.org/)).

### OM1 Shield

One of my Principal Investigator's colleague has already implemented Arduino shields (OpenMaze 1 – OM1 for short) to run his own behavioral experiments and luckily for us, the designs were open source. You can find details about the the shield [here](www.openmaze.org). To give you a brief summary however, these are the major features of the OM1 shield:

1)	7 pins broken out to Power-Ground-Input-Output (PGIO) ports (red box)  
> **IMPORTANT:** Breakout pins 7,8,9,10 are not connected to normal Arduino power. In order to supply 5V power to these 4 breakout pins, you must connect the pink circle (arrow) with the other pink circle with a jumper wire. For 12V power, connect the pink circle (arrow) with the green circle (refer to PCB connection diagram for explanation).  

2)	socket for the H-bridge chip (green box)  
3)	4 pins broken out for solenoid valves (blue box)  
4)	a connector for MPR121 capacitive touch sensor (yellow box) - won’t be using in the lab  

<p align="center">
    <img title = "figure1" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_3.OM1_Shield/imgs/Figure_1.png?raw=true" align=center width=300/> <br><br>
    <b><i>Figure 1:</b> Diagram of the OM1 Shield. Source: <a href="http://www.openmaze.org/ "> Link </a> </i>

</p>

Note that the picture above is a bare bone shield. The electrical connections are all imprinted within the printed circuit board (PCB), but it won’t work unless we attach the necessary components and the headers! This section will detail the steps on how to solder on the necessary components.

<p align="center">
    <img title = "figure2" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_3.OM1_Shield/imgs/Figure_2.png?raw=true" align=center width=300/><br><br>
    <b><i>Figure 2:</b> Small version of all the electrical connections within the OM1 Shield. Red and blue lines are used just to differentiate connections. They do not carry any meaning.
</p>

### Necessary Components

Below is a picture of the necessary components that we have to solder on to the OM1 shield.

<p align="center">
    <img title = "figure3" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_3.OM1_Shield/imgs/Figure_3.png?raw=true" align=center width=300/><br><br>
    <b><i>Figure 3:</b> List of components needed to make a functioning OM1 Shield.</i>
</p>

The following is the list of bare minimum materials necessary to make a functioning OM1 Shield. For more details and where to purchase them, refer to the [Bill of Materials](https://github.com/jhl0204/AIM-Hardware-Documentations/wiki/Bill-of-Materials)

- OM1 Shield
- pushbutton
- 2.1mm DC Barrel Jack
- Stacking Headers (1x10 (1) / 1x8 (2) / 1x6 (1))
- Chip Socket + H Bridge
- Female + Male Headers

##### What is a H-Bridge? (optional)

> At this point you might be wondering what a H-bridge is. (If you haven’t been wondering, that’s fine too – you can skip this part). There are a bunch of online resources that explain how H-bridges work and in which settings they are used. I won’t go into those details because all the “under the hood” intricacies are not important for our purposes. We only need to know that H-bridges are electric circuits that can reverse the polarity of the voltage and that they can “amplify” low power signals to high power signals. That is how Arduinos, which has a 5V limit, use H-bridges to power up solenoids which require 9V input. H-bridges are also used widely in robotics to drive motors forward and backward. For reference though, we are using a dual H-Bridge motor driver (L293D) that can run four solenoids at once with a limit of 600mA per channel.

Links for more learning:   
1) [Making H-Bridge on a Breadboard](https://www.instructables.com/id/H-Bridge-on-a-Breadboard/)  
2) [Basics of H-Bridge](http://www.modularcircuits.com/blog/articles/h-bridge-secrets/h-bridges-the-basics/)  
3) [Driving a DC Motor using H-Bridge](http://hades.mech.northwestern.edu/index.php/Driving_a_high_current_DC_Motor_using_an_H-bridge)  

### Soldering Diagram

Once you have all the components ready, you can just solder those components according to the diagram below. For best solder results however, refer to tips 2 and 3 from [Essential Tips and Tricks](https://nbviewer.ipython.org/github/jhl0204/DNAMIC-Hardware-Documentations/blob/master/Chapter_1.Getting_Started-Essential_Tips_and_Tricks/1_Essential_Tips_and%20Tricks_vF.ipynb) before starting.

<p align="center">
    <img title = "figure4" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_3.OM1_Shield/imgs/Figure_4.png?raw=true" align=center width=500/><br><br>
    <b><i>Figure 4:</b> The physical components are color coded with red, stacking headers with dark blue, and female headers with green. When soldering on any components, make sure to adjust the pins if necessary so that they would fit into the holes on the board.</i>
</p>

### Note on the Chip Socket

The chip socket and the H-bridge chip have directionality. When soldering on the chip socket and inserting the H-bridge chip, make sure the semicircle is aligned according to the arrow. The semicircle in the chip determines the location of pin 1. As can be seen from **Figure 6**, pin 1 starts from the upper left corner where the semicircle is located. For more details on how the H-bridge connects to the solenoid, see the diagram below **Figure 6**. Also you might have realized that the socket doesn’t actually have directionality (only H-Bridges do). However, I do recommend aligning the socket as well since it would be easier to remember the direction when inserting in the H-bridge.

<p align="center">
    <img title = "figure5" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_3.OM1_Shield/imgs/Figure_5.png?raw=true" align=center width=300/><br><br>
    <b><i>Figure 5:</b> Note how the half circle in the chip socket is aligned in the direction of the yellow arrow. Red box is explained in detail in <b> Figure 6. </b></i>
</p>

<p align="center">
    <img title = "figure6" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_3.OM1_Shield/imgs/Figure_6.png?raw=true" align=center width=300/><br><br>
    <b><i>Figure 6:</b> Diagram of H-bridge used in OM1 Shield. <a href="http://www.openmaze.org/"> Source </a> </i>
</p>

### Finished Shield

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
