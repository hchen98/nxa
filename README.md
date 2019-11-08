# nxa
An RC car based on ROS, Raspberry Pi, Keras, and Donkey<sup>®</sup> Car API

**Demo**:

[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/cA7kywWOXXk/0.jpg)](https://www.youtube.com/watch?v=cA7kywWOXXk)

---
<h4>Requirements:</h4>

-   Python 3.x
-   Raspberry Pi 3/ 4 (recommended and used in this project) or Nvidia Jetson Nano
-   Servo Driver PCA 9685
-   Magnet Car or alternative
-   ROS/ Raspbian Lite
-   3D printed parts

<hr>

<h4>Brief View of Hardware Setup:</h4>
<img src="https://github.com/879099766/nxa/blob/master/Wire%20Connection.png">

<hr>
<h4>Collecting Data:</h4>

1. Collbrate with Pi:
```bash
$ donkey calibrate --channel x/x
```
2. Drive the Pi:
```bash
$ python drive.py
```
3. View the drive control panel on host computer:
Opening your web broswer and typing your Pi's IP address and port *`8887`*

e.g., `127.0.0.1:8887`

<hr>

<h4>To get start with training model and drive:</h4>

1. Trand your Keras Model
```bash
$ python train.py [tub directory]
```
2. Drive with your trained model
```bash
$ python train.py [tub directory]
```

 ***NOTE***: Donkey<sup>®</sup> Car project provides Unity simulator for training. [Chech out here!](http://docs.donkeycar.com/guide/simulator/ "Chech out here!")
