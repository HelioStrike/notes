
# Week 1 - 3

## Week 1 - Requirements for Autonomy

### Levels of Autonomous Capabilities

- Level 0 - No automation

- Level 1 - Driving Assistance 
    Lateral or Longitudinal control

- Level 2 - Partial Driving Automation 
    Lateral and Longitudinal control

- Level 3 - Conditional Driving Automation 
    Includes automated object and event detection and response. 
    
- Level 4 - High Driving Automation
    Handles emergencies autonomously, driver can entirely focus on other tasks.

- Level 5 - High Driving Automation
    Can drive in any environment and weather.

### Perception

Making sense of the environment.
- Identification
- Understanding motion
to inform our driving decisions.

Things to percieve:
- Static objects
- Dynamic objects
- Ego localization (position, velocity, etc.)

Challenges:
- Robust detection and segmentation
- Sensor uncertainty
- Occlusion, reflection
- Illumination, lens flare
- Weather

### Planning

Decisions:
- Long term - How to navigate between 2 places
- Short term - Can I switch to that lane?
- Immediate - Accelerate or brake

Reactive Rule based planning: Involves decision trees.

Predictive planning: Make predictions about other objects.

## Week 2 - Self-Driving Hardware and Software Architectures

### Sensors for perception

- Exteroceptive - external
- Proprioceptive - internal

Comparison metrics:
- Resolution
- Field of view (FOV)
- Dynamic range

Exteroceptive Sensors:
- Camera
- LIDAR - number of beams, points per second, rotation rate, FOW
- RADAR - range, FOV, position and speed accuracy
- SONAR - range, FOV, cost

Proprioceptive Sensors:
- GPS - measures position, velocity, rotation, etc.
- IMU - "
- Wheel odometry - tracks speed

Localization map - Captures difference between 2 LIDAR maps
Occupancy grid - Identifies static objects in a map
Detailed roadmap - Contains info of lanes, and any other road elements

## Week 3 - Safety

Analytical safety - Ensures system works in theory and meets safety requirements found by hazard assessment.

Data driven safety - Guarantee due to the fact that syystem has performed autnomously without fail on the roads for a very large number of kms.