# DS551/CS525 Inidividual Project 3
# Deep Q-learning Network(DQN)
Please don't revise test.py, environment.py, atari_wrapper.py, main.py, and agent.py

You work on the following files, including agent_dqn.py and dqn_model.py. 

You can optionally update argument.py to add your own arguments (if needed).

#### Starating Date
* Week 7, Tuesday Oct 10, 2023 (23:59)

#### Due Date
* Week 12, Tuesday Nov 14, 2023 (23:59))

#### Total Points
* 100 (One Hundred)

## Leaderboard and Bonus Points
In this project, we will provide a leaderboard and give **10** bonus points to the **top 3** highest reward students! 
* Where to see the leaderboard 
  * We will create a discussion on Canvas and each of you can post your highest reward with a sreenshot. TA will summarize your posts and list the top 3 highest rewards and post it below. <br>
  * The leaderboards of previous years are also posted at the end of this page, you can check it out.
  
  **Leaderboard for Breakout-DQN** 
  **Update Date: **
  
  | Top | Date | Name | Score | Model |
  | :---: | :---:| :---: | :---: | :---: |
  | 1  | 11/7/2023 | Antony Garcia | 426 | DQN |
  | 2  | 11/13/2023 | Daniel Moyer | 377.5 | ... |
  | 3  | ... | ... | ... | ... |


* How to elvaluate
  * You should submit your lastest trained model and python code. TA will run your code to make sure the result is consistent with your screenshot. 
* How to grade
  * Top 3 students on the leaderboard can get 10 bonus points for project 3.
  
## Setup
* Recommended programming IDE (integrated development environment): VS code (See [install VS code](https://code.visualstudio.com/)) 
* Install [Miniconda](https://www.python.org/downloads/)
* Install [Python 3](https://www.python.org/downloads/), by default, it's Python 3.11.5.
* Create virtual environment: `conda create -n myenv python==3.11.5`
* Activate your virtual environment: `conda activate myenv`
* Install gymnasium: `pip install opencv-python-headless gymnasium[atari] autorom[accept-rom-license]` (See [install gymnasium](https://github.com/Farama-Foundation/Gymnasium))
* install pytorch: See [install pytorch](https://pytorch.org/get-started/locally/)
* For the  Atari wrapper, install the following two items: `pip install -U "ray[rllib]" ipywidgets`
* For video recording in testing, install the following three items: `conda install -c conda-forge moviepy`, `conda install -c conda-forge ffmpeg`, `conda update ffmpeg`
* When testing, for nice output on the terminal, you need to install tqdm: `conda install -c conda-forge tqdm`

## How to run :
training DQN:
* `$ python main.py --train_dqn`

testing DQN:
* `$ python main.py --test_dqn`

testing DQN while recording a video (recording video takes time, so usually you use this option when the number of testing episodes is small):
* `$ python main.py --test_dqn --record_video`

## Goal
In this project, you will be asked to implement DQN to play [Breakout](https://gymnasium.farama.org/environments/atari/breakout/). This project will be completed in Python 3 using [Pytorch](https://pytorch.org/). The goal of your training is to get averaging reward in 100 episodes over **40 points** in **Breakout** (each episode has 5 lives), with OpenAI's Atari wrapper & clipped reward. For more details, please see the [slides](https://docs.google.com/presentation/d/1Yg1_RIOF7LA_a6uSa0lZ4asmayQ1s6ce/edit?usp=sharing&ouid=106040042903845857494&rtpof=true&sd=true).

<img src="/Project3/materials/project3.png" width="80%" >

## Deliverables
Please compress all the below files into a zipped file and submit the zip file (firstName_lastName_hw3.zip) to Canvas.

* **Trained Model**
  * Model file (.pth)
  * If your model is too large for Canvas, upload it to a cloud space and provide the download link 

* **PDF Report**
  * screenshot of the test results
  * Set of Experiments Performed: 
    * Include a section describing the set of experiments that you performed
    * what structures you experimented with (i.e., number of layers, number of neurons in each layer)
    * what hyperparameters you varied (e.g., number of epochs of training, batch size and any other parameter values, weight initialization schema, activation function)
    * what kind of loss function you used and what kind of optimizer you used.
  * Special skills: Include the skills which can improve the generation quality. Here are some [tips](https://arxiv.org/pdf/1710.02298.pdf) may help. (Optional)
  * Visualization: Learning curve of DQN. 
    * X-axis: number of episodes
    * Y-axis: average reward in last 30 episodes.
    
    <img src="/Project3/materials/plot.png" width="60%" >

* **Python Code**
  * All the code you implemented including sample codes.

## Grading
* **Trained Model (50 points)**
  * Getting averaging reward in 100 episodes over **40 points** (with 5 lives) in Breakout will get full credits. 
  * For every average reward below 40, you will be taken off 2 points. i.e., you will be taken off 2 points, if getting averaging reward in 100 episodes is 39 and taken off 4 points, if averaging reward is 38, so on so forth.

* **PDF Report (30 points)**
  * Set of parameters performed: 20 points
  * Visualization: 10 points
  
* **Python Code (20 points)**
  * You can get full credits if the scripts can run successfully, otherwise you may loss some points based on your error.

## Hints
* [Naive Pytorch Tutorial](https://github.com/lllyyyt123/WPI-DS551-Fall23/blob/main/Project3/Pytorch_tutorial.ipynb)
* [How to Save Model with Pytorch](https://github.com/yingxue-zhang/DS595CS525-RL-Projects/blob/master/Project3/materials/How%20to%20Save%20Model%20with%20Pytorch.pdf)
* [Official Pytorch Tutorial](https://pytorch.org/tutorials/)
* [Official DQN Pytorch Tutorial](https://pytorch.org/tutorials/intermediate/reinforcement_q_learning.html)
* [Official DQN paper](https://www.cs.toronto.edu/~vmnih/docs/dqn.pdf)
* [Rainbow: Combining Improvements in Deep Reinforcement Learning](https://arxiv.org/pdf/1710.02298.pdf)
* [DQN Tutorial on Medium](https://medium.com/@jonathan_hui/rl-dqn-deep-q-network-e207751f7ae4)

## Tips for Using Turing GPUs or Google Cloud
* [How to use GPUs on WPI Turing](https://github.com/yanhua-rep/WPI-DS551-Fall23/blob/main/Project3/materials/Turing_Setup_Instructions.pdf)
* [Google Cloud Platform](https://colab.google/)

  
## Leaderboard for Fall 2019** 
  
  | Top | Date | Name | Score |
  | :---: | :---:| :---: | :---: |
  | **1**   |10/22/2019| **Prathyush SP**          |  **142.77**    | 
  |         |10/18/2019| Prathyush SP          |  81.07     | 
  | **2**   |10/28/2019| **Sapan Agrawal**         |   **91.34**    |
  | 3   |11/1/2019| Hanshen Yu| 86.82 |
  | **4**   |10/31/2019| **Mohamed Mahdi Alouane** | **80.24**     | 
  | 5   |10/26/2019| Vamshi Krishna Uppununthala|  79.5   | 
  | 6   |10/31/2019| Sai Vineeth K V | 66.5 | 
  | 7   |11/14/2019| Cory neville | 59.96 | 
  | 8   |10/24/2019|Shreesha Narasimha Murthy  |56.79     | 
  | 9   |10/20/2019|Sinan Morcel            |53.26        |
  
## Leaderboard for Fall 2020** 

  | Top | Date | Name | Score |
  | :---: | :---:| :---: | :---: | 
  | 1  | 11/19/2020|Abhishek Jain  | 424.21  |
  | 2  | 11/19/2020|Akshay Sadanandan  | 403  |
  | 3  | 11/19/2020|Dhirajsinh Deshmukh  | 393.37  |
  |4 |11/19/2020 |   Daniel Jeswin Nallathambi      | 335.26  |
  | 5  | 11/18/2020|Sayali Shelke  | 334  |
  |6 | 11/19/2020|Varun Eranki  | 298  |
  | 7  | 11/5/2020|Apiwat Ditthapron  | 194.5  | 
  |8 | 11/18/2020|Panagiotis Argyrakis  | 156.09  |
  |9 | 11/20/2020|Scott Tang  | 153.89  |
  |10 | 11/18/2020|Xinyuan Yang  | 139.11  |
  
## Leaderboard for Spring 2022**
  
  | Top | Date | Name | Score |
  | :---: | :---:| :---: | :---: | 
  | 1  |4/6/2022 | Hongchao Zhang | 128 |
  | 2  |4/13/2022 | Apratim Mukherjee| 112 |
  | 3  | 4/6/2022 |  Puru Upadhyay | 82 |
  | 4  | 4/6/2022 |  Khai Yi Chin | 81 |
  | 4  | 4/6/2022 |  Karter Krueger | 81 |
  | 6  | 4/6/2022 |  Sailesh Rajagopalan | 78 |
  | 6  |4/6/2022 | Steven Hyland | 78 |
  | 8  |4/6/2022 | Yiran Fang | 74 |
  | 9  |4/6/2022 | Zhentian Qian | 67 |
  | 10  |4/6/2022 | Anujay Sharma | 66 |

## Leaderboard for Fall 2022**
  | Top | Date | Name | Score | Model |
  | :---: | :---:| :---: | :---: | :---: |
  | 1  | 10/24/2022 | Palawat Busaranuvong | 317 | Prioritized DQN |
  | 2  | 11/15/2022 | Amey Deshpande | 166.8 | ... |
  | 2  | 11/15/2022 | Rane, Bhushan | 166.8 | ... |
  | 3  | 11/15/2022 | Yash Patil | 113.14 | ... |
  | 4  | 11/06/2022 | Yiwei Jiang | 96.45 | DDQN |
  | 5  | 11/15/2022 | Aniket Patil | 92.18 | ... |
  | 6  | 11/14/2022 | Samarth Shah | 85.39 | DDQN with Prioritized Replay |
  | 7  | 11/15/2022 | Neet Mehulkumar Mehta | 80.39 | ... |
  | 8  | 11/15/2022 | Noopur Koshta | 79.68 | ... |  
  | 9  | 11/15/2022 | Kunal Nandanwar | 79.68 | ... |            
  | 10  | 11/14/2022 | Aadesh Varude | 71.65 | Vanilla DQN |
  | 11  | 11/1t/2022 | Rutwik Bonde | 69.52 | ... |  
  | 12  | 11/07/2022 | Brown, Galen | 69.01 | Basic DQP with reward shaping |
  | 13  | 11/5/2022  | Ryan Killea | 67.12 | ... |
  | 14  | 11/14/2022  | Rushabh Kheni | 65.51 | Vanilla DQN with Deepmind architecture |  
  | 15  | 10/30/2022 | Jack Ayvazian | 47.49 | Double DQN, DeepMind Architecture |  
  
