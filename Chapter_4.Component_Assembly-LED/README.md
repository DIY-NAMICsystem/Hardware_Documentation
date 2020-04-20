# Chapter 4. Component Assembly - LED (Light Emitting Diodes)

#### What you will learn:

Basics of LEDs and how to solder them on to the customized nose ports
___

### Introduction
LEDs (light emitting diodes) are incorporated into the customized nose ports to function as stimuli.

<p align="center">
    <img title = "figure1" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_4.Component_Assembly-LED/imgs/Figure_1.png?raw=true" align=center width=300/><br><br>
    <b><i>Figure 1:</b> The LED has been threaded through the holes in the noseports. <b>Left:</b> Front View / <b>Right:</b> Back View</i>
</p>

<p align="center">
    <img title = "figure2" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_4.Component_Assembly-LED/imgs/Figure_2.png?raw=true" align=center width=300/><br><br>
    <b><i>Figure 2:</b>  Using the multimeter to test the LED is helpful before soldering them in place. <b>Left:</b> Front View / <b>Right:</b> Back View</i>
</p>

### About LEDs

LEDs, or diodes in general, have two polarized legs. One is the cathode (-) and the other is the anode (+). In LEDs, the cathode tip (-) is shorter than the anode (+). What I mean by polarized is that there is a directionality in the current flow. LEDs won’t light up unless you connect the cathode to ground (GND) and anode to power (PWR). Circuit diagram in **Figure 4** shows this directionality clearly. In order to power up the LED, current must flow from the anode to the cathod. And just a quick refresher for the engineering students reading this manual. The little diagonal arrows going in the 1 o’clock direction in the circuit symbol signifies that it is a light-emitting diode. Without the small arrows, the circuit symbol would signify a diode.

<p align="center">
    <img title = "figure3" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_4.Component_Assembly-LED/imgs/Figure_3.png?raw=true" align=center width=300/><br><br>
    <b><i>Figure 3:</b> LED with the cathode lead and the anode lead. Image Source: <a href="http://sciencewithkids.com/science-facts/facts-about-LEDs.html"> Link </a> </i>
</p>

<p align="center">
    <img title = "figure4" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_4.Component_Assembly-LED/imgs/Figure_4.png?raw=true" align=center width=300/><br><br>
    <b><i>Figure 4:</b> Diagram of how current flows in an LED. Note how the <b>flat (blunt) spot</b> is the cathode tip. Image Source: <a href="http://www.mainbyte.com/ti99/electronics/led.html"> Link </a> </i>
</p>

### Importance of Current-Limiting Resistors

The brightness of an LED depends directly on how much current it draws. So the more current it draws, the brighter it is going to be. The forward current increases exponentially as a function of forward voltage. (If the terms forward current ($I_{f}$), forward voltage ($V_{f}$)are unfamiliar to you, it simply means how much current and voltage is being run across that component.) Too much current equals too much power and too much heat, which will eventually burnout the LED and could also potentially damage the whole circuit (including the Arduino). 

<p align="center">
    <img title = "figure5" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_4.Component_Assembly-LED/imgs/Figure_5.png?raw=true" align=center width=350/><br><br>
    <b><i>Figure 5:</b> IV curve (current versus voltage curve) for different types of LEDs. You can notice that the current increase is exponential as a function of forward voltage. Image Source: <a href="http://lednique.com/current-voltage-relationships/iv-curves/"> Link </a></i>
</p>

Essentially this is why we need current-limiting resistors for LEDs. The name is self-explanatory. Resistors prevent excessive current flow to LEDs so that they may operate under maximum forward current ($I_{f}$) and not burn themselves out. Typically, the maximum forward current is 20mA for most LEDs.

To calculate current-limiting resistor values for different types of LEDs, you can use this [resistor value calculator](https://www.digikey.com/en/resources/conversion-calculators/conversion-calculator-led-series-resistor), but if you just want the short answer/want to play it safe, we use 1k Ω for our blue LEDs. Considering that blue LEDs typically have a forward voltage of 3.0V, this will effectively give us 2mA of operating current for the LED. For more information on picking resistors for LEDs, check out [this blog](https://www.evilmadscientist.com/2012/resistors-for-leds/) from **evilmadscientist.com**

### Soldering LEDs

#### Note of Warning

>Do a simple continuity test with a multimeter on the LEDs so that you know that the LEDs are not faulty. Remember to connect the anode to PWR (red) and cathode to GND (black). Additionally, if you have a breadboard and an Arduino in hand, you can just hook up a simple circuit with a resistor to test out that the LEDs are working.

Since everything will be connected in series, the current limiting resistor can go on either anode or cathode. The LEDs will receive a dialed-down current no matter where you connect the resistor. To standardize things however, we will solder the resistor to the cathode (-) so that it will be easier to distinguish the cathode terminal. As I’ve mentioned before, the cathodes have shorter leads than anodes. If you’ve already cut the terminals however, and can’t distinguish the length, there are other ways to tell. If you look at **Figure 4**, you will see that the cathode tip has a flat surface on the LED. On the other hand, anodes will have a rounder surface. Since cathodes connect to GND, I like to remember this scheme as **“blunt is black”** (Electrical engineers typically color code PWR with red and GND with black).

###### END OF CHAPTER
