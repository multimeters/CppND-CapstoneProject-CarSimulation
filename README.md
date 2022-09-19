#  Car Simulation with MPC Controller 

This code implements a car simulator. And implements MPC(Model Predictive Control) algorithm to control the simulated car to fllow a trajectory.

<p align="center">
    <img src="mpc.gif" width="400"/>
</p>

## DEPENDENCIES

This software is built on the Robotic Operating System (ROS), which needs to be installed first.

* ROS : Noetic or Melodic
  * How to install ROS : [Neotic](http://wiki.ros.org/noetic/Installation/Ubuntu) , [Melodic](https://wiki.ros.org/melodic)

## HOW TO RUN

```
1. ./install_tools.sh
2. catkin_make -j1
3. source devel/setup.bash
4. roslaunch mpc_car simulation.launch
```

## HOW TO TURN PARAMETERS

```
./src/mpc_car/config/mpc_car.yaml -> mpc parameters
./src/car_simulator/config/car_simulator.yaml -> initial states (in simulation)
```
## RUBRIC POINTS
1.CRITERIA-The project reads data from a file and process the data, or the program writes data to a file. In "./src/mpc_car/launch/simulation.launch" line 11. The <rosparam> tag enables the use of rosparam YAML files for loading and dumping parameters from the ROS Parameter Server. It can also be used to remove parameters. The <rosparam> tag can be put inside of a <node> tag, in which case the parameter is treated like a private name. 