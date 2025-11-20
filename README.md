🚀 GaganYaan – Deep Q-Network Agent for Lunar Landing
A PyTorch-based Deep Reinforcement Learning project using DQN (Deep Q-Network) to safely land a spacecraft in a custom Gaganyaan lunar landing environment, built on top of Gymnasium’s LunarLander-v3.
This project demonstrates modern reinforcement learning techniques such as experience replay, target networks, epsilon-greedy exploration, and environment rendering for agent behavior visualization.

Features
🌒 Custom Gaganyaan Environment
Modified version of LunarLander-v3
Simulates safe lunar landing dynamics
Reward shaping and landing accuracy focus

🤖 Deep Q-Network (DQN) Implementation
Built from scratch using PyTorch
Uses:
Experience Replay Buffer
Target Network for stable learning
Epsilon-Greedy Strategy
Adam optimizer
Mean squared error loss

🎥 Agent Rendering & Evaluation
Videos generated to visually analyze landing performance
Evaluation phase after training

📓 Jupyter Notebook
Entire workflow in GaganYaan.ipynb
Easy to understand, step-by-step execution
Great for demonstrations and learning RL concepts


🛠️ Tech Stack
Component                  	Technology
Language	                   Python
Machine Learning	           PyTorch
RL Environment          Gymnasium (custom + LunarLander-v3)
Notebook	                 Jupyter (.ipynb)



🚀 How It Works
1. Initialize Environment
A custom environment (similar to LunarLander-v3) is loaded for training.

2. Build the Neural Network
A fully-connected network approximates the Q-values for each action.

3. Train with DQN
The agent learns using:
Replay buffer samples
Periodic updates to a target network
Gradually decreasing exploration (ε-decay)

4. Evaluate
Render episodes to confirm if the spacecraft performs controlled and safe landings.

📊 Results
After training, the agent learns to:
Reduce velocity at the right time
Balance thrust during descent
Perform smooth landings
Achieve higher cumulative rewards
(Rendered video or evaluation plots can be placed here.)


▶️ Running the Project
1. Install Dependencies
pip install torch gymnasium[box2d] numpy matplotlib

2. Run the Notebook
jupyter notebook GaganYaan.ipynb

3. Train the Agent
Run the training cells inside the notebook — results and videos will be generated automatically.


📘 Learning Objectives
This project helps you understand:
Core principles of reinforcement learning
How DQNs stabilize learning using target networks
Balance between exploration & exploitation
Neural network function approximation
Environment interaction loops in RL

🧩 Future Improvements
✔️ Double DQN
✔️ Dueling DQN
✔️ Prioritized Experience Replay
✔️ Logging with TensorBoard
✔️ Turning notebook into a Python module


🙌 Acknowledgements
OpenAI Gym / Gymnasium for LunarLander environment
PyTorch for deep learning framework
ISRO’s Gaganyaan mission for inspiration ✨
