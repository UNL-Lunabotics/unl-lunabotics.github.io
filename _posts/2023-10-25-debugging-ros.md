---
published: true
---
# How to Debug in ROS

## General Debugging:

Check to make sure a ROS topic is published:
```
rostopic list
```

Check to see what is being published on a ROS topic named topic_name:
```
rostopic echo /topic_name
```

## Commonly Encountered Errors:

```
roslaunch: [ ] is neither a launch file in package [ ] nor is [ ] a launch file name
```
* make sure you source the setup.bash file
* rospack find
    * can be used to find the absolute path to a package - if rospack cannot find the file there's an issue
    
```
module error, no module named rospkg
```
* This problem comes from ros being made that we are using Python3 with ros melodic as we should be using Python2
* To fix make sure you have pip3 downloaded "sudo apt-get install Python3-pip" then make sure you have it downloaded with "pip3 --version", then instal rospkg with pip3 "pip3 install rospkg" the problem should now be fixed!

```
Can't launch node of type rosserial
```
* Make sure you have rosserial installed with "sudo apt-get install ros-melodic-rosserial-arduino" and then "sudo apt-get install ros-melodic-rosserial"
