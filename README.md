# Aniruddha Bhattacharjee

## Research Interests
- **Robotics**: Biomimetic and bio-inspired robotics, coordinated control of robotic swarm, haptics and bionic prosthetics
- **Control**: Computing and hardware for control applications, coordinated control of multi-agent systems, optimization and communication for control
- **Dynamical Systems**: Nonlinear systems and chaos

## Contents
- [Projects](#projects)
- [Student Team Projects](#student-team-projects)


## Projects

#### Final semester Major Project (Undergraduate thesis)
- **_Human Arm Motion Capture Using IMU Sensors_**
  - Motivation: To develop a computationally cheaper alternative to computer vision based human body motion tracking technology, by utilising IMU sensors. Develop something which can also be used as a means to further advancements in prosthesis control and human-computer interaction.
  - Methodology:
    - Place IMU sensors (accelerometer + gyroscope + magnetometers) on each segment of the human arm (upper arm, forearm & hand). 
    - Develop necessary mounts and embedded electronics to place and interface sensors on the arm.
    - Use a quaternion based sensor fusion technique to estimate orientation of each segment individually. Rotate each segment’s quaternion using the rotation quaternion calculated for the previous segment. (Rotation quaternion calculated from upper arm sensor data used to reposition coordinate system of forearm)
    - Develop embedded firmware for Arm cortex-m4 based device for sensor interface and communication. Develop a python based 3D render of the human arm for visualization.

![Concept1](/assets/media/concept1.png)     ![layout1](/assets/media/layout1.png)

#### 7th Semester Research Project
- **_Fractal Analysis of Electric Streamers_**
  - Motivation: To better understand the dynamics of an electric streamer occurring during dielectric medium breakdown or natural lightning, in order to assess the amount of charge involved and determine ways to minimize damage to the electrical equipment involved.
  - Highlights:
    - Determination factors affecting streamer pattern geometry in a high voltage electric discharge experimental setup with a liquid dielectric medium. 
    - Calculation of fractal dimensions using box-counting method, for different voltage magnitudes and polarity
    - Worked on developing a mathematical model of the electric streamers, assuming the system to be nonlinear due to the coupling of electromagnetic forces due to charge build up and travelling charged particles.


#### 5th & 6th Semester Project
- **_Flight Control System for a Quadrotor Drone_**
  - Motivation: To develop an intuitive understanding of the mathematics and programming involved in designing control systems for a quadrotor drone.
  - Highlights:
    - Learned about the dynamics and developed free-body diagrams of the drone to form transfer functions relating orientation angles with forces.
    - Worked on orientation estimation using quaternions and complementary filter, from IMU data
    - Developed a simple PI based attitude control and PID based altitude control algorithm, manually selecting gains for each control branch.
    - Programmed an Arm cortex m4 device (Teensy 3.6 with bare-metal firmware) for sensor interface, orientation estimation & control, and ESC calibration.
    - Tested on a X-Frame 14-inch Quadcoptor frame


#### 4th Semester Seminar
- **_Python for Electrical Engineering: 3D visualization of electric and magnetic fields due to charged objects or current elements_**
  - Motivation: To develop interactive 3D plots of electric & magnetic fields due to various geometries of charges objects of current elements to aid learning in course- EE4xx Engineering Electromagnetics.
  - Highlights:
    - Wrote Python scripts for different plotting electric fields of charged objects with different shapes (Sphere, infinite plane, point charges, etc.)
    - Used Python modules such as Numpy and Matplotlib for Finite-element Analysis based calculations and 3D plotting.

## Student Team Projects

#### Nirma University _AUVSI - SUAS_ Team
- **_Design of a Two-wheeled UGV for payload delivery to designated drop zone_**
  - Objective: One of the objectives of the SUAS competition is to airdrop a UGV (from the primary UAV), to deliver a payload (usually a 250ml bottle), to a designated location which is different from the airdrop point. Thus, a UGV capable of surviving uncertainties and rough terrain had to be developed. The design should also focus on how to avoid the possibility of the UGV toppling while landing which can render it immobile.
  - Highlights: 
    - Investigated a design similar to NASA JPL’s PUFFER Bot.
    -	Worked on developing the control systems for steering, position change, and motion, based on data from GPS, proximity and IMU sensors.
    -	Studied various wheel geometry to aid movement in rock/gravel and sandy terrain.
    -	Worked on interfacing low power RF-communication module to communicate with the aerial UAV.

#### Nirma University **_S.A.E. E-BAJA_** Team
- **_Development of Maintenance Probe for Testing & Evaluating the Mechanical Integrity of an Electric All-Terrain Vehicle (ATV) Wiring Harness_**
  - Objective: The Electric-ATV would be subjected to extreme terrain, thereby requiring the low-voltage vehicle control wiring harness, to be tightly secured and monitored for disconnection faults. Thus, the development of an electronic probe, which can connect to a port on the vehicle, in order to assess the mechanical integrity of the wiring harness.
  - Highlights:
    - The concept is based on sending and receiving electrical signals through the said wiring harness, while the ATV is not energized.
    - Designed electronic circuits and embedded systems for the vehicle port and a hand-held inspection device.
    - Integrated an LCD display in the hand-held inspection device, along with Bluetooth enabled telemetry for sending fault related data to a phone.
    - Project based on Arduino Uno (Atmega 328pu) and the HC-05 Bluetooth module 












 
![sci-fi-city-pixelart](/assets/media/sci-fi-pixel1.gif)

