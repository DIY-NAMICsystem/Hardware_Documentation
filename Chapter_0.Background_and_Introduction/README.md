# Chapter 0. Introduction: Dartmouth Nautiyal Arduino Modular Instrumental Conditioning (DNAMIC) Boxes*

### Background - Current Limitations in Behavioral Neuroscience Research
Many psychiatric disorders emerge during adolescence [[1]](https://www.ncbi.nlm.nih.gov/pubmed/28198416), necessitating a careful study of this period in order to prevent these disorders from the onset. To study rodent behavior, behavioral neuroscientists have traditionally used operant boxes from [Med Associates](https://www.med-associates.com/). While these boxes offer diverse and reliable paradigms to test unique behavioral phenotypes of adolescents [[2]](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5453624/), most of the paradigms require months to train the subjects. Considering that the adolescence period in mice span only about 2 weeks, this temporal constraint poses a significant hindrance to studying adolescence in a controlled environment.

### Introduction
A major reason why the paradigms take weeks to just complete the training phase is because mice are not exposed to the paradigms around the clock and thus can't learn quickly. Due to the design and nature of the Med Associates Operant boxes, mice can only be trained on a particular paradigm for a given amount of time per day. Coupled with the reality that most labs try to fit in multiple experiments in their set of operant boxes, the amount of time subjects have per day to learn a certain paradigm is severely limited.

Our lab's solution to this problem was to create a home-cage based operant box so that mice are exposed to paradigms 24 hours a day and can self-pace their learning. While this solution has its limitations such as the inability to group-house animals, it offers many more advantages such as the following.


### Advantages of using AIM  
#### 1. Decreased Stressors for Animal Subjects / Elimination of Confounders

- Subjects have *ad libitum* access to food and can earn unlimited water rewards depending on their task performance. *Ad libitum* access prevents pronounced weight loss, a putative stress-inducing factor for mice.


- Subjects undergo decreased animal handling since experimenters do not have to transfer mice to the operant boxes for training/testing. Animal handling is also a putative stress-inducing factor that is a confounder for mice behavior.


- Subjects do not have to acclimatize to a new environment (Med Associates operant boxes) for paradigm training/testing. Exposure to new environment is another putative confounder for mice behavior especially during adolescence when novelty seeking behavior is high.

#### 2. Better Data Quality

- 24 hour automated data collection, which allows high temporal resolution data and reduces most of labor-intensive work for the experimenter.

#### 3. Decreased Experiment Time

- Subjects have 24 hour access to a given paradigm, allowing them to learn the paradigms quickly. In fact, mice have learned the variant 5-choice serial reaction time task in just 2 weeks, a paradigm that typically takes months to complete. This is a crucial reason why we can study **adolescence** using AIM.


#### 4. Compatibility / Flexibility

- Compatible with standard laboratory colony caging setups.

#### 5. Low Cost

- Inexpensive and low-cost relative to traditional Med Associates operant boxes, making high throughput experiments feasible. For comparision, a typical Med Associates [Behavioral Test Box with Five Hole Nose Poke for Mouse](https://www.med-associates.com/product/five-hole-nose-poke-wall-chamber-package-for-mouse-2/) costs \$4000 per box. AIM costs \$200 per box with an initial equipment investment cost of \$340.


#### 6. Open Source

- All design files and code are open source - Contribution from members of the research community will improve this project and set forth new avenues for better tools in behavioral neuroscience research. Being open source also means that the software is free. For comparision, Med Associates requires a compatible software rig to be purchased with its boxes. Med Associates rig that supports up to 8 boxes cost \$6800. AIM runs on open-source Arduino platform, that supports unlimited number of Arduino microprocessors.

### Quick Cost Comparison Chart
- For 8 boxes

Cost| Med Associates Boxes | Arduino Instrumental Modules (AIM)
------|:-------:| -----
**Box** | 8 x \$4000 = \$32,000 | \$340 + (8 x \$200) = \$1,940
**Software** | \$6,800 | \$0  
**Total** | \$38,800 | \$1,940



* AIM requires about initial equipment investment of \$340.

**Conclusion:** 20-fold reduction in cost when using AIM!
