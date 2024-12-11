# Sonification-of-Snake-Robot-Gaits

### UM-Dearborn ECE 591 - Directed Studies

Julia Korde (MS Robotics-2025)

Advisor - Dr. Alireza Mohammadi


### Description - Snake robot simulation data (angular position vs. time) are converted into audio files in a process called sonification

## Video - 

## Article - 

### Overview:
1. Create snake robot simulations
2. Change the gait parameters of the snake robot
3. Use the snake robot position data to create or modify music
  
### Tutorial - 
1. Download CoppeliaSim software -> https://www.coppeliarobotics.com/
2. Download and open provided robotic simulation files (under 'Simulation Files' directory)
   - Serpentine_Baseline.ttt
   - Serpentine_Case2.ttt
   - Serpentine_Case3.ttt
   - Serpentine_Case4.ttt
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
7. Download the provided music clips (under 'Music to Modify' directory)
   - Mozart.mp3 (see ref. [1])
   - Dvorak1.mp3 (see ref. [2])
   - Dvorak2.mp3 (see ref. [2])
9. Open the correct sonification code (matching the simulation) in Google Colab
10.  Upload the 'csv' file to use for the sonification to the Google Colab code environment
11. Run the sonification code
    - Note: For 'Music Modification' section, check that a music clips is uploaded to the Google Colab code environment)
12. Download the '.midi' file from the Google Colab environment to save the audio

### References:

[1]: Mozart, W.A. (1783). Piano Sonata No. 11 in A Major, K.331/330i, Rondo alla Turca: Allegretto. Album: Walter Gieseking: Historic Broadcast Performances (1944-1950).

[2]: Dvorak, A (1893). Symphony No. 9 in E minor Op.95 From the New World I.Adagio-Allegro molto. Album: LSO Live, London Symphony Orchestra (2005).

### Sources for Code Development:
- https://jbrussell.github.io/eilive2020/part2a_sonification/
- https://medium.com/@astromattrusso/sonification-101-how-to-convert-data-into-music-with-python-71a6dd67751
