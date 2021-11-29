# Aniruddha Bhattacharjee

## Research Interests
- **Robotics**: Biomimetic and bio-inspired robotics, coordinated control of robotic swarm, haptics and bionic prosthetics
- **Control**: Computing and hardware for control applications, coordinated control of multi-agent systems, optimization and communication for control
- **Dynamical Systems**: Nonlinear systems and chaos

## Projects

#### Final semester Major Project (Undergraduate thesis)
- **_Human Arm Motion Capture Using IMU Sensors_**
  - Motivation: To develop a computationally cheaper alternative to computer vision based human body motion tracking technology, by utilising IMU sensors. Develop something which can also be used as a means to further advancements in prosthesis control and human-computer interaction.
  - Methodology:
    - Place IMU sensors (accelerometer + gyroscope + magnetometers) on each segment of the human arm (upper arm, forearm & hand). 
    - Develop necessary mounts and embedded electronics to place and interface sensors on the arm.
    - Use a quaternion based sensor fusion technique to estimate orientation of each segment individually. Rotate each segment’s quaternion using the rotation quaternion calculated for the previous segment. (Rotation quaternion calculated from upper arm sensor data used to reposition coordinate system of forearm)
    - Develop embedded firmware for Arm cortex-m4 based device for sensor interface and communication. Develop a python based 3D render of the human arm for visualization.

![Concept1](/assets/media/concept1.png) ![layout1](/assets/media/layout1.png)






 
![sci-fi-city-pixelart](/assets/media/sci-fi-pixel1.gif)

