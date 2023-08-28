# DS551/CS525 2023 Fall Individual Project 1
# Dynamic Programming of Markov Decision Process

#### Starting Date
* Week 2 Tuesday September 5, 2023(23:59)

#### Due Date
* Week 4 Tuesday September 19, 2023(23:59)

#### Total Points
* 100 (One Hundred)

## Goal

* In this assignment, you will be asked to implement policy iteration and value iteration for the Frozen Lake environment (FrozenLake-v1) from [OpenAI Gymnasium](https://gymnasium.farama.org/environments/toy_text/frozen_lake/) and play the game with the algorithms you implemented. This project will be completed in Python 3.



<img src="/Project1/img/hw1.png" width="80%">

* See more details of FrozenLake on [OpenAI Gymnasium](https://gymnasium.farama.org/environments/toy_text/frozen_lake/).


* If your program works, the command line output should look like this.
<img src="/Project1/img/UnitTest2023.png" width="80%">

## Deliverables

Please compress your mdp_dp.py file into a zipped file (firstName_lastName_hw1.zip) and submit it to Canvas.

## Grading
* policy evaluation (20 points)
* policy improvement (20 points)
* policy iteration (20 points)
* value iteration (20 points)
* rander game (20 points)

## Hints
* Policy Evaluation<br/>
<span style="color:red">**Please note that reward can be defined on (state), (state, action), (state, action, next_state). In this assignment, we define the reward on (state,action,next_state).** The following pseudocode is the general method.</span>
<img src="/Project1/img/pe.png" width="80%" >

* Policy Iteration<br/>
<img src="/Project1/img/pi.png" width="80%" >

* Value Iteration<br/>
<img src="/Project1/img/vi.png" width="80%" >


## Setup
* Recommended programming IDE (integrated development environment): VS code (See [install VS code](https://code.visualstudio.com/)) 
* Install [Miniconda](https://www.python.org/downloads/)
* Install [Python 3](https://www.python.org/downloads/), by default, it's Python 3.11.4 now (Aug 20, 2023).
* Create virtual environment: conda create -n myenv python
* Activate your virtual environment: conda activate myenv
* Install gymnasium: pip install "gymnasium[atari]" (See [install gymnasium](https://github.com/Farama-Foundation/Gymnasium))
* Install nose: pip install pynose (See [install nose](https://pypi.org/project/pynose/))
  

```diff
- Note: Our environment code mdp_dp.py and mdp_dp_test.py were developed/updated for the latest version of OpenAI gymnasium (version 0.29.0). 

- So when you install your gym, please use command line pip install "gymnasium[atari]". 
```


## Guidelines
* Implement functions in mdp_dp.py
* Evaluate functions by typing "nosetests -v mdp_dp_test.py" in terminal (you need put mdp_dp.py and mdp_dp_test.py in the same folder)
* If you got error using "nosetests -v mdp_dp_test.py" due to python version (sometimes, nosetests will use python2.7 by default), try: python3 -m nose -v mdp_dp_test.py

## Tips for Python and OpenAI Gym
[Python Documentation](https://www.python.org/doc/)

[Python Tutorial](https://www.geeksforgeeks.org/python-programming-language/)

[OpenAI Gym Documentation 1](https://gymnasium.farama.org/)

[OpenAI Gym Documentation 2](https://github.com/Farama-Foundation/Gymnasium)
