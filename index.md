# <span style="color:blue">ECE 5 Final Project</span>
## Team CATalyst (Team 9)
<image src = "catalyst.png" width="480" height="480"></image>


<image src="ECE 5 Poster Team CATalysts.jpg" width="1080" height = "720"></image>

### Group Members
- Luke H.
- Ariel A.
- Tina N.
- MacKenzie F. 

<image src = "team.jpg" width="720" height="480"></image>

### COMPETITION DAY VIDEO
<video src="IMG_2267(1)(1).mov" controls preload width="720" height="480"></video>
**Our ranking is as follows:**
Frequency Sweep: 2nd with 15 rounds \
Drag Race: Made the quarterfinals \
Loop: 14.3 rounds 
### Final Competition Robot
Note we ended up removing the cardboard portions of the light shield due to their flimsiness, and the fact that our pink lightshield that is annotated did a good enough job at blocking out light!
![annotation](https://github.com/user-attachments/assets/3154e582-04bf-4091-ad34-3d5fd487076a)



### Last minute improvements
#### Here are the changes we made in the last week of our project to both the code and hardware.  
We moved our LED strip closer to the photoresistors on the underside of the robot so that the front wheel would not inhibit light from the LEDs. We reprinted our chassis, adding more supports around the motors to prevent the chassis from bending or breaking. In order to give the speed potentiometer more range, we changed the range of the SpRead variable in the line following code from 100 to 200. We also increased the factors on kP and kD, since we were regularly using P and D near the highest position to accommodate the high speed values. Moreover, to accurately see when our robot has finished calibrating, we added an LED directly onto the Arduino and implemented the necessary code to physically signal the calibration.

### So here's a video of our robot following a line
<video src="IMG_9217_1.mov" controls preload width="720" height="480"></video>
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
Our chosen SPID values were a base speed of 55, a P value that was scaled by a factor of 3.0, a I factor scaled by 0.004 and a D scaled by a factor of 0.4. This was done to make sure that P was the most important of the PID Control, while I and D contributed as needed depending on the track. While we didn't collect exact values, for the drag race, we turned out speed up to the max (around 255 speed), and had a bit of P and D, with I at 0. This was because there were very minor turns so we didn't need our robot to make sharp turns. For the loop track, we turned up P and D by about an equal amount on the potentiomers, and upped I a bit as well. S was also chosen to be a more reasonable value. This was done to account for the sharper turns on the loop. Finally, for the frequency sweep track, we turned up P to around the maximum it could be while turning down speed. This was done to ensure the robot could make sharp turns. 

