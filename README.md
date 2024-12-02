#Trajectory Tracking for SCARA Robot with Unknown Mass of Links Using Adaptive Slotine Controller

This project involves controlling a SCARA robot arm with 4 links and 4 degrees of freedom (4-DOF) to track a desired trajectory in task space. The robot has unknown link masses, and an indirect adaptive Slotine controller is implemented to estimate these unknown masses and ensure accurate trajectory tracking.

#Problem Description
It is assumed that the mass of each robot link is unknown. For simulation purposes, the method initially considers only one link's mass as unknown (e.g., the fourth link), but the proposed approach is scalable to account for multiple unknown masses.

#Methodology
An indirect adaptive controller is employed to estimate the unknown variables in real-time using adaptive laws. The estimated values are then used in the adaptive Slotine control algorithm to enable the robot to accurately track the desired trajectories in the task space.

#Implementation Details
Model 2 Simulink: Simulates control of the SCARA robot with all link masses known.
Model 4 Simulink: Simulates control when the fourth link's mass is unknown. The unknown mass is estimated online using the adaptive law block, and the results demonstrate both the accuracy of mass estimation and the robot's ability to track the desired path in the task space.
Figures for Each Simulation: Generate 3D plots illustrating the robot's path in the task space.

##Requirements
MATLAB R2018a or newer
