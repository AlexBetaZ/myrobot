## go_chase_it ##
  This is robot project. In this project, a robot and a white ball place in a predefined environment. The robot will processes its camera image to locate the position of the white ball. The robot will autonomously changes its orientation and heads toward the white ball. 
### Configuration ###
- Ubuntu 16.04.6 xenial
- Gazebo 7.15.0
- ROS kinetic kame
### Installation ###
  Firstly, creat a workspace:
```
  mkdir -p <YOUR_CURRENT_DIRECTORY>/catkin_ws/src
  cd catkin_ws/src
  catkin_init_workspace
```
  Secondly, clone the repository:
```
  git clone https://github.com/huanalexzhao/go_chase_it.git
```
  The last, build the project:
```
  cd .. # go to the catkin_ws/ directory
  catkin_make
```
### Run the project ###
```
  source devel/setuo.bash # make sure you in the catkin_ws/ directory
  roslaunch my_robot world.launch
```
  Open a new terminal by ctr+shift+T:
```
  source devel/setup.bash
  roslaunch ball_chaser ball_chaser.launch
```
