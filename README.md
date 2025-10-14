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

    
Results of this code: 
// added new results for all 11 files + added new event counter which prevents events between files from merging that caused 'per event' calculations to be off by several magnitudes 
// also made it so that code now correctly averages across all events instead of each event with the particle inside of it

      ID Particle Type  Average particles per event  Number of events        Std  Statistical Uncertainty
   Particle Type  Total number of particles  Average particles per event        Std  Statistical Uncertainty
0         anti-p                  5468374.0                     1.185008   1.510055                 0.000675
1         anti-Λ                  1254658.0                     0.271887   0.574873                 0.000257
2              p                  5578528.0                     1.208878   1.539350                 0.000688
3             Κ+                 11586991.0                     2.510924   2.783082                 0.001245
4             Κ-                 11560741.0                     2.505236   2.782604                 0.001244
5              Λ                  1277278.0                     0.276789   0.582206                 0.000260
6             Ξ+                   180093.0                     0.039027   0.200699                 0.000090
7             Ξ-                   182130.0                     0.039468   0.201785                 0.000090
8             Ω+                     5318.0                     0.001152   0.033966                 0.000015
9             Ω-                     5482.0                     0.001188   0.034522                 0.000015
10            π+                 92125884.0                    19.963864  18.188553                 0.008134
11            π-                 91976878.0                    19.931574  18.171601                 0.008127

This code searches for momentum of <200 to remove extreme outliers for better calculations

<img width="1536" height="760" alt="Graphs" src="https://github.com/user-attachments/assets/9c0fc014-2180-4107-884e-1eeff7d19b3a" />
