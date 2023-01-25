# Localisation_of_robot
A ROS package using amcl ros package for localization of a two wheeled differential drive robot in a known environment

## Instructions :-

* Clone the repositry
```
git clone https://github.com/Vamsi-IITI/AMCL_AGV.git
```
* You may need to edit amcl launch file , there in rviz node you need to give path of rviz_config.rviz file in your system
* Enter the repositry and make
```
cd AMCL_AGV
catkin_make
```
* Launch my_robot in Gazebo 
```
roslaunch my_robot world.launch
```  
* Launch amcl node  
```
roslaunch my_robot amcl.launch
```  
## Testing :-

The mobile robot can be navigated using two features and hence we have two options to control your robot while it localize itself here:

* Send navigation goal via RViz
* Send move command via teleop package.
```
rosrun teleop_twist_keyboard teleop_twist_keyboard.py
```
Navigate your robot, observe its performance and tune parameters for AMCL.

## Some screenshots : - 
![Screenshot from 2023-01-23 09-51-22](https://user-images.githubusercontent.com/92263050/213965991-d566ad2e-e0cb-4422-b37b-e9ce73d4d827.png)

![Screenshot from 2023-01-23 09-51-50](https://user-images.githubusercontent.com/92263050/213966006-f5260ce2-d513-41e4-8aa6-3dbf93c700d0.png)

![Screenshot from 2023-01-23 09-52-10](https://user-images.githubusercontent.com/92263050/213966017-eee68bfa-e152-485d-ba40-866ea0b13b64.png)
