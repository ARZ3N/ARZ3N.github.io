## Aniruddha Bhattacharjee

### [<< GitHub >>](https://github.com/ARZ3N)

## Contents
- [Areas of Interest](#areas-of-interest)
- [Projects](#projects)
- [Student Team Projects](#student-team-projects)
- [Publications](#publications)
- [Ongoing Projects](#ongoing-projects)
- 
## Areas of Interest
| Control Systems Design | Robotics | Computing & Embedded |
|     :--------------:   | :-----:  | :----------------:   |
|Physics & System Modelling|Motion Control| Microcontroller Firmware|
|Linear Systems Analysis | Sensors | Real Time Operating Systems |
| PID Control | Mechatronics | Systems level Programming |
| Full-State Feedback | Hardware Design | Computational Methods |
| LQR Optimal Controllers | Bio-inspired methods | High Performance Computing |
| Root Locus Techniques | Human-Machine Interaction |
| Nonlinear Systems | Sensor Fusion |
| State Estimation |

## Projects

#### Final semester Major Project (Undergraduate thesis)
- ### **_Human Arm Motion Capture Using IMU Sensors_**
  - _Motivation_: To develop a computationally cheaper alternative to computer vision based human body motion tracking technology, by utilising IMU sensors. Develop something which can also be used as a means to further advancements in prosthesis control and human-computer interaction.
  - Methodology:
    - Sensor interface and Signal processing:
     + Sensor used: Invensense MPU 9250 Accelerometer + Gyroscope + Magnetometer
     + Implemented FIR/Moving Average Filter for removing noise due to sudden shifts in motion over a short period of time.
     + I2C communication channel between sensor and microcontroller.
    - Used a quaternion based sensor fusion technique to estimate orientation of each segment individually. Rotate each segment’s quaternion using the rotation quaternion calculated for the previous segment. (Rotation quaternion calculated from upper arm sensor data used to reposition coordinate system of forearm).
    - Develop necessary mounts and embedded electronics to place and interface sensors on the arm.
    - Develop embedded firmware for Arm cortex-m4 (MK66FX1M0) device for sensor interface and communication. Develop a python based 3D render of the human arm for visualization.

     ![Concept1](/assets/media/concept1.png)  ![layout1](/assets/media/layout1.png)

      Development Code Source: [imu-arm-motion-capture--GitHub](https://github.com/ARZ3N/imu-arm-motion-capture)
      
      Conference Publication Link: [DOI: https://doi.org/10.1007/978-981-19-4975-3_63](https://doi.org/10.1007/978-981-19-4975-3_63)
      
#### 8th Semester Course Project: CE006 Operating Systems
- ### **_Development of a custom Command Line Interface_**
  - _Motivation_: To understandthe internal working of a command-line interface, with primary emphasis on OS-based shells, like BASH, and how these make use of processes to execute commands.
  - Developed a simple BASH-like CLI capable of invoking some custom commands and interact with OS functions.
  - Learned to use the POSIX "pthreads.h" library and how to create processes and child-process management.
  - Developed understanding of the shell program structures including input parsing, validation, execution blocks, etc.

      Project Source: [SeaShell -- GitHub](https://github.com/ARZ3N/Cshell)
      
#### 7th Semester Research Project
- ### **_Fractal Analysis of Electric Streamers_**
  - Motivation: To investigate the dynamics of an electric streamer occurring during dielectric medium breakdown or natural lightning, in order to assess the amount of charge involved and determine ways to minimize damage to the electrical equipment involved. Owing to its highly branched and random formations, there must be some chaotic interplay of different factors which lead to such erratic electromagnetic behaviour.
  - Summary:
    - Determination factors affecting streamer pattern geometry in a high voltage electric discharge experimental setup with a liquid dielectric medium. 
    - Calculation of fractal dimensions using box-counting method, for different voltage magnitudes and polarity.
    - Worked on developing a mathematical model of the electric streamers, assuming the system to be nonlinear due to the coupling of electromagnetic forces due to charge build up and travelling charged particles.


#### UG Mini Project
- ### **_Flight Control System for a Quadrotor Drone_**
  - Motivation: To develop an intuitive understanding of the mathematics and programming involved in designing control systems for a quadrotor drone.
  - Highlights:
    - Designed a Roll-Pitch controller for an X-type multi-rotor drone with PID feedback control using MATLAB/Simulink model based on free-body diagram derived system dynamics.
    - Programmed an Arm-Cortex-m4 based MCU (STM32F411VET6) to implement moving data filters, sensor fusion and control law implementation along with Timer control for BLDC motor ESC drive signal and UART peripherals for data transfer to host & SPI SD card data logging.
    - Implemented a quaternion based orientation tracking algorithm (after facing problems using Euler angle based method).
    - Attempted a Hardware-In-Loop (HIL) simulation testing method using Python scripts to run C-code and plot data using python modules- Matplotlib, Numpy.


#### 4th Semester Seminar
- ### **_Python for Electrical Engineering: 3D visualization of electric and magnetic fields due to charged objects or current elements_**
  - Motivation: To develop interactive 3D plots of electric & magnetic fields due to various geometries of charges objects of current elements to aid learning in course- EE4xx Engineering Electromagnetics.
  - Highlights:
    - Developed Python scripts for different charge distributions and standard charged objects such as Sphere, infinite plane, point charges and custom charge distributions also.
    - Used Python modules such as Numpy and Matplotlib for Finite-element Analysis based calculations and 3D plotting.

## Student Team Projects

#### Nirma University _AUVSI - SUAS_ Team
- ### **_Design of a Two-wheeled UGV for payload delivery to designated drop zone_**
  - Objective: One of the objectives of the SUAS competition is to airdrop a UGV (from the primary UAV), to deliver a payload (usually a 250ml bottle), to a designated location which is different from the airdrop point. Thus, a UGV capable of surviving uncertainties and rough terrain had to be developed. The design should also focus on how to avoid the possibility of the UGV toppling while landing, which may render it immobile.
  - Highlights: 
    - Worked on developing control firmware for a 2-wheel differential drive rover and developed embedded systems for sensor interface, drive control and motor and servo control.
    - Designed bio-inspired wheel geometry and traction surface, for the rover to have better grip on rocky/gravel based terrain.

#### Nirma University **_S.A.E. E-BAJA_** Team
- ### **_Development of Maintenance Probe for Testing & Evaluating the Mechanical Integrity of an Electric All-Terrain Vehicle (ATV) Wiring Harness_**
  - Objective: The Electric-ATV built for the S.A.E. E-BAJA competition would be subjected to extreme terrain, thereby requiring the low-voltage vehicle control wiring harness, to be tightly secured and monitored for disconnection faults. Thus, the development of an electronic probe, which can connect to a port on the vehicle, in order to assess the mechanical integrity of the wiring harness.
  - Highlights:
    - Developed an electronic probe to check proper connection of wires inside vehicle cockpit and identify and locate loose wire faults, with the capability of sending results to a Bluetooth-enabled phone.
    -	Designed hardware and embedded C++ software (Arduino) for GPIO, UART peripherals and Bluetooth (HC-05) sensor interface.
    -	Also involved designing the PCB layout, soldering components onto board and testing.

## Publications

- ### Bhattacharjee, A., Bhatt, C. (2021). Human Arm Motion Capture Using IMU Sensors. 1st International Conference on Smart Ennery and Advancements in Power Technology (Track- Biomedical Instrumentation and Applied Sciences), National Institute of Technology, Jamshedpur. Springer Lecture Notes in Electrical Engineering.
Conference Publication Link: [DOI: https://doi.org/10.1007/978-981-19-4975-3_63](https://doi.org/10.1007/978-981-19-4975-3_63)

## Ongoing Projects
#### Course Project (ASU): EEE 511 Artificial Neural Computation
- ### **_Learning Aerodynamics: Estimating Arifoil Lift Coefficients using Neural Netowrks_**
  - Motivation: Neural Networks are often referred to as “Universal Approximators”, and rightfully so as these constructs have the ability to generate and fit mathematical curves of varying linearity and degree. This project intends to demonstrate how neural networks can be made to learn the mathematical function governing the aerodynamics of an Airfoil, and give estimates related to performance variables such as Lift coefficient. Since the mathematical relation between different shape-defining variables, fluid characteristics and the aerodynamic performance variables is nonlinear and complex, conventional methods employ computational fluid dynamics and Finite-element analysis based methods to accomplish the same thing. This project is far from a replacement for the reliable and true approach to solving this problem, which is the conventional way; but is a great demonstration of the learning capability of neural networks and its potential to become better at solving this problem, in the future.
  - Software / Languages / tools being used currently:
 C, Python, Tensorflow, Bash scripting, XFoil


- ### **Using Python for Hardware-In-Loop (HIL) Simulations of Embedded Control Systems**
Learning Automation and simulation workflows to design Python System modelling library for HIL simulations that can work with embedded targets.









 
![urban_sprawl_dusk](/assets/media/giphy_dusk_japan_city.gif)

##### Thank You! ^
