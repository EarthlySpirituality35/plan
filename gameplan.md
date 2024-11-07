# **Assessment Game Plan**

## **Identifying and Defining**

### **Identifying the Need**

I am creating a golf like game where the user hits the ball with a certain amount of power. The more you drag back, the more power the golf ball gets. As the user, you will have to complete levels with the least amount of swings possible. This game would require a variety of skills that include focus, hand-eye coordination and problem-solving. It is vital that children gain skills such as focus, hand-eye coodination and problem-solving and this game provides these skills while making it interactive and entertaining which is an important part of teaching skills to children. I will utilise the rolling ball tutorial to get a base of creating the game then use other tutorials to get the ball velocity or mouse drag movement.

### **Requirements Online**

**Inputs**

When the user pulls back the mouse the amount its pulled back should correspond to the amount of velocity that the ball has. When the user scrolls on the scrollwheel, the camera should scroll out.When the user holds right click and moves the mouse, it should be a sort aiming tool, panning around.

**Processing**

When aiming,  the user should not aim when the ball is rolling or when it is already in the hole. When the ball is moving and it collides with a wall, it should be able to bounce off the wall with respective velocity. 

**Outputs**

The number of turns spent and par should both be put on the topside of the screen.After completing the level, a number of stars should be allocated with the par being 2 stars, under par being 3 stars and above the par being 1 star. After the golf ball is put into the golf hole, there should be a victory sound. After striking the ball, a ding sound of some sort should be made.

**Transmission**

There will be no multiplayer options in the game.


**Storage**

The data of the game should be able to be saved locally on the computer of the one playing the game.

### **Functional Requirements**

**User Interactions**

Using WASD will turn and aim your camera in the corresponding direction. If the user clicks space, it will make the ball temperarily go up and down, sort of like jump function. By dragging the mouse back, it will make the ball go forwards. '

**Core Gameplay or Simulation Mechanics**
 
There are many mechanics incorperated into my game such as a pull back mechanic where you pull back your mouse the amount you pull back translates to the velocity that the ball has. It also has a wall bounce mechanic and when the ball bounces off the wall, it should lose velocity and bounce back accordingly. 

**Scoring and Feedback**

There is a scoring system with the par being a certain number. The amount of swings would corrolate with the amount of stars with on par being 2 stars, over par being 1 star and under par being 3 stars. This should be able to be saved.

**Level Progression or Simulation Stages**

There is a level system and after completing one level, you will move on to the next level. After getting the ball into the hole, there will be an option whether to redo the level to get more stars or to move onto the next level.

**Saving and Data Loading**

Data will be saved locally on the user's device.

### **Non-Functional Requirements**

**Performance Requirements**

The game should be smooth with all textures and parts loading in quickly. Moving onto the next stage or repeating a stage should be almost instant. The game should load within a couple seconds and respond to inputs instantly.

**Usability Requirements**

The game will have a play button and an instructions button after loading in. After clicking play, the levels should come up. If the user clicks instructions, a step-by-step guide should come up. This game should be fairly easy to navigate.

**Scalability Requirements**

The game is extremely scalable as it would be easy to add new stages or levels as the scripts and mechanics should be virtually the same.

### **Consideration of Social and Ethical Issues**

Equity: equity is all about fairness, giving everyone an equal chance but it could also to do with the value of shares, issued by a company
Accessibility: accessibility is all about whether everyone has the ability to play the game or whether it can be used by everyone.

**Accessability**

Everyone on a computer should have access to this game. It should be able to be globally used by everyone.

**Privacy and Data Protection**

It should not take any other information except the scores and levels that the user has completed.

**Fairness and Representation**

There will be no negative representations within my game as there are no people/races, rather just being a white golf ball.

**Mental and Emotional Well-Being**

The game in no way encourages or talks about anything to do with mental well-being. 

**Cultural Sensativities**

The game in no way has anything to do with race or culture. 

## **Researching and Implementing**

### **PMI Table**

### **Pseudocode and Flow Chart**

![](userinteractions.png)


BEGIN UserInteraction  
&nbsp;&nbsp;WHILE "Scouting"  
&nbsp;&nbsp;&nbsp;&nbsp; IF "W Pressed" THEN  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  DISPLAY "Move Camera Upwards"  
&nbsp;&nbsp;&nbsp;&nbsp; ELSE IF "A Pressed" THEN  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  DISPLAY "Move Camera Leftwards"  
&nbsp;&nbsp;&nbsp;&nbsp; ELSE IF "S Pressed" THEN  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  DISPLAY "Move Camera Downwards"  
&nbsp;&nbsp;&nbsp;&nbsp; ELSE IF "D Pressed" THEN  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  DISPLAY "Move Camera Rightwards"  
&nbsp;&nbsp;&nbsp;&nbsp; END IF  
&nbsp;&nbsp;END WHILE  
&nbsp;&nbsp;WHILE "Aiming"  
&nbsp;&nbsp;&nbsp;&nbsp; INPUT PulledBackAmount  
&nbsp;&nbsp;&nbsp;&nbsp; DISPLAY DistanceTravelled  
&nbsp;&nbsp;END WHILE  

&nbsp;&nbsp;WHILE "Game Start"  
&nbsp;&nbsp;&nbsp;&nbsp; IF "Space Pressed" THEN  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  DISPLAY "Jump"  
&nbsp;&nbsp;&nbsp;&nbsp; END IF  
&nbsp;&nbsp;END WHILE  
END UserInteraction