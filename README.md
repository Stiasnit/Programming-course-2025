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

    
Results of this code: (Ran into memory issues running this code with all 11 files, currently in process of solving this, see below results for 500k particles in output-set1)

      ID Particle Type  Average particles per event  Number of events        Std  Statistical Uncertainty
0  -3334            Ω+                     1.000000               544   0.000000                 0.000000
1  -3312            Ξ+                     1.035993             17670   0.194309                 0.001462
2  -3122        anti-Λ                     1.249198            101060   0.550232                 0.001731
3  -2212        anti-p                     2.099594            260699   1.455190                 0.002850
4   -321            Κ-                     3.373277            344187   2.751152                 0.004689
5   -211            π-                    20.208140            456538  18.200839                 0.026937
6    211            π+                    20.232215            456633  18.213585                 0.026953
7    321            Κ+                     3.369051            344562   2.741307                 0.004670
8   2212             p                     2.128621            262889   1.492391                 0.002911
9   3122             Λ                     1.254797            102313   0.554331                 0.001733
10  3312            Ξ-                     1.037240             17481   0.199076                 0.001506
11  3334            Ω-                     1.001686               593   0.041065                 0.001686

