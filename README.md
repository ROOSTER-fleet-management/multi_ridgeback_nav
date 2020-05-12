This package consists of launch files to setup a multi ridgeback navigation simulation using the ROS navigation stack.


This package requires installing the ridgeback simulation and navigation pacakges mentioned in the ridgeback tutorials by clearpath robotics (http://www.clearpathrobotics.com/assets/guides/kinetic/ridgeback/simulation.html)

The terminal commands for installing the above mentioned packages: 
```console
sudo apt-get install ros-kinetic-ridgeback-simulator ros-kinetic-ridgeback-desktop
sudo apt-get install ros-kinetic-ridgeback-navigation
```
Also for teleoperation of the robots from terminal, install the teleop_twist_keyboard package using the following command:
```console
sudo apt-get install ros-kinetic-teleop-twist-keyboard
```
Also note that this package requires multi_ridgeback_gazebo package to be installed. This package can be found here https://git.tu-delft.ne-kloud.de/neel.nagda/multi_ridgeback_gazebo.git (If you cannot access it, let me know:- n.n.nagda@tudelft.nl )

Clone the repository into the src folder of your workspace and run catkin_make in the toplevel directory of your workspace. You can then use the following roslaunch command straight out of the box, to start a gazebo simulation with 3 ridgebacks and rviz to command navigation goals. Additionally terminals are also launched to manually operate the robot if it is stuck.
```console
roslaunch multi_ridgeback_nav multi_ridgeback_nav.launch
```
