# Soldiworks CFD Simulation Project

&emsp;With my second year in college nearing, I wanted to obtain engineering experience through working on personal projects. As my end goal was to get an internship through showing employers my experience, I looked at and compared the qualifications and desired skills for a multitude engineering internships. A commonly desired skill I found throughout the internships was testing. Testing, in a general sense, has a broad meaning. It can range from manually making sure electronic components are functional to working on simulations by analyzing the airflow over a wing. I thought that working on simulations would be a excellent idea since I didn't need much to start: simply a computer with simulation software downloaded to it. 

&emsp;With the help of my dad, he pointed me to an article on computational fluid dynamics simulation with airfoils using Solidworks Flow simulation. Since I was a complete beginner in doing simulations, I carefully followed the tutorial until the end. Through this, I became more confident in doing simulations, and decided to take it a step further. In the latter half of my first in year college, I was in an aerial robotics club whose goal was to design a fixed-wing drone that would complete a set of challenges while navigating through an obstacle course. An idea suddenly popped into my mind that would involve the usage of my club's wing design. I used the same tutorial to help guide me through setting up the simulation. However, a complication soon arose. When attempting to run the simulation, an error message popped up reporting an inconsistency in the geometry of the model, which was mostly likely due to the design not being fully solid, or watertight. To get around this, I recreated the wing with the exact same parameters using my club's wing root and tip sketches, while keeping the part solid. In order to simulate actual flying conditions, I decided to base my parameters off of my team's competition rules (which included velocity, altitude, and thus temperature and pressure) assuming cruising altitude. 

&emsp;One of the most important technologies inside the Solidworks Flow simulation is goals, which lets the user set what type of values on what surfaces are to be calculated. The software offered different types of goals to be set; the main ones I used were surface goals, global goals, and equation goals. Surface goals allow the user to specify the surface or surfaces where the simulation will be done on, while global goals analyze all surfaces. Equation goals are mathematical equations that are dependent on other goals. I mainly used the surface goals to calculate crucial values such as velocity, pressure, and vorticity. I inserted one global goal to find the lift force of the wing, while from the global goal, I used the equation goal to find the coefficient of lift. From previous knowledge, I knew that the angle of attack of an airfoil directly influences the amount of lift produced, or more specifically, the lift coefficient. I decided to use angles of attack from 0 to 20 in steps of two, through cloning the project and altering the wing design using a rotation feature. 
