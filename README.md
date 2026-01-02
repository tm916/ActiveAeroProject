This is a project to investigate the use of control systems to command the actuation of control surfaces on aircraft. This project specifically analyses the effects of elevator deflection on pitch control and was developed as a personal exploration into plant modelling and closed-loop control systems. 
<br> <br>There are two distinct modes of operation:<br> <br>
- A simulated pitch mode where elevator deflection was controlled via a PID loop, taking in the difference between current and target pitch and generating a response. This mode models pitch dynamics, resulting on continually changing error.
- A real pitch mode using IMU derived pitch readings as feedback
<br> <br>  Equipment/parts list:<br> <br>
-  Breadboard and jumper wires
- MPU6050 Accelerometer
- Miuzei MF90 Mini Servo 
- Foam and Cardboard
Software and Libraries:
- Arduino IDE
- Servo.h library
- Adafruit MPU6050 library
<br><br>   Repository strucutre:
- Demonstration Videos - referred to in report
- Plots - referred to in report
- Raw data - logged data used for plot
- Code - contains the Arduino sketches
<br> <br> Explanation of videos: The "Simulated Pitch Demonstration" shows the response of the elevator to a target pitch, the first described mode of operation.
The "Real Pitch Demonstration" shows the actuator response when attempting to maintain a target pitch of 0°, using accelerometer-derived pitch measurements as feedback.
<br> <br>  Notes:<br> <br>
- The Real Pitch sketch contains unused variables originating from the simulated pitch implementation. These do not affect functionality but are retained for development continuity.
- The project prioritises control-system behaviour and implementation realism over aerodynamic fidelity.
- Both sketches may also contain residual functions that were used during testing
Future Work:
- Improved plant modelling including stability derivatives and airspeed dependence
- Higher-resolution actuator control
- Sensor fusion using gyroscope data for improved pitch estimation





