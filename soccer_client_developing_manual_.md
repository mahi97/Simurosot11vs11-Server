## Strategy development:

Because the Client/Server mode applied in simulating robot soccer game, the strategy of client depends on the position of every robot and ball sent by the server. According to the position of robots and ball in the game field, each team can decide what strategy can be used. Some variables in the strategy are introduced as follow:

1. Attacking Direction : in the simulation system, the strategies of each team can be considered  attacking from right to left,  i.e., each team can develop the strategy without consideration whether the team is left or right. The coordinate conversion of left team and right team will be completed in the server, as figure 1 shows.
  
2. Member position: we defined the five robot structure which each team used: home1,home2,home3,home4,..., and use structure opponent that gives positions of opponent team.

3. The coordinates of member: homeX.position.x , homeX.position.y is the position of member X of our team. Opponent.positionX.x, opponent.positionX.y is the position of opponent team member X.
  
4. The angle of member : homeX.angle is the direction of member X.

5. The size of game field: In program, boundRect.left, boundRect.right are used to show the x coordinates of the left and right end of the game field , boundRect.right>boundRect.left , boundRect.top, bountRect.bottom to show the y coordinates of the top and bottom of the field; undRect.bottom>boundRect.top.
Therefor,boundRect.left,bountRect.right,boundRect.top,boundRect.bottom is defined in CStrategySystem::CStrategySystem() . The degree increases from 0 to 180 when robot rotates clockwise. And the degree decreases from 0 to   -180 when robot rotates counterclockwise.

6. The using of Velocity function:
We provide the bottom layer function of kinematics calculating, so that each team can devote its effort entirely into the design of game strategies. We can get the left and right velocity of robot by these functions, which can expediently be used by each team to develop their strategies more better and faster.
Function prototype: Velocity(int which,int vL,int vR), here 'which' is the same as the Position entry parameter, it is used to indicate one member of this team. vL,vR is used to show the  velocity of left wheel and right wheel. Velocity is calculated according to dynamics.

7. Coordinates of balls:
  We defined the class object of balls in the strategy class, Robot1 ball, The coordinates of balls is showed as that:
X direction 's coordinates:  ball.position.x,
Y direction 's coordinates:  ball,position.y

8. Strategy examples:
  We have completed the network communication framework in Client, the strategy of Client can be written in the strategy function we left, The function is:  NormalGame(), NormalGame1(), NormalGame2(), NormalGame3(), NormalGame4(), NormalGame5().
  
9. Brief summary:
  We introduced some variables and functions that are used in Simulating robot soccer system. Using these basic variables and functions, we can develop more advanced action and game strategy. If the existing strategy functions isn't enough, developer can add more strategy function in CstrategySystem::Think() function. The detailed method can consult Think() function. In addition, the numerical value used in the above variables and functions are all given by the pixels of screen. But it can't affect our strategy developing.
