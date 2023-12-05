# SOLVING RUBIK'S CUBE OF 3X3X3 BY USING REINFORCEMENT LEARNING



The goal of this project is to use Q-learning to represent and solve the traditional Rubik's cube.

We used *Q-Learning, a potent reinforcement learning technique, to solve the Rubik's cube problem and **utilization of a pattern database* to determine the quality of near-finished cubes.


The *branching factor (bf)* of the cube's *state space tree* is significantly reduced since this project assumes that a Rubik's cube can *only execute 180 degree side turns*.


The other goal of this project is to solve a solved cube that has had *n random moves executed on it*. At the moment, the value of n can be as high as 5 to find a goal state for each execution, or as low as 6–10 to achieve some degree of success.


>*State()**, the state representation of a Rubik's Cube, and a few auxiliary functions that are utilized in other parts of the application are included in **puzzle.py*.


> A range of test cases are included in *tests.py* and *others.py* that can be run to verify that the cube's state representation is implemented correctly.


> The implementation of a reinforcement learning agent is included in *Agent.py*. It uses a pattern database in addition to Q-Learning iterations to build up a Q-Table, which is then used to attempt solving the random Rubik's cube.


### Using this project

copy the repository and verify you have python3 (any versions above 3.6) installed

`>>> python Agent.py (will run Q-Learning on a n=5 scrambled cube, and attempt to solve it) `
>>> It will take time to execute completely and final result may be achieved at first time if not re-execute / compile another time by *python Agent.py* until the agent reach the goal State.
>>> Future Scope: In future iterations, we plan to explore advanced techniques such as deep reinforcement learning to further improve the efficiency and accuracy of our Rubik's Cube solver. Additionally, incorporating parallelization for faster convergence is a potential avenue for optimization.


>>> To provide more context, we produced a video and posted it to YouTube. 
 *link: https://youtu.be/-D300FvlCWI?feature=shared*

To change the number of moves to apply to the initial cube, change *n=4* to any value on the *line 22* in Agent.py
`>>> self.start_state = cube if cube is not None else n_move_state(n=4) `


### contributors:
 **DINESH REDDY JETTA AND SAI KUMAR REDDY TUMMETI**


###### References:

McAleer, Stephen. *Solving the Rubik's Cube without Human Knowledge*. https://arxiv.org/pdf/1805.07470.pdf
OpenAI. _Solving Rubik's Cube with a Robot Hand._](https://openai.com/research/solving-rubiks-cube)

Lapan, Max. **Reinforcement Learning to solve Rubik’s cube (and other complex problems!)**. https://medium.com/datadriveninvestor/reinforcement-learning-to-solve-rubiks-cube-and-other-complex-problems-106424cf26ff 
