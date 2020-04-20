# Chapter 1. Essential Tips and Tricks


____  
### Introduction
This page covers some basic knowledge and skills for those less familiar with building electronic platforms. 

### 1. Multimeter

Multimeters are a useful debugging tool for this project. [Amazon Link to Multimeter](https://www.amazon.com/AstroAI-Digital-Multimeter-Voltage-Tester/dp/B01ISAMUA6/ref=sr_1_1_sspa?keywords=multimeter&qid=1571619926&sr=8-1-spons&psc=1&spLa=ZW5jcnlwdGVkUXVhbGlmaWVyPUFINUcyVlJPTUk2S0gmZW5jcnlwdGVkSWQ9QTA4NTQ4Mzg1U0pNUlYxREUzN0QmZW5jcnlwdGVkQWRJZD1BMDAzNzc5MTNNMU05T1dXRVhWMEQmd2lkZ2V0TmFtZT1zcF9hdGYmYWN0aW9uPWNsaWNrUmVkaXJlY3QmZG9Ob3RMb2dDbGljaz10cnVl)

Multimeters can measure a lot of things including continuity, resistance, voltage, current, capacitance etc. But the most useful functionality (in my opinion) is the continuity / diode testing mode. This functionality allows you to check if a diode is working or not (which has directionality), and whether two points in a circuit are electrically connected or not. The multimeter will beep (output of a piezo buzzer) if the two points are connected and will light up the LED if the cathode is connected to GND and anode is connected to PWR. But always remember to turn the knob to continuity / diode testing mode before testing anything! Otherwise the multimeter would be powered off.

<p align="center">
    <img title = "multimeter" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/test_branch/Chapter_1.Getting_Started-Essential_Tips_and_Tricks/imgs/multimeter.jpg?raw=true" align=center width=200/><br><br>
    <b><i>Figure 1:</b> Continuity test mode shown on the multimeter (white circle). The value on the display indicate the resistance value. Value “1” signifies that it’s an open loop. </i>
</p>

<p align="center">
    <img title = "continuity_symbol" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/test_branch/Chapter_1.Getting_Started-Essential_Tips_and_Tricks/imgs/continuity_symbol.jpg?raw=true" align=center width=200/><br><br>
    <b><i>Figure 2:</b> Close up view of the continuity / diode testing option </i>
</p>

To provide more perspective, continuity testing is extremely useful in verifying your solder joints either on the printed circuit boards (PCB) or on any other wires. If you’ve soldered something on, probed the two solder points and got a beep, that means the two points are connected. Now this might be good or bad depending on each case. If you meant to connect the two points, then you're all set. If the two points are **NOT** supposed to be connected, then you have a short circuit. This means you’ll have to redo the solder connection, but doing this now will save you a ton of time in the future when you’re running your software on the circuit board and the hardware component is not working as you expected. (Hardware will not work properly if there is a short circuit!).

Below is a summary I found on [Adafruit.com](https://learn.adafruit.com/multimeters/continuity) on various things the continuity test can be useful for:

<p align="center">
<img title = "continuity_testing" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/test_branch/Chapter_1.Getting_Started-Essential_Tips_and_Tricks/imgs/continuity_testing.jpg?raw=true" align=center width=500/>
</p>   

#### Using the multimeter for this project

To make DIY-NAMIC boxes, the following major components are needed: PCB / LEDs / IRs/ and solenoids.

Using the multimeter on the PCB is fairly straightforward. If you want to verify connections between two points, you can probe it using the clips. If It’s connected, you should hear a beep. Using the multimeter on LEDs is simple as well. Once you connect them correctly, ***(cathode to GND / anode to PWR)*** the LED will light up (you will not hear any beeps). For IR LEDs, you won’t “see” the IRs light up because human eyes can’t detect infrared light but ***there are [tricks](https://nbviewer.ipython.org/github/jhl0204/DNAMIC-Hardware-Documentations/blob/master/Chapter_5.Component_Assembly-Infrared_Detectors/5_Component_Assembly_IR_vF.ipynb) you can use to "see" the IRs***. For solenoids, it’s a little different story. If you test out the two leads, although the two leads are not touching each other, the multimeter will give you a beep. 

<p align="center">
  <img title = "solenoid" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/test_branch/Chapter_1.Getting_Started-Essential_Tips_and_Tricks/imgs/solenoid.jpg?raw=true" align=center width=200/><br><br>
  <b><i>Figure 3:</b> Red arrow indicates Power (PWR) and the black arrow indicates Ground (GND) </i>
</p>   
See here for more info: [solenoid valve section](https://nbviewer.ipython.org/github/jhl0204/DNAMIC-Hardware-Documentations/blob/master/Chapter_6.Component_Assembly-Solenoid_Valves/6_Component_Assembly_Solenoid_Valves_vF.ipynb). The solenoids are actually continuous cylindrical coil of wire. The two leads you see in **Figure 3** are two ends of the same wire. The cylindrical coil is hidden inside the component. The exact resistance of the coil will depend on a lot of things, but it will tend to be very low and seem like a short circuit. If they don't have a low resistance, then it's likely that the wire has broken internally, and the valve is dead. So to sum it up, the “beep” you hear when you test out the continuity on the solenoid valves means that the valves are working!

### 2. Breaking off Pins

Breaking off header pins (especially female types) correctly is surprisingly difficult. If you try breaking them off with a wire cutter, you’ll notice that often times you end up with one less header than you intended because the encasings break off. Thus, this method of using the wire cutters is very unreliable when you want to get a specific length of the header pins.

<p align="center">
  <img title = "figure_4" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/test_branch/Chapter_1.Getting_Started-Essential_Tips_and_Tricks/imgs/figure_4.png?raw=true" align=center width=300/><br><br>
  <b><i> Figure 4:</b> Two types of header pins – Female (red circle) and Male (green circle) pins. </i>
</p>

<p align="center">
  <img title = "figure_5" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/test_branch/Chapter_1.Getting_Started-Essential_Tips_and_Tricks/imgs/figure_5.png?raw=true" align=center width=300/><br><br>
  <b><i> Figure 5:</b> An example of an improper way of breaking off pins. Notice that the metal header pin has fallen off from the black encasing.</i>
 </p>

--------------
 
 #### Making a 1x4 header pin

1. As a first step, you need to remove the $(n+1)^{th}$ pin from the parent bulk of pins. You can see from the yellow arrow in **Figure 6** that the 5th pin has been removed since our goal is to get a 1 x 4 pin.

<p align="center">
  <img title = "figure_6" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/master/Chapter_1.Getting_Started-Essential_Tips_and_Tricks/imgs/figure_6.png?raw=true" align=center width=300/><br><br>
  <b><i> Figure 6:</b> Female header pins after removing the (n+1)th pin. This location will later serve as the spot to make etched guidelines.</i>
 </p>

2. Next, you want to make **“cutting guidelines”** into the 5th encasing. The encasings are made of plastic so it’s pretty easy to do. You can see the etched guidelines in the red circle in **Figure 8**. Make these guidelines on both sides of the encasing. After making the guidelines, you can just snap them off. The header will easily snap off along the guidelines you have created.

<p align="center">
  <img title = "figure_7" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/master/Chapter_1.Getting_Started-Essential_Tips_and_Tricks/imgs/figure_7.png?raw=true" align=center width=300/><br><br>
  <b><i> Figure 7:</b> Making the cutting guidelines with a wire cutter </i>
 </p>

 <p align="center">
   <img title = "figure_8" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/master/Chapter_1.Getting_Started-Essential_Tips_and_Tricks/imgs/figure_8.png?raw=true" align=center width=300/><br><br>
   <b><i> Figure 8:</b> It might be a little hard to see, but you can fainlty notice the etched guidelines at the empty pin location (red circle) Once you have the guidelines, gently snap them off along the guidelines to get the finished product. </i>
  </p>

  <p align="center">
    <img title = "figure_9" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/master/Chapter_1.Getting_Started-Essential_Tips_and_Tricks/imgs/figure_9.png?raw=true" align=center width=300/><br><br>
    <b><i> Figure 9:</b> We have successfully made a 1x4 female header pin! Compare and contrast this to **Figure 5** where we failed to properly break off the pin size of our interest. </i>
   </p>

3. As a final touch, you can sand down these headers using a belt grinder (or with normal sandpaper) to give them a cleaner, smoother finish. The smooth finish will not only give the finished product a more professional look but also allow other components to fit better on the board.

<p align="center">
  <img title = "figure_10" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/master/Chapter_1.Getting_Started-Essential_Tips_and_Tricks/imgs/figure_10.png?raw=true" align=center width=300/><br><br>
  <b><i> Figure 10:</b> Before <b> red rectangle </b> and after <b> green rectangle </b> sanding down the headers. Notice the smoother finish in the 'after' products </i>
 </p>

 ### 3. Soldering Components to PCB

When soldering anything onto a PCB, you want the components to be flush with the board. Simply put, you don’t want your components to look like the X-marked headers in **Figure 1** below. This is surprisingly pretty tricky to do because headers tend to move around a lot when soldering. As you go through the pins in a serial fashion, you’ll quickly realize one small misalignment will lead to the misalignment of the whole component (like in **Figure 1** below) because solder joints cool down and harden very quickly.

<p align="center">
  <img title = "Image_1" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/master/Chapter_1.Getting_Started-Essential_Tips_and_Tricks/imgs/Image_1.png?raw=true" align=center width=300/><br><br>
  <i> Examples of good soldered (first and third) and bad soldered headers (second and fourth) <i/>
 </p>

 #### Soldering Components Flush with the board

The basic idea behind this trick is to temporarily affix the components / headers flush with the board with some tape, and soldering key anchor points to the board. Once you have the anchor points, you can take the tape off and solder the remaining leads to the board. I’ll use the stacking pins as an example to demonstrate this method.

1. Use tape to fixate the components / headers to the shield so that it doesn’t fall off even when the board is upside down

<p align="center">
  <img title = "figure_11" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/master/Chapter_1.Getting_Started-Essential_Tips_and_Tricks/imgs/figure_11.png?raw=true" align=center width=300/><br><br>
  <b><i> Figure 11:</b> Use tape to affix the stacking pins to the shield. (Top-down view) </i>
 </p>

 2. With the tape attached, solder just the two ends of the stacking pins so that you can take the tape off. These will be your anchor points.

 <p align="center">
   <img title = "figure_12" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/master/Chapter_1.Getting_Started-Essential_Tips_and_Tricks/imgs/figure_13.png?raw=true" align=center width=300/><br><br>
   <b><i> Figure 12:</b> Stacking pins after the anchor points (white circles) have been soldered on. Notice the silver solder joints within the white circles </i>
  </p>

3. Note that step 2 will not anchor the stacking pins perfectly flush with the shield (red box in **Figure 14**). To anchor the stacking pins flush with the shield, heat up your anchor solder joints and push in / wiggle the stacking pins against the shield until you feel that the stacking pins are flush.  

<p align="center">
  <img title = "figure_13" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/master/Chapter_1.Getting_Started-Essential_Tips_and_Tricks/imgs/figure_14.png?raw=true" align=center width=300/><br><br>
  <b><i> Figure 13:</b> Note that the stacking pins are not yet flush with the shield (red box). </i>
 </p>

 4. After adjusting the stacking pins and your anchor points, it’s time to solder in the remaining holes. If you feel that the stacking pins are getting misaligned as you solder, repeat step 3 so that the stacking pins are actually flush with board.

 <p align="center">
   <img title = "figure_14" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/master/Chapter_1.Getting_Started-Essential_Tips_and_Tricks/imgs/figure_15.png?raw=true" align=center width=300/><br><br>
   <b><i> Figure 14:</b> Bottom view of a finished solder work. Note all the solder connections (red box). </i>
  </p>

  <p align="center">
    <img title = "figure_15" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/master/Chapter_1.Getting_Started-Essential_Tips_and_Tricks/imgs/figure_16.png?raw=true" align=center width=300/><br><br>
    <b><i> Figure 15:</b> Side view of a finished solder work. Notice that the stacking pins are flush with the shield. Compare this image with <b> Figure 11 <b/>.</i>
   </p>
