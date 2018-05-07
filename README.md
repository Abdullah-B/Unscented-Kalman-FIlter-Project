# Unscented Kalman Filter Project Starter Code
Self-Driving Car Engineer Nanodegree Program

In this project utilize an Unscented Kalman Filter to estimate the state of a moving object of interest with noisy lidar and radar measurements. Passing the project requires obtaining RMSE values that are lower that the tolerance outlined in the project rubric.

## Basic Build Instructions

1. Clone this repo.
2. Make a build directory: `mkdir build && cd build`
3. Compile: `cmake .. && make`
4. Run it: `./UnscentedKF` Previous versions use i/o from text files.  The current state uses i/o
from the simulator.

## Changes and Results

as per what was requested for this project the following files were modified to fullfil the requirments of the project

   ### 1 : UKF.cpp
   
Frist we adjusted the value of the Process noise standard deviation longitudinal acceleration from 30 to 1 m/s^2
as well as the standard deviation yaw acceleration from 30 to 0.5rad/s^2

And then finished all the initializations indicated in the comments

   ### 2: tools.cpp

Aded the code to calculate the RMSE inside : VectorXd Tools::CalculateRMSE(const vector<VectorXd> &estimations,
                                                                           const vector<VectorXd> &ground_truth)
    
   ### The resutls were
    
   ![Screenshot](/OutPut&Results/ResultPNG.PNG)
   
   and the Matrix outputs are documented inside OutPut&Results/ OUTPUT.txt
   