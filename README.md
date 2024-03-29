# Soldiworks CFD Simulation Project

&emsp;With my second year in college nearing, I wanted to obtain engineering experience through working on personal projects. As my end goal was to get an internship through showing employers my experience, I looked at and compared the qualifications and desired skills for a multitude engineering internships. A commonly desired skill I found throughout the internships was testing. Testing, in a general sense, has a broad meaning. It can range from manually making sure electronic components are functional to working on simulations by analyzing the airflow over a wing. I thought that working on simulations would be a excellent idea since I didn't need much to start: simply a computer with simulation software downloaded to it. 

&emsp;With the help of my dad, he pointed me to an article on computational fluid dynamics simulation with airfoils using Solidworks Flow simulation. Since I was a complete beginner in doing simulations, I carefully followed the tutorial until the end. Through this, I became more confident in doing simulations, and decided to take it a step further. In the latter half of my first in year college, I was in an aerial robotics club whose goal was to design a fixed-wing drone that would complete a set of challenges while navigating through an obstacle course. An idea suddenly popped into my mind that would involve the usage of my club's wing design. I used the same tutorial to help guide me through setting up the simulation. However, a complication soon arose. When attempting to run the simulation, an error message popped up reporting an inconsistency in the geometry of the model, which was mostly likely due to the design not being fully solid, or watertight. To get around this, I recreated the wing with the exact same parameters using my club's wing root and tip sketches, while keeping the part solid. In order to simulate actual flying conditions, I decided to base my parameters off of my team's competition rules (which included velocity, altitude, and thus temperature and pressure) assuming cruising altitude. 

&emsp;One of the most important technologies inside the Solidworks Flow simulation is goals, which lets the user set what type of values on what surfaces are to be calculated. The software offered different types of goals to be set; the main ones I used were surface goals, global goals, and equation goals. Surface goals allow the user to specify the surface or surfaces where the simulation will be done on, while global goals analyze all surfaces. Equation goals are mathematical equations that are dependent on other goals. I mainly used the surface goals to calculate crucial values such as velocity, pressure, and vorticity. I inserted one global goal to find the lift force of the wing, while from the global goal, I used the equation goal to find the coefficient of lift (put mathematical equation here!). From previous knowledge, I knew that the angle of attack of an airfoil directly influences the amount of lift produced, or more specifically, the lift coefficient. I decided to use angles of attack from 0 to 18 degrees in steps of two, through cloning the base project and altering the wing design using a move/copy feature. 

The below table displays the angles of attack from 0 to 18 degrees along with the corresponding lift coefficient value that was automatically calculated through the use of the lift equation.
| Angle of Attack (degrees)  | Lift Coefficient |
| ------------- | ------------- |
| 0  | 0.0051222  |
| 2  | 0.0074153  |
| 4  | 0.0082679  |
| 6  | 0.0129699  |
| 8  | 0.014454  |
| 10  | 0.0411846  |
| 12  | 0.0184427  |
| 14  | 0.0191028  |
| 16  | 0.0224054  |
| 18  | 0.022218  |

Here are the graphed results:  
![image](https://user-images.githubusercontent.com/107323771/203658252-a6828f71-7a58-4047-9ebc-b0e2815b2987.png)  

As shown in the table and graph, an angle of attack of 10 degrees results in the highest lift coefficient.  

From a visual perspective, here are two animations (one at a 0 degree angle of attack, the other at a 10 degree angle of attack) that shows the pressure across the airfoil as time passes.  


0 degree angle of attack:  

https://user-images.githubusercontent.com/107323771/203663617-531f5d1f-8c24-45d1-96ec-87d8164fd73d.mp4  

10 degree angle of attack:  

https://user-images.githubusercontent.com/107323771/203663869-3829e0a7-e34d-4627-8f73-73de41ed9808.mp4  

With a 0 angle of attack, as time goes on, the pressure values around the airfoil end up stabilizing, and the pressure above and below the airfoil are at the lowest. In comparison, with a 10 degree angle of attack, over time, the pressure distribution is such that there is more pressure below than above the airfoil, and this pressure difference across the airfoil is what causes lift. 

To further enforce the findings, here is an animation of the velocity in the x direction at an angle of attack of 10 degrees:  

https://user-images.githubusercontent.com/107323771/203666147-60c187bb-c002-4ec0-8ae6-42145a2098f7.mp4

From the start of the animation, it is clear that the velocity flows faster over than under the airfoil. By Bernoulli's equation, a low velocity means a high pressure, while a high velocity means a low pressure. The same conclusion is once again reached-lift is created due to the pressure difference.
