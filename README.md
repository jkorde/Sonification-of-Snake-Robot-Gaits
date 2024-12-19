# Sonification-of-Snake-Robot-Gaits

### UM-Dearborn ECE 591 - Directed Studies

Julia Korde (MS Robotics-2025)

Advisor - Dr. Alireza Mohammadi


### Description - Snake robot simulation data (angular position vs. time) are converted into audio files in a process called sonification

## Video - https://youtu.be/A_cKRoLog4c

## Article - [Snake_Robot_Sonification.pdf](https://github.com/user-attachments/files/18203715/Snake_Robot_Sonification.pdf)


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
4. Open a simulation to modify the gait parameters and 'csv' file name
   
   ![image](https://github.com/user-attachments/assets/c926698c-d361-41c5-99b8-adfae7324c23)
   ![image](https://github.com/user-attachments/assets/5cb63881-6952-4a4a-b9c1-e4e907793fb8)
4. Run the simulation
   
   ![image](https://github.com/user-attachments/assets/23efb23a-87ed-42ea-a2a8-d4923493eb73)
5. Locate the 'csv' file on local drive
   
   ![image](https://github.com/user-attachments/assets/b4e19d81-7f5d-4daa-a5dd-2abecbf72380)
6. Download the provided sonification code (under 'Sonification Code' directory)
   - Serpentine.ipynb
   - Rectilinear.ipynb
   - Eel.ipynb
7. Download the provided music clips (under 'Music to Modify' directory)
   - Mozart.mp3 (see ref. [1])
   - Dvorak1.mp3 (see ref. [2])
   - Dvorak2.mp3 (see ref. [2])
8. Open the correct sonification code (matching the simulation) in Google Colab
9.  Upload the 'csv' file to use for the sonification to the Google Colab code environment
    
     ![image](https://github.com/user-attachments/assets/bce935f5-e06b-47b9-8d99-063a01a67ec6)
10. Run the sonification code
    - Note: For 'Music Modification' section, check that a music clips is uploaded to the Google Colab code environment)
      
    ![image](https://github.com/user-attachments/assets/01261752-c235-44f7-ac1f-c2ce19fb5837)
11. Download the '.wav' or 'mp3' file from the Google Colab environment to save the audio


### Remarks/Challenges:
- The scaling compression factor (f_scale) was linked to the max position value (max_vpos), if it was above 1 then some of the lower values merged into one low note
  
  ![image](https://github.com/user-attachments/assets/76dd4d0a-ef20-4ef9-b2ca-608059d6eafc)
  
- To create a larger audible difference to the position peaks (max_vpos), it was linked to the maximum and minimum volume with an exponential function
  ![image](https://github.com/user-attachments/assets/cb0ada52-768d-47a4-9977-54cd7838474a)

- The rectilinear gait had a sensitivity to changes in gait parameters, so only 2 scenarios were modeled



### References:

[1]: Mozart, W.A. (1783). Piano Sonata No. 11 in A Major, K.331/330i, Rondo alla Turca: Allegretto. Album: Walter Gieseking: Historic Broadcast Performances (1944-1950).

[2]: Dvorak, A (1893). Symphony No. 9 in E minor Op.95 From the New World I.Adagio-Allegro molto. Album: LSO Live, London Symphony Orchestra (2005).

### Sources for Code Development:
- https://jbrussell.github.io/eilive2020/part2a_sonification/
- https://medium.com/@astromattrusso/sonification-101-how-to-convert-data-into-music-with-python-71a6dd67751

### Paper for Further Reading:
- https://link.springer.com/article/10.1007/s11042-023-15385-y
