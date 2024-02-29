# Boron
This repositiory contains C++ code for the Boron that communicates with the OpenMV. 

The code contains 4 main sections:
      1. Setup of the Boron
      2. A loop that digital wirtes low, high, low, high that wakes up the OpenMV to 
          to undergo its seperate process that ultimately sends information back to             the Boron. 
      3. The boron prints to the serial monitor either "Flood" or "No Flood" which is           being reported back by OpenMV. 
      4. The Boron then sleeps for 60 seconds and then repeats. 

The goal of this code is to recieve data from the OpenMV which can then be used in seperate platforms if other code is added. 

