# Setup Terrence (Test Bot)

In order to setup Terrence you have to follow a couple steps
1. Plug in a 11.1 V LiPo battery into terrence
2. Make sure that the emergency stop (e-stop) has a battery pack attached
3. Make sure the e-stop is **not** pressed

## Remote Setup (not plugged into terrence, using control station)
1. Run the following command (will open another terminal window do **not** touch it)
TODO: make sure below lines work
```
bash ./Documents/2022-control_station/otherfiles/startControl.bash
```
2. On the new terminal, run the following
TODO: make sure the rmctestbot thing is right
```
ssh unllunar@rmctestbot
bash ./Documents/2022-terrence/otherfiles/startRemoteBot.bash
```

## Wired Setup
1. Plug in the monitor, joystick, mouse into the test robot
3. pull up a terminal and run the following command:
```
cd Documents/2022-terrence/otherfiles
bash ./startManualControl.bash
```