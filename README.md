Multimodal-Brain-Computer-Interfaces
====================================
My research to using convolutional neural network architectures for decoding visual stimuli with EEGs.
------------------------------------------------------------------------------------------------------

## Background Info
This is a multidisciplinary research project, branching accross the fields of Neuroscience, Electrical Engineering,
 and Computer Science. Five programming languages were utilized to bring this research to fruition i.e. "Processing,
 Java, Batch, MATLAB, and Python". These languages provided the means to have a UI to collect the data with,
 preprocess the data, and run the encoded data through a convolutional neural network (CNN).

## Reminder
I will refer to different project components throughout this page as (1, 2, or 3).

## Project Components
1. Data Acquisition
2. Preprocessing
3. Creating the Classifier

## Hardware Components
* OpenBCI Cyton Board
* OpenBCI Daisy Board Add-on
* OpenBCI Wifi Shield
* (Recommended) GPU

### Prerequisites (1)
* Processing Language & IDE
* OpenBCI Hub Download
* OpenBCI GUI Download

### Prerequisites (2)
* Java Language
* IntelliJ IDE
* libGDX Framework
* MATLAB --- (Octave might work as an alternative)

### Prerequisites (3)
* Python2
* Pip
* (For CUDA Only) CUDA Drivers & Toolbox
* TensorFlow --- (For CUDA Only) choose the GPU option for installation

#### Versions
* TensorFlow v1.8
* Java 8
* OpenBCI GUI v3.3

#### Pip Installations (For The Dependencies)
* tensorflow
* numpy
* getpass
* argparse
* textwrap
* re
* itertools
* tfplot
* matplotlib
* sklearn
* scikitplot

### Resources
* [OpenBCI](http://openbci.com/)
* [libGDX](https://libgdx.badlogicgames.com/)
* [Java](https://java.com/en/download/)
* [MATLAB](https://www.mathworks.com/products/matlab.html)
* [Octave-alternative](https://www.gnu.org/software/octave/)
* [IntelliJ](https://www.jetbrains.com/idea/)
* [TensorFlow](https://www.tensorflow.org/)

## Run Intructions
### Running (1)
* Replace the corresponding processing source code files in the Sketch folder with what is in
 this repository
* Run the OpenBCI Hub application
* Open the Processing IDE
* Load the OpenBCI_GUI processing file
* Run the program
* Click stream data & Configure your gain settings accordingly
* Go to the other UI, type the amount of *minutes* to run the experiment for, and click start
* The participant will be randomly shown visual stimuli pertaining to different "fruit"
* The participant should only focus on identifying these fruit for the selected time & a new
 fruit will show up every second
* When the UI says complete, data will no longer be stored
* Exit the program & go to the saved data folder
* Find the txt file and rename it raw_(*the number of this trial should match the fruit_labels_## file*) e.g. raw_0.txt and fruit_labels_0.txt

### Running (2)
* Move the Batch and MATLAB file to the saved data folder
* Open my java project with intelliJ
* Go to the Preprocessing.java file
* Comment out line 79 and uncomment line 78
* Run the program & wait for the red screen
* Go to the Preprocessing.java file
* Comment out line 78 and uncomment line 79
* Run the program & wait for the blue screen

### Running (3)
* Move parser.py and generic_data_partitioner.py to the saved data folder
* Run parser.py
* Run generic_data_partitioner.py
* Move cnn_final.py your tmp folder
* Run cnn_final.py

#### Time Training Model w/ CPU vs GPU
* [CPU] --> Roughly 1 week training on an i7 intel processor
* [GPU] --> Roughly 2 hours training on an Nvidia 1070

### My Website
[Kyle Zeller](http://cs.oswego.edu/~kzeller/)

### My Contact Info
[Email](kzeller@oswego.edu)