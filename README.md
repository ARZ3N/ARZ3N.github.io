## Aniruddha Bhattacharjee

### [<< GitHub >>](https://github.com/ARZ3N)

## Contents
- [Areas of Interest](#areas-of-interest)
- [Projects](#projects)
- [Publications](#publications)
- [Student Team Achievements](#student-team-Achievements)

## Areas of Interest
### Control Systems Design, Sensors & Actuators, Robotic Locomotion & Control
### Systems Level Programming, Embedded Systems
### Nonlinear Systems, Computational Sciences


## Projects
- ### RTOS integrated Human Arm Movement Tracking with Haptic Feedback
  _motivation_: To integrate extended sensory feedback for an existing motion tracking system, to built it as a human-machine interface technology.
  
- ### Linear Optimal COntrol of Two Wheel Self-Balancing Robot
  _Motivation_: The Linear Quadratic Regulator offers a great way to associate weights with states and inputs to optimize system performance around a quadratic cost function. With some idea and hit-and-trail success, weights can be chosen such that desired system performance (overshoot, rise time, settling time) is achieved. But what if a method of weight selection exists which can provide a formal method to achieving this?
  
- ### ** Estimating Airfoil Aerodynamic Lift Coefficient Using Neural Networks
  _Motivation_: Usually, to calculate lift coefficient of a given airfoil, software (such as XFOIL) use iterative methods to converge to a value by considering differential equations describing air flow around an object. But quite often, for some airfoil geometries, the software is unable to converge at a 'good' value or does not converge at all.
    Neural Networks being excellent function approximators, an idea was put to test- to make a neural network learn about the math and physics behind airflow around a 2D geometry, ultimately predicting the lift coefficient of the given airfoil.
  - Designed a deep learning model with 2x Convolution layers with RELU activation function, an Input Layer, 1x fully dense layer and an output layer.
  - Airfoil shapes (2D crossectional shape) is considered as 31 pairs of 2D cartesian cordinates forming the boundary of the airfoil. Other details involve flight condition with a viscuous flow Reynold's number of 1.3e7 and subsonic flight conditions of Mach 0.3. Angle fo attack would vary from -2 deg to 10 deg.
  - Used UIUC's Airfoil Datasite to access 1621 airfoil shape data. Created C and Shell scripts to standardize coordinate listing format.
  - Used XFOIL solver for gathering lift coefficient data for available. Created C and Powershell scripts to parse through files and check convergence failure in data files associated with all 1621 airfoil shapes. XFOIL would often fail to converge for certain airfoil shapes with the given flight conditions.
  - Trained the neural net for 1600 epochs. Deep learning model built and trained with Tensorflow-Python.
  - Achieved lift coefficient estimation accuracy of 98.63% and the neural network is also able to estimate lift coefficients of arbitrary airfoil shapes (completely new shapes).

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

## Publications

- ### Bhattacharjee, A., Bhatt, C. (2021). Human Arm Motion Capture Using IMU Sensors. 1st International Conference on Smart Ennery and Advancements in Power Technology (Track- Biomedical Instrumentation and Applied Sciences), National Institute of Technology, Jamshedpur. Springer Lecture Notes in Electrical Engineering.
Conference Publication Link: [DOI: https://doi.org/10.1007/978-981-19-4975-3_63](https://doi.org/10.1007/978-981-19-4975-3_63)

## Student Team Achievements
- ### National Winners, SAE Electric BAJA Championship, INDIA - 2019

![EBAJA_Vehicle1](/assests/media/SAE_BAJA_2019.JPG)



##### Thank You! ^
![urban_sprawl_dusk](/assets/media/giphy_dusk_japan_city.gif)


