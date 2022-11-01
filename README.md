# Mobile robot in gazebo environment

![Overview](image.png)]

## Build Instructions
1. Make sure you have the following installed:
   - [ROS](http://wiki.ros.org/ROS/Installation)
   - Cmake
   - gcc/g++
   - Git
2. Clone the project using `git clone < >`
3. Open build folder in terminal
4. Build with cmake `cmake ../ && make`
5. Add the build folder to the Gazebo plugin path: 
`GAZEBO_PLUGIN_PATH=${GAZEBO_PLUGIN_PATH}:<path_to_build_folder>`.
6. Go back to world folder.
8. Launch Gazebo world `gazebo world` or `gazebo world --verbose` for debug

## Structure
```
.Project             # Build My World Project 
├── model                          # Model files 
│   ├── House
│   │   ├── model.config
│   │   ├── model.sdf
│   ├── myrobot
│   │   ├── model.config
│   │   ├── model.sdf
├── script                         # Plugin files 
│   ├── welcomeworld.cpp
├── world                          # World files
│   ├── world.world
├── CMakeLists.txt
└── build   
```
