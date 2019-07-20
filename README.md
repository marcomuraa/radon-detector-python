# Radon detector Python
 Using Google's tensorflow library to detect and count Radon in provided images quickly and efficiently. For a brief introduction i reccomend you read [this Google Doc](https://docs.google.com/document/d/17juSBhaiAiygBygc_O9VRmdZct-5RxTr5DOl4vL7SNY/edit?usp=sharing).

# Installation
In order to run the program you will first need to install TensorFlow correctly on your system. 

First install Python (on Mac and Linux it's already there, on Windows download the installer from [here](https://www.python.org/)).

# Windows
1) Install Anacoda
2) Clone my repository on your computer
3) Download [the tensorflow-models](https://github.com/tensorflow/models/tree/master/research) repository
4) Copy the research folder from models-master into radon-detector-python folder
5) Do this command
    > https://tensorflow-object-detection-api-tutorial.readthedocs.io/en/latest/install.html
    Get-ChildItem object_detection/protos/*.proto | foreach {protoc "object_detection/protos/$($_.Name)" --python_out=.}
 compiles protobuf
>
6) go into research folder
    ```
    python setup.py build
    ```
    ```
    python setup.py install
    ```

7) Finally  cd.. then python radon_detector_v5.py
8) Pray it works otherwise :goberserk:

