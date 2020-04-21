# Chapter 8. Wiring and Soldering

#### What you will learn:

How to wire the components (IR / solenoids / LEDs) to the jumper wires
____

### Introduction

Protoyping with a breadboard and jumper wires is a helfpul initial step. As things become more complicated and you know that your prototype works, you will want to make your project permanent by soldering / crimping components together.  

<p align="center">
    <img title = "figure1" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_8.Wiring_and_Soldering/imgs/Figure_1.png?raw=true" align=center width=350/><br><br>
    <b><i>Figure 1:</b> Simple Half-Breadboard </i>
</p>

<p align="center">
    <img title = "figure2" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_8.Wiring_and_Soldering/imgs/Figure_2.png?raw=true" align=center width=350/><br><br>
    <b><i>Figure 2:</b> Three types of jumper wires: Male/Male, Male/Female, Female/Female </i>
</p>

### Hacking the Dupont connectors

When connecting components to the breadboard or generally connecting two points together, we slide in the male wire to the female jumper wire. We can do this thanks to the Dupont connectors at the end. Dupont connectors are standardized pins that are 0.1” (2.54mm) in width (same as Arduinos and breadboards).  

<p align="center">
    <img title = "figure3" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_8.Wiring_and_Soldering/imgs/Figure_3.png?raw=true" align=center width=350/><br><br>
    <b><i>Figure 3:</b> Female Dupont connectors (red) and Dupont connectors with housing (blue) </i>
</p>

<p align="center">
    <img title = "figure4" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_8.Wiring_and_Soldering/imgs/Figure_4.png?raw=true" align=center width=350/><br><br>
    <b><i>Figure 4:</b> Male Dupont connector can fit into Female Dupont connector. </i>
</p>

You can see an example of a female Dupont connector in **Figure 3**. This picture was taken after removing the black encasing on the red wire. The yellow arrows show you where the crimp was made to the red wire. 

For prototyping purposes, it is sufficient to just use jumper wires to connect components to the Arduino or to the breadboard. For permanent wiring, the component lead can be inserted directly into the bare-bone female Dupont pins that have their encasing removed, and then the two parts can be soldered together **(Figure 5).** 

<p align="center">
    <img title = "figure5" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_8.Wiring_and_Soldering/imgs/Figure_5.png?raw=true" align=center width=350/><br><br>
    <b><i>Figure 5:</b> Sliding in the male pin to the female Dupont connector with the encasing removed </i>
</p>

<p align="center">
    <img title = "figure6" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_8.Wiring_and_Soldering/imgs/Figure_6.png?raw=true" align=center width=350/><br><br>
    <b><i>Figure 6:</b> LED wiring stages </i>
</p>

The above picture **(Figure 6)** depicts the wiring schemes in different stages. In stage 1, the component leads are shown. In stage 2, the jumper wires have the black encasings removed. (yellow arrows) Also in stage 2, the male pins were connected to the female Dupont pins. To make them permanent, I have made a solder connection where the male pin and the female Dupont pin overlap. And finally in step 3, the heat shrink is heated with a lighter. Note that the appropriately sized heat shrink tubes before you make the solder connection between the wires and the component.

<p align="center">
    <img title = "figure7" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_8.Wiring_and_Soldering/imgs/Figure_7.png?raw=true" align=center width=350/><br><br>
    <b><i>Figure 7:</b> Fraying of the wire at the crimp junction (red circle). Excess solder probably weakened the crimp connection. </i>
</p>

### Example: Photo interrupters

The same method is used to solder the IR photo interrupters to the jumper wires (female – to – male 30 cm long). 

<p align="center">
    <img title = "figure8" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_8.Wiring_and_Soldering/imgs/Figure_8.png?raw=true" align=center width=350/><br><br>
    <b><i>Figure 8:</b> Materials Needed for IR - wire soldering </i>
</p>

<p align="center">
    <img title = "figure9" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_8.Wiring_and_Soldering/imgs/Figure_9.png?raw=true" align=center width=350/><br><br>
    <b><i>Figure 9:</b> Wiring the IRs. Notice the heat shrink tubes (red arrow) </i>
</p>

<p align="center">
    <img title = "figure10" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_8.Wiring_and_Soldering/imgs/Figure_10.png?raw=true" align=center width=350/><br><br>
    <b><i>Figure 10:</b> Wiring the phototransistors. Notice the heat shrink tubes (red arrow) </i>
</p>

<p align="center">
    <img title = "figure11" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_8.Wiring_and_Soldering/imgs/Figure_11.png?raw=true" align=center width=350/><br><br>
    <b><i>Figure 11:</b> Completed wiring. Before and after applying heat to shrink tubes. </i>
</p>

###### END OF CHAPTER
