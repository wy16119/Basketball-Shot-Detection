# Shot Detection
### L.J. Brown, Zihao Mao, Preston Deason, Austin Wiedebusch
## AI Basketball Shot Detection and Analysis
Our program is able to detect when a shot occurs and extrapolate the balls flight from captured data. The program calculates the balls initial velocity and launch angle. The program is able to determine the balls flight perpedicular to the camera plane (The z axis). The program is also able to detect when the balls flight is interupted by another object and will drop those data points. In the case of unstable video, the program currently calculates the balls trajectory relative to the person shooting the ball. In the future we will impliment more accurate stabilization techniques. Additional note: the program currently requires at least 2 data points of a shot to be captured to perform its anylisis.

## Tracking and anylisis performed on unstable video
![Unstable Video](shot_1.gif)
### Output world coordinates
![world coordinates](shot_1_trajectory_extrapolation_points_v1.png)

### Tracking and anylisis performed on interrupted shot by person
![Shot with missing datapoints](shot_2.gif)
### Trajectory Extrapolation
[Trajectory](shot_2.png)
### Output world coordinates
![world coordinates](shot_2_trajectory_extrapolation_points_v1.png)

### Tracking and anylisis performed on interrupted shot by object
#### Successful anylisis of shot angle 
![Hits net piecewise linear regression](shot_16.gif)
### Output world coordinates
![world coordinates](shot_16_trajectory_extrapolation_points_v1.png)
### (Adjust Trajectories For Shot Angle/Camera Depth)
![Depth Adjustment](depth_adjustment_shot_16.png)
