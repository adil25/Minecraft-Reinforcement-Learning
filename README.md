# Minecraft-Reinforcement-Learning
Deep Q Learning for resolving Partially Observable MDP based on Minecraft environment.
We use gym-minecraft which allows the use of the MalmoProject with an OpenAI like API.

## Prerequisites
- Python 3.6
- Tensorflow (GPU)
- Jupyter

## Installation
- Here’s the tutorial to [install gym-minecraft on Ubuntu 16.04](https://github.com/vincentberaud/Minecraft-Reinforcement-Learning/blob/master/Gym-Minecraft_Installation.ipynb).
- You can find the environments we use in the folder “envs”. You’ll have to put them in “site-packages/gym_minecraft-0.0.2-py3.6.egg/gym-minecraft/assets/

*Warning: The CliffWalking environment doesn’t work (the move action doesn’t work)*

## Neural Architecture
You can choose (with an enum) between 3 network types:
- Feed Forward
- Convolutional Network
- LSTM + CNN

![LSTM architecure](https://raw.githubusercontent.com/vincentberaud/Minecraft-Reinforcement-Learning/master/LSTM_Architecture.jpg)

## DQN settings
- Implementation of Double Q Learning
- Learning Rate, α : 0.00025
- ε-greedy implementation
- Experience replay iplementation

## Note
Unlike Deepmind’s implementations of DQN for Atari games, Minecraft has the constraint that the game isn’t in pause during two actions ordered by the agent. Accordingly the agent and the network have to be as fast as needed to play in the range of time fixed in the environment.

## Credits
We would like to thank Arthur Juliani for all his work and medium articles. Tambet Matiisen for his nice implementation of Gym-Minecraft. 

