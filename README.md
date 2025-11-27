# Forest Fire Model

This is an adaptation of the Forest Fire Model by Veritasium, as demonstrated in their [YouTube video](https://www.youtube.com/watch?v=HBluLfX2F_k).  
  
## Video Contents
This video explores the difference between the normal distribution (bell curve), where outcomes cluster around an average, and the power law distribution, where a few extreme outliers dominate the average. It uses examples like wealth distribution, the St. Petersburg paradox, and natural phenomena like earthquakes and <mark>forest fires</mark> to show how systems in a "critical state" (like self-organized criticality) often follow a power law, making large, unpredictable events inevitable. The key takeaway is that understanding which distribution governs a domain should fundamentally change how one approaches decision-making and risk, with power law-governed fields rewarding riskier, persistent bets over consistent average performance.
  
## The Forest Fire Model (Drossel–Schwabl)
The video discusses the concept behind the Drossel-Schwabl model through its forest fire simulator, which serves as an example of a system exhibiting Self-Organized Criticality (SOC).  
  
This model demonstrates that a system with simple rules—like trees growing on empty squares and random "lightning strikes" causing fires will naturally tune itself to a critical state without any external fine-tuning. In this critical state, the resulting fire sizes follow a power law distribution. This means that while most fires are small, the probability of extremely large, massive fires is significantly higher than you would expect from a normal distribution. The key insight is that large fires are not caused by special events; they are simply magnified versions of small fires, all triggered by a single lightning strike, making the occurrence of system-altering events unpredictable and inevitable.  

## This Project
This project however was more ispired by the forest fire model itself rather than the video topic of power law distribution, which I did still find interesting. I essentailly want to try to develop the Drossel-Schwabl model from an example of power law and instead add more factors to increase its realism. In my adapted version, I have added a few extra parameters and features:
- Neighbor Reproduction Boost: The first of these extra parameters is a neighbor reproduction boost. It attempts to simulate the way that trees usually disperse their seeds only in the area around them.
- River & River Buffer Zones: The second of these extra features is a river crossing the simulated area. It attempts to demonstrate the fact that trees living in areas near or next to rivers are less likely to catch fire. Various parameters for this feature is able to be edited.
- River Fire Jump: The third feature is the ability for fire to jump across narrow parts of the river. This feature is not the most functional.
- Seed & Environment: The seed sets the internal pseudo-random number generator. Given the same seed and the same parameters, the simulation is reproducible:
  - The wiggly river’s shape is determined by the seed.
  - The initial random growth of trees is determined by the seed.
  - Lightning strikes and fire spread follow the same sequence for a fixed seed.
  
## Links
- [Veritasium's Forest Fire Model (Drossel–Schwabl)](https://www.veritasium.com/simulation5)
  
- [My Adapted Model](josiahlegg.com/forest-fire-model-v1.1)
