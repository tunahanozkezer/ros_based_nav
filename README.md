# ROS Based Nav Application


## Project Description
Directory Structure
```
 .catkin_ws                         # Go Chase It Project
    ├── my_robot                       # my_robot package                   
    │   ├── launch                     # launch folder for launch files   
    │   │   ├── robot_description.launch
    │   │   ├── world.launch
    │   ├── meshes                     # meshes folder for sensors
    │   │   ├── hokuyo.dae
    │   ├── urdf                       # urdf folder for xarco files
    │   │   ├── my_robot.gazebo
    │   │   ├── my_robot.xacro
    │   ├── world                      # world folder for world files
    │   │   ├── joy.world
    │   ├── CMakeLists.txt             # compiler instructions
    │   ├── package.xml                # package info
    ├── ball_chaser                    # ball_chaser package                   
    │   ├── launch                     # launch folder for launch files   
    │   │   ├── ball_chaser.launch
    │   ├── src                        # source folder for C++ scripts
    │   │   ├── drive_bot.cpp
    │   │   ├── process_image.cpp
    │   ├── srv                        # service folder for ROS services
    │   │   ├── DriveToTarget.srv
    │   ├── CMakeLists.txt             # compiler instructions
    │   ├── package.xml                # package info                  
    └──
```

## First Terminal
```sh
source devel/setup.sh
roscore
```

## Second Terminal
```sh
source devel/setup.sh
roslaunch src/ball_chaser_robot/my_robot/launch/world.launch
```

## Third Terminal
```sh
source devel/setup.sh
roslaunch src/ball_chaser_robot/ball_chaser/launch/ball_chaser.launch
```


<div style="text-align: center;"> <img src="https://user-images.githubusercontent.com/47686437/168548113-b3cd4206-3281-445b-b7c6-bc0a3251293d.png" alt="Yıldız Technical University Logo" style="width: 5%; height: auto;"> </div> https://youtu.be/cuEREXvIRL0
