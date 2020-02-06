
# DIY-Nautiyal Arduino Modular Instrumental Conditioning (DIY-NAMIC) Boxes for Behavioral Neuroscientists


<p align="center">
    <img src="https://media.giphy.com/media/iKFyMgWnooZwu8bYSN/giphy.gif" align=center width=500/><br>
    <b><i>Figure 1:</b> Mouse retrieving water reward during behavioral testing in the DNAMIC box.</i>
</p>

<p align="left">
  <img src="readme_imgs/diagonal_view.jpg" align=center width=300/><br>
    <b><i>Figure 2:</b> Diagonal View </i>
</p>

<p align="left">
  <img src="readme_imgs/side_view.png" align=center width=300/><br>
    <b><i>Figure 3:</b> Side View </i>
</p>

<p align="left">
  <img src="readme_imgs/top_view.jpg" align=center width=300/><br>
    <b><i>Figure 4:</b> Top View </i>
    <br>
    <br>
</p>

<p align="center">
  <img src="readme_imgs/boxes_in_action.png" align=center width=400/><br>
</p>

**Figure 5:** *DIY-NAMIC boxes in operation in the vivarium on a standard ventilated rack. Data is collected automatically by Processing software to a computer in the next room.*
___

### What is DIY-NAMIC?

The DIY-NAMIC box is a customizable, low-cost apparatus for automated homecage operant behavioral testing. Made with Arduino microprocessor, 3D printed parts, and various *off-the-shelf* components, the boxes enable 24-hour data collection, significantly increasing trials/day without food or water restriction, and allowing for self-initiated trials during rodent's dark/active phase.  

Most importantly, this is an open-source project - any contributions / suggestions / feedback are welcome and appreciated!

___
### Benefits of DIY-NAMIC boxes.

1. Decreased Experiment Length
Rodents have 24 hour access self-initiated trials allowing hundreds of trials per day. This allows for faster testing, reducing the number of days that many standard operant paradigms typically takes to run. This also permits testing during developmental time periods which can be very limited in rodents.

2. Inexpensive compared to commercially available operant testing chambers
All the materials used to make one DNAMIC box cost around $200, compared to$4000-$10,000 for the commercially-available units, which have limited customizability.

3. No food or water restriction
Mice consume their normal daily intake of water, and no food deprivation is required.  The sated condition is important for the interpretation of many behavioral effects.  Additionally, this allows testing during development when food/water deprivation can be deleterious to growth.

4. Reduced daily experimenter effort
There is minimal daily effort required from the experimenter, since mice are living in their homecage, and data is logged in realtime.

5. More ethologically-relevant testing
Through self-initiated trials, mice can perform during their standard dark/active phase of the light-dark cycle. 

There are other key benefits to using AIM and you can find a complete list of benefits and advantages in the [Introduction]().


___
### Overview

The purpose of this repository is to provide **hardware manuals and documentations** for anyone who would like to build their own AIM for use in behavioral neuroscience research. This manual is intended for behavioral neuroscientists without previous experience in engineering or computer science. Therefore the manuals sometimes include explanations on the inner workings of major components used in AIM.

The online documentation is divided into three different repositories. The present repository contains the **hardware** build instructions, the [second repository](https://github.com/jhl0204/DNAMIC_Arduino_Software_Programs) contains the programs for the **behavioral paradigms**. The [last repository](https://github.com/jhl0204/DNAMIC_Data_Analysis) contains Python scripts for **data analysis** of the behavioral output. 


#### Contents

* [**Chapter 0 - Background and Introduction**](https://nbviewer.ipython.org/github/jhl0204/DNAMIC-Hardware-Documentations/blob/master/Chapter_0.Background_and_Introduction/0_Background_and_Introduction_vF.ipynb) 
* [**Chapter 1 - Getting Started - Essential Tips and Tricks**](https://nbviewer.ipython.org/github/jhl0204/DNAMIC-Hardware-Documentations/blob/master/Chapter_1.Getting_Started-Essential_Tips_and_Tricks/1_Essential_Tips_and%20Tricks_vF.ipynb)
* [**Chapter 2 - Modifying the Rodent Cage**](https://nbviewer.ipython.org/github/jhl0204/DNAMIC-Hardware-Documentations/blob/master/Chapter_2.Modifying_Rodent_Cage/2_Modifying_the_Rodent_Cage_vF.ipynb)
* [**Chapter 3 - OM1 Shield**](https://nbviewer.ipython.org/github/jhl0204/DNAMIC-Hardware-Documentations/blob/master/Chapter_3.OM1_Shield/3_OM1_Shield_vF.ipynb)
* [**Chapter 4 - Component Assembly - LED**](https://nbviewer.ipython.org/github/jhl0204/DNAMIC-Hardware-Documentations/blob/master/Chapter_4.Component_Assembly-LED/4_Component_Assembly_LED_vF.ipynb)
* [**Chapter 5 - Component Assembly - Infrared Detectors**](https://nbviewer.ipython.org/github/jhl0204/DNAMIC-Hardware-Documentations/blob/master/Chapter_5.Component_Assembly-Infrared_Detectors/5_Component_Assembly_IR_vF.ipynb)
* [**Chapter 6 - Component Assembly - Solenoid Valves**](https://nbviewer.ipython.org/github/jhl0204/DNAMIC-Hardware-Documentations/blob/master/Chapter_6.Component_Assembly-Solenoid_Valves/6_Component_Assembly_Solenoid_Valves_vF.ipynb)
* [**Chapter 7 - Component Assembly - Reward Spout**](https://nbviewer.ipython.org/github/jhl0204/DNAMIC-Hardware-Documentations/blob/master/Chapter_7.Component_Assembly-Reward_Spout/7_Component_Assembly_Reward_Spout_vF.ipynb)
* [**Chapter 8 - Wiring and Soldering**](https://nbviewer.ipython.org/github/jhl0204/DNAMIC-Hardware-Documentations/blob/master/Chapter_8.Wiring_and_Soldering/8_Wiring_and_Soldering_vF.ipynb)
* [**Chapter 9 - Final Assembly**](https://nbviewer.ipython.org/github/jhl0204/DNAMIC-Hardware-Documentations/blob/master/Chapter_9.Final_Assembly/9_Final_Assembly_vF.ipynb)

* [**Appendix - Bill of Materials**](https://github.com/jhl0204/AIM-Hardware-Documentations/wiki/Bill-of-Materials)

____
### Other open-source projects in the behavioral neuroscience community

1. [Feeding Experimentation Device (FED) - Kravitz Lab](https://github.com/KravitzLab/FED)
2. [CombiCage - Loos Lab](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5309744/)
3. [ArControl - Li Lab](https://github.com/chenxinfeng4/ArControl)
4. [Openmaze.org](http://openmaze.org/) - open source hardware and software for behavioral neuroscience
5. [Openbehavior.com](http://openbehavior.com/) - repository of open source tools for advancing behavioral neuroscience research]

DIY-NAMIC
### Development
_____

##### What to Contribute

- Inaccurate / incorrect information regarding components or explanations
- Typos or grammar mistakes
- Component suggestions
- Your own tips, tricks, and experiences for any hardware projects.

- If you decide to make DIY-NAMIC boxes yourself, send us photos and any hacks/design modifications that you made! We would love to see how this project expands! Feel free to open an issue or submit a pull request, or email jun.ho.lee@dartmouth.edu.


### Contributions and Thanks
_____

A big thanks to **Andrew R. Alvarenga** for his generous support and suggestions regarding hardware. Thank you for also allowing me to use the machine shop and test out different prototypes of the 3D printed parts on the 3D printer.

Thank you to undergraduate researchers **Bonnie Shea** and **Selin Capan** for assisting with daily running of the code.


#### Contact

For any questions or issues, contact **Jun Ho Lee** at jun.ho.lee@dartmouth.edu or **Katherine Nautiyal** at katherine.nautiyal@dartmouth.edu.
