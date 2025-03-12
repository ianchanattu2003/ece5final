# <span style="color:blue">ECE 5 Final Project</span>
## Team CATalyst (Team 9)
<image src = "catalyst.png" width="480" height="480"></image>
### Group Members
- Ariel A. 
- Luke H.
- MacKenzie F.
- Tina N.

<image src="ECE 5 Poster Team CATalysts.jpg" width="1080" height = "720"></image>

### So here's a video of our robot following a line
<video src="IMG_9217_1.mov" controls preload width="720" height="480"></video>

### Last minute improvements
#### Here are the changes we made in the last week of our project to both the code and hardware.  
We moved our LED strip closer to the photoresistors on the underside of the robot so that the front wheel would not inhibit light from the LEDs. We reprinted our chassis, adding more supports around the motors to prevent the chassis from bending or breaking. In order to give the speed potentiometer more range, we changed the range of the SpRead variable in the line following code from 100 to 200. We also increased the factors on kP and kD, since we were regularly using P and D near the highest position to accommodate the high speed values. Moreover, to accurately see when our robot has finished calibrating, we added an LED directly onto the Arduino and implemented the necessary code to physically signal the calibration.


### Assembled Robot Prototyping

This is the assembled robot prototype as of 2/28/2025. 


#### Side View
<image src = "sideview.jpg" width="720" height="480"></image>
#### Top View
<image src = "topview.png" width="720" height="480"></image>

#### Bottom View 
<image src = "bottomview.jpg" width="720" height="480"></image>





### PID Control Explained 

PID control stands for "Proportional, Integral, Derivative" Control and it is a feedback based control loop that responds to error in order to manage the control of an object. In our case we use PID for our robot in order to keep it following the black line that makes up the track being followed. 
Our chosen PID values were:
- Circle Track:
- Wave Track:
- Drag Race:
  
Our chosen speed is:
- Circle:
- Wave:
- Drag Race:

We chose these speed values because: 
