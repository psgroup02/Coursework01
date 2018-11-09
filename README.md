# Simulator of Density
  
**Version 1.0.0**

This software simulates bidimensionally the density of pumas and hares in an area covered by both land and water.

## User Guide

### Software needed:

* Programming Language: Python 2.7

* Libraries: PyQt4 and Numpy.

* Additional packages: PIL, matplotlib.

### How to Start

* **Execute the package**

&nbsp; &nbsp; &nbsp; &nbsp; A file called **simulation.tar.gz** compressed contains the executable file to do the simulation.

&nbsp; &nbsp; &nbsp; &nbsp; Run the following commands to display the application:

```
tar -xvf simulation.tar.gz
./main
```

* **Parameters**

&nbsp; &nbsp; &nbsp; &nbsp; The software models the density of hares and pumas that can be obtained simply by changing the values of the parameters.

&nbsp; &nbsp; &nbsp; &nbsp; Parameters are initially set and the values can be substituted after or before *Uploading Landscape*, but not after clicking on *Start*.

&nbsp; &nbsp; &nbsp; &nbsp; The values of the first seven parameters have to be double except the **timestep** which is an integer from 2 to 500.

* **Upload Landscape**

&nbsp; &nbsp; &nbsp; &nbsp; Click on *Upload* to upload a file that contains a matrix of size up to 2000x2000 elements.

&nbsp; &nbsp; &nbsp; &nbsp; The elements of the matrix must be 0s or 1s that can be represented in a *black/white .bmp file* or explicit written in a *.txt* or *.dat* file.

&nbsp; &nbsp; &nbsp; &nbsp; A diagram in gray & blue will be displayed in the right half of the window. The blue color represents the water and the gray, the land.

### Run the simulation

Click on the button *Start* to run the simulation. It will return a diagram colored with red that represents the density of pumas, and in blue color, the density of hares.

**Note:** When the simulation ends, a new window pop-up will appear in the middle of the Window. Additionally, directories with format *Output\<datetime\>* which includes images of the state on each timestep will be generated.

### The Results

* Av. Density of Hares: This value will be updated as the timestep progresses. This consider the average of density of hares of all the squares(from the land area).

* Av. Density of Pumas: This value will be updated as the timestep progresses. This consider the average of density of pumas of all the squares(from the land area).

* Timesteps: According the parameter given as an input, the timestep will be updated until the simulation ends.

* Simulation Time: it will indicate the time in format *hh:mm:ss* as the timestep will be changed.
