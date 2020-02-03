# Chapter 6. Component Assembly - Solenoid Valves

#### What you will learn:

Basics of solenoid valve operation, testing, and assembly + manifolds
___

### Introduction - What are solenoid valves?

A solenoid valve is an electromechanical device in which the solenoid uses an electric current to generate a magnetic field and thereby regulate fluid flow using a valve. Simply put, the magnetic field created by solenoids are what switches the valves on and off. Then what are solenoids? **A solenoid is a cylindrical coil of wire acting as a magnet when carrying electric current.** Solenoids are actually easily confused with electromagnets, but the key difference is that the solenoids don’t have a metal core in the center. If there was a magnetic core, then it would be an electromagnet and the strength of the magnetic field would be proportional to the electric current. Without the magnetic core, the wires would be called a solenoid and exist only in binary on and off states. This is why solenoids are used as simple binary switches in electrical systems.

<p align="center">
    <img title = "figure1" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_6.Component_Assembly-Solenoid_Valves/imgs/Figure_1.png?raw=true" align=center width=350/><br><br>
    <b><i>Figure 1:</b>Example of a solenoid. Note the absence of a magnetic core. Note that these solenoids are inside the solenoid valves. </i>
</p>

<p align="center">
    <img title = "figure2" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_6.Component_Assembly-Solenoid_Valves/imgs/Figure_2.png?raw=true" align=center width=350/><br><br>
    <b><i>Figure 2:</b> Different types of solenoid valves. </i>
</p>

For the DNAMIC boxes, we use the solenoid valves to control the flow of reward. There are a lot of different types of solenoid valves out there and you should explore the different types that best fit your own needs. In our lab, we use [LHDA0531115H](https://www.theleeco.com/products/electro-fluidic-systems/solenoid-valves/control-valves/lhd-series/3-port/ported/) (3-port ported solenoid valves) because they are compact, and we are able to attach appropriate tubing to effectively lengthen the distance of reward delivery.

____

### Solenoid Valve LHDA0531115H

The following is the solenoid valve we use in the lab. As you can notice from **Figures 3 and 4**, it is very small and has 3 ports.

<p align="center">
    <img title = "figure3" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_6.Component_Assembly-Solenoid_Valves/imgs/Figure_3_1.jpeg?raw=true" align=center width=300/><br><br>
    <b><i>Figure 3:</b> Use starburst for comparison! </i>
</p>

<p align="center">
    <img title = "figure4" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_6.Component_Assembly-Solenoid_Valves/imgs/Figure_4.png?raw=true" align=center width=350/><br><br>
    <b><i>Figure 4:</b> Notice that the top port is closed off and the bottom two ports are open. </i>
</p>

You might also notice from **Figure 4** that the top port is closed off and the bottom two are open. I won’t go into the details of how solenoid valves work, but basically the solenoids control the opening and closing of the ports by releasing or obstructing the openings of the ports using a plunger (**Figure 5**). And with electrical current, we can control how long the valves stay open or closed. That’s how solenoid valves can dispense water (or any liquid or gas). Let's also look at a diagram from the official specification sheet to understand the solenoid valves better.

<p align="center">
    <img title = "figure5" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_6.Component_Assembly-Solenoid_Valves/imgs/Figure_5_1.png?raw=true" align=center width=350/><br><br>
    <b><i>Figure 5:</b> Cross section view of the solenoid valve. Solenoid coil (green) controls the plunger (blue) which in turn determines which of the three ports will be open. </i>
</p>

<p align="center">
    <img title = "figure6" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_6.Component_Assembly-Solenoid_Valves/imgs/Figure_6.png?raw=true" align=center width=400/><br><br>
    <b><i>Figure 6:</b> Diagram of the ports in solenoid LHDA0531115H. Note that the ports are either <b>‘normally closed’, ‘common’, or ‘normally open’</b> / Source: Lee Company </i>
</p>

As you can see from **Figure 6** the top port is 'normally closed' while the bottom port is 'normally open'. The middle port is 'common'. To be perfectly honest, I am not sure what this means or why the solenoids are designed like so. ***(Comments / Pull Requests / Feedback would be much appreciated from the enginnering community out there!)*** From what I've figured out however, I can control the fluid flow using the middle and top ports when the solenoid valve is powered up. Also, since the bottom port is “normally open”, we need to cap the port so that the fluid doesn’t leak during operation. In order to make the cap, I’ve just burned one side of the tubing and fitted it over the bottom port. **(Figure 7)**

<p align="center">
    <img title = "figure7" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_6.Component_Assembly-Solenoid_Valves/imgs/Figure_7.png?raw=true" align=center width=350/><br><br>
    <b><i>Figure 7:</b> Tubing have been burnt at one end to be used as caps for the bottom port of the solenoid valve. </i>
</p>

### Manifolds

DNAMIC boxes were designed to hold three noseports and thus three reward centers. Each reward center requires a solenoid valve which in turn requires a separate reward (fluid) source. However having a reward source for each solenoid valve is spatially expensive. Could there be a hardware that can solve this problem? Meet manifolds. Manifolds are chambers that branch into several openings, just like in **Figure 8** where the manifold branches out into 3 different ports or outlets (see the numberings 1, 2 and 3 in the figure). Our lab picked this [particular manifold](https://www.mcmaster.com/catalog%2f125%2f237) (Ref #: 5203K929) because it would allow fluid control to 3 different solenoid valves using just one syringe as an inlet source. These are also push-to-connect manifolds meaning that you can just push in the appropriate tubing into the orange outlet and the “claws” within the port will clamp down on the tubing and hold it down. Just make sure that the tubing end is cut evenly since a slanted cut will affect the effectiveness of the clamp. When inserting the tubing, make sure to pull out the orange O-ring completely, insert tubing, and push in the orange O-rings again. The tubing specifications used for the solenoid valves and manifolds can be found in the [Bill of Materials](https://github.com/jhl0204/AIM-Hardware-Documentations/wiki/Bill-of-Materials) (Part #: TET-062A)

<p align="center">
    <img title = "figure8" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_6.Component_Assembly-Solenoid_Valves/imgs/Figure_8_1.png?raw=true" align=center width=350/><br><br>
    <b><i>Figure 8:</b> Diagram of how the fluid will flow in the system. White arrows denote the direction of fluid flow. The dashed arrows signify that it will flow only when solenoid valve is powered up. Note that only one solenoid valve was shown in this example. Also note that the tubing from manifold is attached to the top port of the solenoid valve and the tubing from reward spout is attached to the middle port. </i>
</p>

<p align="center">
    <img title = "figure9" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_6.Component_Assembly-Solenoid_Valves/imgs/Figure_9.png?raw=true" align=center width=350/><br><br>
    <b><i>Figure 9:</b> Push-to-connect manifolds side by side. The orange O-ring is where the tubing goes in and can slide in and out. </i>
</p>

The tubing that goes into the manifold will connect to the top port of the solenoid (refer to **Figures 4 and 6**). When the manifold is fitted onto the manifold encasing, the length required for the tubing to reach the solenoid is about ~13cm. However, you can’t extend the length of the tubing after a cut, so give yourself some extra length and cut about 15cm for the tubing. These push-to-connect manifolds are prone to leaks and you might end up readjusting (pull out and re-insert) often.

<p align="center">
    <img title = "figure10" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_6.Component_Assembly-Solenoid_Valves/imgs/Figure_10_2.png?raw=true" align=center width=350/><br><br>
    <b><i>Figure 10:</b> Manifold fitted with appropriate tubing. The numbers represent the number of outlets. </i>
</p>

The manifolds are also more prone to leakage when placed vertically. They will be lying horizontally on the encasings in the finished product however, so as long as the manifolds don’t leak when laid horizontally, you don’t need to worry about the leak. If they keep leaking after multiple adjustments however, try to identify the source and glue it in with Loctite 401. Personally, I found that the juncture between the body and the orange O-ring turns out to be the source of the leak 90% of the time, so that’s where I would use Loctite **(Figure 11)**. Going forward however, I believe a new manifold is needed since more than 80% of the outlets have been leaking with the normal push-to-connect mechanism.

<p align="center">
    <img title = "figure11" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_6.Component_Assembly-Solenoid_Valves/imgs/Figure_11.png?raw=true" align=center width=350/><br><br>
    <b><i>Figure 11:</b> Red arrow represents where I have glued the orange slider to the body. Green arrows indicate that no glue was used. </i>
</p>

###### END OF CHAPTER
