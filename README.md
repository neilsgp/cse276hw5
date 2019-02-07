First run dependent services
```
$ roscore
$ roslaunch turtlebot_bringup minimal.launch
$ roslaunch astra_launch astra_pro.launch
```

Run `cmvision`,
```
$ roscd cmvision
$ rosparam set /cmvision/color_file /home/turtlebot/colors.txt
$ rosrun cmvision cmvision image:=/camera/rgb/image_raw
```

Run the project using
```
$ cd ~/catkin_ws/src/where_is_blob/src
$ python color_tracker.py
```

![Alt text](/images/FSM.jpeg?raw=true "FSM Diagram")
