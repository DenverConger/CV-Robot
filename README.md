 [ <font size="30"> How to Guide</font>](Tutorials/Start.md)

# Planning
The current plan is to use Object detection with a camera above to have a robotic arm organize objects by either shape or color into certain areas avalible to it.

# Steps

##### 1. Robotic arm design 
done (kind of) I need to finish 3d printing it
  <br />


##### 2. End effector design (how the robot interacts with the world)
done (kind of)
  <br />
3. Object recognition
done by using  machine learning algorithms for computer vision. (prob a neural network)
  <br />
4. Task planning
How do we want to help the robot determine what its actions should be?
This could be as simple as some if statements or as complex as a large neural network.
  <br />
5. Motion planning
Motion planning is planning motions of the robotic arm while still followinng and listeningg to dynamic and safety constraints provided. 
Planning Algorithms by Steven LaValle. is a book the internet constantly reccomends (i am too cheap to but it tho right now) 
It needs to determine optimal paths AND trajectories which are similar to paths but include derivatives like position or velocity or acceleration
and than it has to complete the tasks we want of it safely.
I think a good example would to pick up a small red box we give it. It has to carefully move over to pick it up, and than puick it up. 
and than move it all while avoiding other things and being CAREFUL AND SAFE
  <br />

6. Low level control
(ah yes... I think this will prob be THE BEAST)
 low level controller (arduino) determines the actual (not simulated) values to send to the motors. Many people use an in-between controller board to convert
 these planned trajectories into motor forces and the low level controller converts them to the values needed. Basically we need to figure out how to get the rasbperry pi 
 and an arduino to tlak as if they were best friends
 We may also want to add some feedback control like some simple sensors within the arm to help get an accurate estimate of the state of the robot arm. The camera could do this by istelf 
 but i have much more preactice with simple resistance sensors. This is really to make sure the robot isnt being stupid

## Neural Networks

    - https://www.youtube.com/watch?v=aircAruvnKk&t=2s 

    - LEARN THIS TUTORIAL
        - https://www.tensorflow.org/tutorials/keras/classification
        
## Machine Learning
https://www.sololearn.com/learning/1094


# Things to get
1. Figure out how to do a camera stand
2. zip ties (Cable Management)


# SHORT TERM PLAN
1. Learn ROS in more detail
2. Get a servo to be controlled with solely the ROS and (arduino)
3. Learn machine learning programming
4. Neural network understanding
5. begin to tackle individual parts

**REMINDER**

    THIS IS A MASSIVE PROJECT THAT WE AM ACTIVELY WORKING ON
    please understand that this is a long term project (like potentially upwards of a year)

    I want to use this to fully understand every facet of higher robotic 
    concepts and how to utilize them to create a "smart" robot
# Long term Learning Plan  
Research ideas (aka things to learn while in this process)
### Common Robotic systems
http://manipulation.csail.mit.edu/
notes on an overall process MIT uses to create comp[lex decision makin robotics

ROS or Robotoc Operating system is a big goal of ours for this project. I want to learn how to use it well
http://wiki.ros.org/
        Sub wiki articles good to know about
        http://wiki.ros.org/smach

https://scottlocklin.wordpress.com/2020/07/29/open-problems-in-robotics/
where i created my own steps from this link


### Kinematics
https://en.wikipedia.org/wiki/Robot_kinematics
A good understanding of physics and specifically kinematics and how rigid structures with jointss are affected

(i found the following explaination for robotic kinematicsonline)
This is basically doing the math to say when I move motor n, the system moves in Cartesian (x, y, z) by (i, j, k). 
This applies the other way too, where if you want to move i in x direction, you may need to move multiple motors together.


### MediaPipe?
https://github.com/google/mediapipe


### This is the robot we will be modifying for our needs
https://www.thingiverse.com/thing:1454048
(EEZYbotARM MK2 bydaGHIZmois licensed under theCreative Commons - Attribution - Non-Commerciallicense)


