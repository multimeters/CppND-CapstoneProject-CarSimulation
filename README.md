#  Car Simulation with MPC Controller 

This code implements a car simulator. And implements MPC(Model Predictive Control) algorithm to control the simulated car to fllow a trajectory.

<p align="center">
    <img src="mpc.gif" width="400"/>
</p>

## Dependencies

This software is built on the Robotic Operating System (ROS), which needs to be installed first. 

* ROS : Noetic or Melodic
  * how to install ROS : [Neotic](http://wiki.ros.org/noetic/Installation/Ubuntu) , [Melodic](https://wiki.ros.org/melodic)

## HOW TO RUN

```
./install_tools.sh
catkin_make -j1
source devel/setup.bash
roslaunch mpc_car simulation.launch
```

## HOW TO TURN PARAMETERS

```
./src/mpc_car/config/mpc_car.yaml -> mpc parameters
./src/car_simulator/config/car_simulator.yaml -> initial states (in simulation)
```

## Theory

### Linearize  Nonlinear Model

<p align="center">
  <img src="equation1.png" width="800"/>
</p>

### Constrained Quadratic Problem
 
<p align="center">
   <img src="equation2.png" width="800"/>
</p>

### Delay Compensation

<p align="center">
  <img src="equation3.png" width="800"/>
 </p>

# CppND-CapstoneProject-CarSimulatorr
