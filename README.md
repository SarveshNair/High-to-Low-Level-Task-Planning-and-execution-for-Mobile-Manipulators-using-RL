# High-to-Low-Level Task Planning and Execution for Mobile Manipulators using Reinforcement Learning

## Overview
This project explores a hierarchical reinforcement learning (HRL) framework for sequential task planning and execution in mobile manipulators. The approach integrates high-level decision-making with low-level control for tasks such as navigation, object manipulation, and environment interaction. Using Unity ML-Agents, the framework provides a proof-of-concept for robots performing complex tasks in dynamic environments.

## Features
- **Hierarchical Reinforcement Learning (HRL):** Decomposition of complex tasks into subtasks for efficient learning.
- **Reward Shaping:** A combination of extrinsic and intrinsic rewards to accelerate convergence.
- **Intrinsic Curiosity Module (ICM):** Encourages exploration in sparse reward environments.
- **Unity ML-Agents Framework:** Simulated environment with realistic dynamics for training and testing.
- **Proximal Policy Optimization (PPO):** Algorithm for robust policy learning in continuous action spaces.

## Project Structure
- **Phase 1: Navigation**
  - Training the agent to navigate to target locations while avoiding obstacles.
- **Phase 2: Manipulation**
  - Training a 2-DOF manipulator for object pick-and-place operations.
- **Phase 3: End-to-End Integration**
  - Integrating navigation and manipulation tasks into a sequential workflow.

## Environment Setup
1. **Unity ML-Agents Toolkit**
   - Install Unity 2021 or later.
   - Add ML-Agents package via Unity Package Manager.

2. **System Requirements**
   - OS: Windows/macOS/Linux
   - Unity version: 2021.3 or later
   - Python: 3.8 or later
   - Required Python packages: `mlagents`, `numpy`, `torch`

3. **Running the Simulation**
   - Open the Unity project folder in Unity Hub.
   - Navigate to `Assets/Scenes` and open the training environment.
   - Start the Unity editor and run the simulation.

## Key Results
- **Improved Training Efficiency:**
  - Reward shaping and curriculum learning led to faster policy convergence.
- **Task Execution:**
  - The integrated system successfully navigates to targets, manipulates objects, and returns to drop-off locations.
- **Scalability:**
  - The framework demonstrates robustness and adaptability in dynamic environments.

## Future Work
- **Integration of Large Language Models (LLMs):**
  - Use LLMs to interpret high-level commands and design reward functions dynamically.
- **Real-World Deployment:**
  - Test the framework on physical robots for tasks like garbage collection in household environments.
- **Augmented Reality (AR) Interfaces:**
  - Develop user-friendly interfaces for task guidance and monitoring.

## How to Use
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/HighToLowTaskPlanningRL.git
   ```
2. Navigate to the project folder:
   ```bash
   cd HighToLowTaskPlanningRL
   ```
3. Open the project in Unity:
   - Launch Unity Hub.
   - Add the project folder.
   - Open the Unity Editor and start training.
4. Train the RL agent:
   - Modify training parameters in `ml-agents-config.yaml` if necessary.
   - Run training scripts from Unity Editor or Python.

## References
- [Unity ML-Agents Documentation](https://github.com/Unity-Technologies/ml-agents)
- "Curiosity-driven Exploration by Self-supervised Prediction" ([Paper](https://arxiv.org/pdf/1705.05363))
- "ExploRLLM: Guiding Exploration in Reinforcement Learning with Large Language Models" ([Paper](https://arxiv.org/abs/2403.09583))

## License
This project is licensed under the MIT License. See `LICENSE` for details.

## Acknowledgments
We extend our gratitude to Prof. Yanhua Li and our teaching assistant for their invaluable guidance throughout the project. Special thanks to the Unity ML-Agents team for their open-source tools and documentation.

