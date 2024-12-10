# Sonification-of-Snake-Robot-Gaits
## Julia Korde, advisor - Dr. Alireza Mohammadi
### UM-Dearborn ECE 591 - Directed Studies

Description - Snake robot simulation data (angular position vs. time) are converted into audio files in a process called sonification

Video - 

Article - 

Overview:
1. Create snake robot simulations
2. Change the gait parameters of the snake robot
3. Use the snake robot position data to create or modify music
  
Tutorial - 
1. Download CoppeliaSim software -> https://www.coppeliarobotics.com/
2. Download and open provided robotic simulation files (under 'Simulation Files' directory)
   - Serpentine_Baseline.ttt
   - Serpentine_Case2.ttt
   - Serpentine_Case3.ttt
   - Rectilinear_Baseline.ttt
   - Rectilinear_Case2.ttt
   - Rectilinear_Case3.ttt
   - Eel_Baseline.ttt
3. Open a simulation to modify the gait parameters and 'csv' file name
4. Run the simulation
5. Locate the 'csv' file on local drive
6. Download the provided sonification code (under 'Sonification Code' directory)
   - Serpentine.ipynb
   - Rectilinear.ipynb
   - Eel.ipynb
7. Open the correct sonification code (matching the simulation) in Google Colab
8.  Upload the 'csv' file to use for the sonification to the Google Colab code environment
9. Run the sonification code
10. Download the '.midi' file from the Google Colab environment to save the audio

Contact:
Julia Korde - jkorde@umich.edu

References for Code Development:
- https://jbrussell.github.io/eilive2020/part2a_sonification/
- https://medium.com/@astromattrusso/sonification-101-how-to-convert-data-into-music-with-python-71a6dd67751
