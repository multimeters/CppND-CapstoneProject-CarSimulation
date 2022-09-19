#  Car Simulation with MPC Controller 

This code implements a car simulator. And implements MPC(Model Predictive Control) algorithm to control the simulated car to fllow a trajectory.

<p align="center">
    <img src="mpc.gif" width="400"/>
</p>

## Dependencies

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
