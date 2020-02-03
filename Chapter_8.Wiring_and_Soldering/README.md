# Chapter 8. Wiring and Soldering

#### What you will learn:

How to wire the components (IR / solenoids / LEDs) to the jumper wires
____

### Introduction

In any type of electronics project, you will start off with a breadboard and jumper wires to wire things up as a prototype. As things become more complicated and you know that your prototype works, you will want to make your project permanent by soldering / crimping components together.  

<p align="center">
    <img title = "figure1" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_8.Wiring_and_Soldering/imgs/Figure_1.png?raw=true" align=center width=350/><br><br>
    <b><i>Figure 1:</b> Simple Half-Breadboard </i>
</p>

<p align="center">
    <img title = "figure2" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_8.Wiring_and_Soldering/imgs/Figure_2.png?raw=true" align=center width=350/><br><br>
    <b><i>Figure 2:</b> Three types of jumper wires: Male/Male, Male/Female, Female/Female </i>
</p>

### Soldering or Crimping

The difference between soldering and crimping is that crimping is an electrical connection done with physical force while soldering involves making a connection by heating up the wires and connecting them with solder alloy. Personally, I prefer crimping when making electrical connections because they offer more flexibility and reliability compared to soldering. However, soldering can be great for making quick electrical connections that you might later “undo” since you can always de-solder them by applying additional heat. Soldering and crimping each offers its advantages and disadvantages but given the components we work with in the lab, I’ve decided to take advantage of both crimping and soldering.

### Hacking the Dupont connectors

When connecting components to the breadboard or generally connecting two points together, we slide in the male wire to the female jumper wire. We can do this thanks to the Dupont connectors at the end. Dupont connectors are standardized pins that are 0.1” (2.54mm) in width. The widths are standardized so that they fit on Arduinos and other breakout boards. In fact, the spacings between each pin on Arduinos is also 0.1” (2.54mm).

<p align="center">
    <img title = "figure3" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_8.Wiring_and_Soldering/imgs/Figure_3.png?raw=true" align=center width=350/><br><br>
    <b><i>Figure 3:</b> Female Dupont connectors (red) and Dupont connectors with housing (blue) </i>
</p>

<p align="center">
    <img title = "figure4" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_8.Wiring_and_Soldering/imgs/Figure_4.png?raw=true" align=center width=350/><br><br>
    <b><i>Figure 4:</b> Male Dupont connector can fit into Female Dupont connector. </i>
</p>

You can see an example of a female Dupont connector in **Figure 3**. This picture was taken after removing the black encasing on the red wire. The yellow arrows show you where the crimp was made to the red wire. Actually, you can make your own Dupont connectors at home with a crimping tool, male/female pins, and encasings. ([See Youtube Video](https://www.youtube.com/watch?v=N3zK9fzIPBo)) However, note that the in-house crimp connections won’t be as good as factory-made connections.

Now for prototyping purposes, it is sufficient to just use jumper wires to connect components to the Arduino or to the breadboard. I would do this by sliding in the component lead into one of the female-type Dupont connectors. This wouldn’t work so well when you want to make the wiring permanent. The leads will slide right off with a gentle tug. To prevent this, you would slide in the component lead right into the bare-bone female Dupont pins that have their encasing removed and solder the two parts together **(Figure 5).** In an ideal world, you would directly crimp the components to the wires but since that method proved to be too time consuming, I have opted for this current method.

<p align="center">
    <img title = "figure5" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_8.Wiring_and_Soldering/imgs/Figure_5.png?raw=true" align=center width=350/><br><br>
    <b><i>Figure 5:</b> Sliding in the male pin to the female Dupont connector with the encasing removed </i>
</p>

I will demonstrate this method using the LED wirings as an example. Note that all the jumper wires that were used were 30cm long and were of the female – to – male type.

<p align="center">
    <img title = "figure6" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_8.Wiring_and_Soldering/imgs/Figure_6.png?raw=true" align=center width=350/><br><br>
    <b><i>Figure 6:</b> LED wiring stages </i>
</p>

The above picture **(Figure 6)** depicts the wiring schemes in different stages. In stage 1, you have the component leads. In stage 2, you can see the jumper wires with their black encasings removed. (yellow arrows) Also in stage 2, you see that the male pins have slid into the female Dupont pins. To make them permanent, I have made a solder connection where the male pin and the female Dupont pin overlap. And finally in step 3, I have shrunken down heat shrink tubes with a lighter. Note that you must slide in the appropriately sized heat shrink tubes before you make the solder connection between the wires and the component.

The purpose of the heat shrink tube is to provide the solder joint with flexibility and protection. Soldered connections can be prone to fraying, especially at the juncture where the wire was crimped (red circle). This is because excess solder can potentially seep through and expand the space between the wire and the crimp. Therefore it is imperative that we use heat shrink tubes to provide support to the solder junction.

<p align="center">
    <img title = "figure7" src="https://github.com/selincapan/DNAMIC-Hardware-Documentations/blob/finished-mardown-files/Chapter_8.Wiring_and_Soldering/imgs/Figure_7.png?raw=true" align=center width=350/><br><br>
    <b><i>Figure 7:</b> Fraying of the wire at the crimp junction (red circle). Excess solder probably weakened the crimp connection. </i>
</p>

### Example: Photo interrupters

We will use the same method as above to solder the IR photo interrupters to the jumper wires. Remember to use female – to – male jumper wires that are 30cm long. Note however that the length of the wires will depend on your individual project.

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
