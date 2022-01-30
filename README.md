# Model-Based-Design-for-Autonomous-Landing-of-Drone-on-a-Moving-Target

>> Flight Controller with Trajectory Planner is developed in one of my Project.Following is the link to navigate ...

>> In the above project consider the Trajectory planner with Minimum Jerk Trajectory i.e 5th Degree Polynomial Equation.

>>The current position of the drone and the target position of the Quadcopter is considered as the input conditions for the trajectory planner. 

>>Which develops the multiple trajectories with starting point at quadcopter location and the ending point of the trajectory as the target position. 

>>Desired positions, velocities and accelerations of drone will be obtained from trajectory planner and flight controller algorithm droves the drone to reach to the target platform. 

>>The following figure shows the layout of the Autonomous block implemented in simscape.

![image](https://user-images.githubusercontent.com/54229744/151695538-a621e906-3568-4545-8efe-4f717ae32b1b.png)

>>In the above figure, we have considered tracking of platform only in straight line i.e., along X- axis i.e. the mobile platform moves along X-axis only.

>>For the autonomous mission block, we are giving inputs of current positions of drone and platform in X-direction and Z- direction. This Autonomous block outputs the initial and final points for the trajectories to be generated. 

>>The subsequent X, Y, Z blocks generates the trajectories and outputs the desired values which needed by Flight controller block.


![image](https://user-images.githubusercontent.com/54229744/151695601-3d789802-5a53-47d7-9dd8-4ca75e7e42bd.png)
       
        Fig : Autonomous Mission Block
        
>>Inside Autonomous Mission block the autonomous mission is planned in to two stages. In first stage the drone has to take off until it reaches to an altitude of 5 meters and in the second stage the tracking and landing mission should be started. 

>>The following shows the simulation window of simscape multibody dynamics.

![alt text](https://github.com/pranavpeddi1/Model-Based-Design-for-Autonomous-Landing-of-Drone-on-a-Moving-Target/blob/main/DroneTrackingLanding_simulink.gif)
