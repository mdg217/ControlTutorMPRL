# ControlTutorMPRL
Thesis project

# Preliminary Instruction
## Install Conda with Jupyter Notebook
To install the notebook click on this link and download the conda version: https://www.anaconda.com/products/distribution\
After the installation you will have all the components to work on your python and RL projects.

## Issue with "pip install"
Unfortunatly with standard installation of **Anaconda** in Windows there aren't some of the most important components to use pip and in particular pip install such as **Microsoft C++ Build Tools**.\
Infact you need to download the installer from: https://visualstudio.microsoft.com/visual-cpp-build-tools/

Now you can choose the following components: **C++ build tools**

*Restarting the Kernel of the notebook now is possible to use **pip install** instruction.*

## Install OpenAiGym
To install **OpenAiGym** you need to use two commands:
1. The first command is for all the repository of **gym**: ```pip install gym``` ;
2. THe second command is for a part of gym that isn't inculuded into main repository: ```pip install gym[2dbox]``` . 

## Example OpenAiGym
### Lunar Lander
Documentation: https://www.gymlibrary.dev/environments/box2d/lunar_lander/
```python
import gym
env = gym.make("LunarLander-v2", render_mode="human")
observation, info = env.reset(seed=30)
for _ in range(1000):
   action = policy(observation)  # User-defined policy function
   observation, reward, terminated, truncated, info = env.step(action)

   if terminated or truncated:
      observation, info = env.reset()
env.close()
```

# Theory necessary

## Reinforcement Learning theory

## MPC theory

## Control Tutor theory