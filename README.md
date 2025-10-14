# Programming-course-2025: Particle Physics
Purpose of code:
  Simulating particle production expected by a specific model commonly used in particle physics using Python 3.
  This code requires the installation of pandas https://pypi.org/project/pandas/.

Questions that will be answered:
  1)What are the average counts of each particle species and their statistical uncertainties?  
  
  2)Is there any asymmetry between the particle and the anti-particle?  
  
  3)Is there any asymmetry as a function of their momentum?  
  

Data included:
  - 5 million pp collisions at √s = 14 TeV across
  - 11 output files containing 500k collisions each
  - 6 particles and their anti-particles
  - Momentum calulations for each group of particles
  - Number of events each particle appeared
  - Average number of each particle per event
  - Statisitcal Uncertainity and Standard Deviation of particles per event
  - Plots of asymmetry as a function of each particle's momentum

Discussion:


    
Results of this code:  
// added new results for all 11 files + added new event counter which prevents events between files from merging that caused 'per event' calculations to be off by several magnitudes  

// also made it so that code now correctly averages across all events instead of each event with the particle inside of it  

// converted to a markdown table for easier reading  


| Particle Type   |   Total number of particles |   Average particles per event |        Std |   Statistical Uncertainty |
|:----------------|----------------------------:|------------------------------:|-----------:|--------------------------:|
| anti-p          |                 5.46837e+06 |                    1.18501    |  1.51006   |               0.000675317 |
| anti-Λ          |                 1.25466e+06 |                    0.271887   |  0.574873  |               0.000257091 |
| p               |                 5.57853e+06 |                    1.20888    |  1.53935   |               0.000688418 |
| Κ+              |                 1.1587e+07  |                    2.51092    |  2.78308   |               0.00124463  |
| Κ-              |                 1.15607e+07 |                    2.50524    |  2.7826    |               0.00124442  |
| Λ               |                 1.27728e+06 |                    0.276789   |  0.582206  |               0.00026037  |
| Ξ+              |            180093           |                    0.0390265  |  0.200699  |               8.97555e-05 |
| Ξ-              |            182130           |                    0.0394679  |  0.201785  |               9.02412e-05 |
| Ω+              |              5318           |                    0.00115242 |  0.0339661 |               1.51901e-05 |
| Ω-              |              5482           |                    0.00118796 |  0.0345217 |               1.54386e-05 |
| π+              |                 9.21259e+07 |                   19.9639     | 18.1886    |               0.00813417  |
| π-              |                 9.19769e+07 |                   19.9316     | 18.1716    |               0.00812659  |


  
| Particle Pair   |    Asymmetry |
|:----------------|-------------:|
| π+ - π-         |  0.000809363 |
| Κ+ - Κ-         |  0.00113402  |
| p - anti-p      |  0.00997148  |
| Λ - anti-Λ      |  0.00893388  |
| Ξ+ - Ξ-         | -0.00562361  |
| Ω+ - Ω-         | -0.0151852   |

This code searches for momentum of <200 to remove extreme outliers for better calculations  

Below is the relevant graph plotting asymmetry and momentum  

<img width="1536" height="760" alt="Graphs" src="https://github.com/user-attachments/assets/9c0fc014-2180-4107-884e-1eeff7d19b3a" />
