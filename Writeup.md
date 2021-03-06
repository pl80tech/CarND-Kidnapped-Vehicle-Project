# **Kidnapped Vehicle Project** 
[![Udacity - Self-Driving Car NanoDegree](https://s3.amazonaws.com/udacity-sdc/github/shield-carnd.svg)](http://www.udacity.com/drive)

---
## Writeup

This is my writeup for the project "Kidnapped Vehicle" of Self Driving Car Nanadegree on Udacity.

[//]: # (Image References)

[image1]: ./output/KidnappedVehicle.gif "Kidnapped Vehicle (Animation)"
[image2]: https://i.ytimg.com/vi/2Qa63TRbtpw/hqdefault.jpg "Thumbnail on Youtube"

---

### Contents

* [About Kidnapped Vehicle Project](#About-Kidnapped-Vehicle-Project)
* [Project code](#Project-code)
* [Output video](#Output-video)
* [Some notes](#Some-notes)

---
## About Kidnapped Vehicle Project

The goals / steps of this project are the following:

* Implement a 2 dimensional particle filter in C++ given a map, some initial localization information and observation/control data at each time step.
* More detail explanation can be found in [README](https://github.com/pl80tech/CarND-Kidnapped-Vehicle-Project/blob/master/README.md)

---
## Project code

Here is my working repository for this project:

https://github.com/pl80tech/CarND-Kidnapped-Vehicle-Project

It is imported and frequently updated (cherry-pick or merge) from below original repository:

https://github.com/udacity/CarND-Kidnapped-Vehicle-Project

---
## Output video

Here are the links to the output videos which were uploaded on Github and Youtube (for easy reference). Click on the thumbnail image to jump to the video on Github/Youtube.

| Link on Youtube              | Link on Github               |
|:----------------------------:|:----------------------------:|
|[![alt text][image2]](http://www.youtube.com/watch?v=2Qa63TRbtpw)|[![alt text][image1]](https://github.com/pl80tech/CarND-Kidnapped-Vehicle-Project/blob/master/output/KidnappedVehicle.mp4)|

---
## Some notes

### Debug option

 Add definition DEBUG in [helper_functions.h](https://github.com/pl80tech/CarND-Kidnapped-Vehicle-Project/blob/master/src/helper_functions.h) as below before compiling the sources to show debug messages with detail information.
 ```C++
 // Flag to enable debug messages with detail information
 // Comment out to disable
 #define DEBUG
 ```
 Another way is to add below description to [CMakeLists.txt](https://github.com/pl80tech/CarND-Kidnapped-Vehicle-Project/blob/master/CMakeLists.txt) to compile the sources with definition DEBUG.
 ```txt
 add_definitions(-DDEBUG)
 ```

 After adding DEBUG option in [CMakeLists.txt](https://github.com/pl80tech/CarND-Kidnapped-Vehicle-Project/blob/master/CMakeLists.txt) (by [following commit](https://github.com/pl80tech/CarND-Kidnapped-Vehicle-Project/commit/fff9b471c156a4fda7033c7fcfba1d74a920434c)), debug option can be enabled by simply specifying -DDEBUG=ON when running cmake as below: 
 ```shell
 $ cmake -DDEBUG=ON ..
 $ make
 ```

### Test code

Folder [/test_code/](https://github.com/pl80tech/CarND-Kidnapped-Vehicle-Project/tree/master/test_code) includes the code (Jupyter notebook, C++) for the quiz on lesson 2 ~ 6. Refer to the description on [runtest.sh](https://github.com/pl80tech/CarND-Kidnapped-Vehicle-Project/blob/master/test_code/runtest.sh) about how to compile and run the C++ code.