# Radon detector Python
 Using Google's tensorflow library to detect and count Radon in provided images quickly and efficiently. For a brief introduction i reccomend you read [this Google Doc](https://docs.google.com/document/d/17juSBhaiAiygBygc_O9VRmdZct-5RxTr5DOl4vL7SNY/edit?usp=sharing).

# Installation
In order to run the program you will first need to install TensorFlow correctly on your system; we will do so in a virtual environment to have better control over the versions of the various libraries.

There is a tutorial in italian [here]().

## Windows ("easier" version)
The only downside to this method is the large download that is required, other than this it should be easier because the folder structure is pre-made.
1) Start by downloading [this compressed folder](https://drive.google.com/open?id=1ba9smJ6EyU7Ho2CajvDAVb4LB5ki_an7);
2) Extract it somewhere on your computer (I suggest putting it in the root of the drive, for example C:\radon-detector-python, and perhaps rename it to something shorter);
3) Install Anacoda from [here](https://anaconda.org/);
4) Open a new Anaconda Prompt as Administrator; 
5) Create a new virtual environment:
    ```
    conda create -n radon pip python=3.6
    ```
    note: you can change "radon" to whatever you want;
6) Now install tensorflow and the other required libraries:
    ```
    pip install tensorflow==1.13.1
    pip install pillow
    pip install opencv-python
    ```
7) Go into the "research" folder and run
    ```
    python setup.py build
    ```
    and then
    ```
    python setup.py install
    ```
8) Close and reopen the Anaconda prompt (as Administrator). Now cd into the directory where the program is and run
    ```
    python radon_detector_v5.py
    ```

## How to use the program
1) Click on "open image dir" and select the folder where the images are; make sure that the folder only contains image files;
2) Press START;
3) The program should count and display the number of Radon traces it thinks there are in the image.


