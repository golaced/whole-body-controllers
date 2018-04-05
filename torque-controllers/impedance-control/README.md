## Module description

This module implements a simple torque control balancing strategy. The robot is assumed to have its `base_link` fixed on a pole.

Input torques are the `gravity toruqes` which allow to perform **gravity compensation**. Optionally, it is also possible to move each controlled joint in order to track a desired joints trajectory.

### Compatibility

The repository contains the Simulink model `impedanceControl.mdl`, which is generated by using Matlab R2016b.

### Supported robots

Currently, supported robots are: `iCubGenova04`, `iCunGenova02`, `icubGazeboSim`, `iCubGazeboV2_5`.

## Module details

### Configuration file

At start, the module calls the initialization file initImpedanceControl.m. Once opened, this file contains some configuration variables. Please follow the instruction inside the script to properly configure your simulation.

### Robot and demo specific configurations

The gains and references for a specific robot (specified by the variable YARP_ROBOT_NAME) or a specific demo can be found in the folder `app/robots/YARP_ROBOT_NAME`.