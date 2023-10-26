# Setup Tabitha (Competition Bot 2022-2023)

In order to setup Tabitha you have to follow a couple steps
1. Plug in a 11.1 V LiPo battery into tabitha (this is supposed to be different than the terrence 11.1V green lipo, it is black and should fit into the 3d print battery holder)
2. Make sure that the emergency stop (e-stop) has a battery pack attached
3. Make sure the e-stop is **not** pressed

## Wired Control
1. Plug in the robot to a monitor, mouse, and keyboard
2. Open up a terminal and run the following commands:
```
cd Documents/2022TabithaBot/otherFiles
bash ./startManualControl.bash
```

## Wireless control
1. Plug in the control station jetson into a monitor, mouse, keyboard
2. Plug in the router (team32 is the name of the network)
make sure the control station is connected to the team32 router NOT eduroam or something else
3. Make sure the robot is powered and turned on (estop not pressed)
4. open terminal and run the following command 
```
cd Documents/2022-control-station/otherfiles
bash ./startWirelessControl.bash
```
5. Connect to the competition robot with the following command
```
ssh unllunar@rmccompbot
```
6. Start the robot with ROS and controls by running the following 
```
bash ./Documents/2022-control_station/otherfiles/startControl.bash
```