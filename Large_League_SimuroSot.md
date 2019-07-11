FIRA Large League SimuroSot Game Rules

Law 0. General rules
(1)   The aim of simulate competition:
(a)   It is used for developing basic action algorithm and game strategy of robot soccer.
(b)   It is used for providing game training and strategy learning environment for each team.
(c)	It is used for testing the feasibility and advancement of the game strategy of each team.

(2)   rationale of simulate competition:
(a)  Using computer graphics to simulate the field, the robots and the ball.
(b)  Using kinematics and dynamics to simulate movements of the robots and the ball.
(c)  Firstly, input each team’s game strategy into the client program, and then link the clients to the server using UDP/IP protocol. Secondly, make the preparation for competition. It includes the startup of system and the position of the robots of each team. Finally, match between each team. Like the MiroSot competition, simulate competition is controlled by the referee. The game begins, when the referee whistles. The game follows the rules that this text puts forward.

(3)   simulate competition hardware:
(a)  The simulate competition uses three computers (IBM/586-600), one used as server, the other two used as clients.
(b)  Three computers are connected through Ethernet.

(4)   Simulate competition software framework:
(a)  Simulate competition software is compiled using VC++ 6.0, and it can run under windows 98.
(b)  Figure 1 is the SimuroSot software framework :

               Figure 1 SimuroSot software framework

(5)  the role of referee is:
(a) to control the begin, break and finish of the game;
(b)  to declare penalty to the fouls.

Law 1. The Field
(1) Playground dimensions (Appendix1)
A black rectangular playground 1130(pixel) x 788(pixel) in size, with 5(pixel) thick light blue side-walls will be used. Solid 42(pixel) x 42(pixel) isosceles triangles shall be fixed at the four corners of the playground to avoid the ball getting cornered.

(2) Markings on the playground (Appendix 2)
The field of play shall be marked as shown in Appendix 2. The center circle will have a radius of 123(pixel). The arc, which is part of the goal area, will be 123(pixel) along the goal line and 28(pixel) perpendicular to it. The major lines/arcs (centerline, goal area borderlines and the center circle) will be gray in color and 4(pixel) in thick. The free ball robot positions (circles) shall be marked in royal purple color. 

(3) The goal 
The goal shall be 246 (pixel) wide. Posts and nets shall not be provided at the goal.

(4) The goal line and goal area
The goal line is the line just in front of the goal which is 246(pixel) long. The goal areas shall comprise of areas contained by the rectangle (sized 426(pixel) x 90(pixel) in front of the goal) and the attached arc (123(pixel) in parallel to the goal line and 28(pixel) perpendicular to it). 

(5) The ball 
An orange golf ball shall be used as the ball, with 5(pixel) diameter. 

(6)  The robots
The robots is square sized 10(pixel) x 10(pixel). Each robot is in team’s clothe which can be chosen before the match.

(7) The field location 
The field is at the center of the screen. 

(8) The control menu
The control menu is at the top of the field. 

(9) The clock
The clock is at the left of the menu.

(10) The score board
The score board is at right of the menu.

Law 2: The Game Sequence 
(1)  The preparation of the match
Firstly, each team inputs its client into the client computer. Secondly, each team run the client program. Finally, each team press the ‘Link’ item in the toolbar, then each client program is linked to the server.
(2)  The begin of the match
When the referee press the ‘go’ item of the menu in the server, the match will start. And if the ‘break’ item is pressed, the match will break. If the ‘stop’ item is pressed, the match will terminate. And pressing ‘Esc’ in the keyboard make the program return to the Windows.

Law 3: Game Duration
(1) The duration of a game shall be two equal periods of 5 minutes each, with a half time interval for 10 minutes. An official timekeeper will pause the clock during substitutions, while transporting an injured robot from the field, during time-out and during such situations that deem to be right as per the discretion of the timekeeper. 

(2) If a team is not ready to resume the game after the half time, additional 5 minutes shall be allowed. Even after the allowed additional time if such a team is not ready to continue the game, that team will be disqualified from the game. 

Law 4: Method of Scoring
(1) The Winner 
A goal shall be scored when the whole of the ball passes over the goal line. The winner of a game shall be decided on the basis of the number of goals scored. 

(2) The Tiebreaker 
In the event of a tie after the second half, the winner will be decided by the sudden death scheme. The game will be continued after a 5 minutes break, for a maximum period of three minutes. The team managing to score the first goal will be declared as the winner. If the tie persists even after the extra 3 minutes game, the winner shall be decided through penalty-kicks. Each team shall take three penalty-kicks, which differs from as only a kicker and a goalkeeper shall be allowed on the playground. The goalkeeper should be kept within its goal area and the positions of the kicker and of the ball shall be the same as the Law. After the referee's whistle, the goalkeeper may come out of the goal area. In case of a tie even after the three-time penalty-kicks, additional penalty-kicks shall be allowed one-by-one, until the winner can be decided. All penalty-kicks shall be taken by a single robot and shall commence with the referee's whistle. 

Law 5: Fouls
A foul will be called for in the following cases. 
(1) Colliding with a robot of the opposite team, either intentionally or otherwise: the referee will call such fouls that directly affect the play of the game or that appear to have potential to harm the opponent robot. When a defender robot intentionally pushes an opponent robot, a free kick will be given to the opposite team. It is permitted to push the ball and an opponent player backwards provided the pushing player is always in contact with the ball. 

(2) It is permitted to push the goalkeeper robot in the goal area, if the ball is between the pushing robot and the goalkeeper. However pushing the goalkeeper into the goal along with the ball is not allowed. If an attacking robot pushes the goalkeeper along with the ball into the goal or when the opponent robot pushes the goalkeeper directly then the referee shall call free-ball. 

(3) It is referred to as handling, as judged by the referee, when a robot other than the goalkeeper catches the ball. It is also considered as handling, if a robot firmly attaches itself to the ball such a way that no other robot is allowed to manipulate the ball.

(4) The goalkeeper robot should kick out the ball from its goal area within 10 seconds. The failure to do so will be penalized by giving a free-ball .

(5) Giving a free-ball to the defensive team will penalize the blocking of a goalkeeper in its goal area.

Law 6: Free Kick
When a defender robot intentionally pushes an opponent robot, a free kick will be given to the opposite team. The ball will be placed at the relevant free kick position (FK) on the playground (Appendix 2). The robot taking the kick shall be placed behind the ball. The attacking team can position its robots freely within its own side. The defending robots shall be placed in touch with the goal area on either side of the arc. With the referee’s whistle all robots can start moving freely.

Law 7: Penalty-Kick
A penalty-kick will be called under the following situation:
Defending with more than one robot in a goal area. An exception to this is the situation when the additional robot in the goal area is not there for defense or if it does not directly affect the play of the game. The referee shall judge the penalty-kick situation.
When the referee calls a penalty-kick, the ball will be placed at the relevant penalty kick position (PK) on the playground (Appendix 2). The robot taking the kick shall be placed behind the ball. While facing a penalty kick one of the sides of the goalkeeper must be in touch with the goal line. The goalkeeper may be oriented in any direction. Other robots shall be placed freely within the other side of the half-line, but the attacking team will get preference in positioning their robots. The game shall restart normally (all robots shall start moving freely) after the referee's whistle. The robot taking the penalty-kick may kick or dribble the ball.

Law 8: Free-Ball 
A free-ball will be called under the following situations.
(1)	When a stalemate occurs for 10 seconds.
(2)	When an opponent robot blocks the goalkeeper in its goal area.
(3)	When attacking with more than one robot in the goal area of the opposite team.
When a free-ball is called within any quarter of the playground, the ball will be placed at the relevant free ball position (FB) (Appendix 2). One robot per team will be placed at locations 14(pixel) apart from the ball position in the longitudinal direction of the playground. Other robots
(of both teams) can be placed freely outside the quarter where the free-ball is being called, but with the rule that, the defending team will get their preference in positioning their robots. The game shall resume when the referee gives the signal and all robots may then move freely. 

 
Appendix 1:

 
Appendix 2:
 


