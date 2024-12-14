# Traffic Signal Control System

This repository contains a project integrating SUMO (Simulation of Urban MObility) with reinforcement learning algorithms to optimize traffic management and control systems. The project includes implementations of Q-learning and DQN (Deep Q-Network) algorithms and provides a complete setup for training and testing RL agents in a SUMO environment.

## Project Structure

- **`outputs/`**  
  Contains CSV files generated by SUMO, including simulation results and performance metrics.

- **`algorithms/`**  
  Implements reinforcement learning algorithms:
  - `ql.py`: Classic Q-learning implementation.
  - `dqn.py`: Deep Q-Network implementation with neural network-based function approximation.
  - `sarsa.py`: SARSA algorithm is a slight variation of the popular Q-Learning algorithm.

- **`docs/`**  
  Contains documentation-related resources, including:
  - Images of actions, reward functions, and the SUMO environment.

- **`sumo_rl/`**  
  Core components of the reinforcement learning environment:
  - `agents/`: Definitions of RL agents.
  - `environment/`: SUMO environment configuration for RL.
  - `exploration/`: Exploration strategies for RL agents (e.g., epsilon-greedy).
  - `.nets files`: Network configuration files for SUMO simulations.

## Prerequisites

- **Python** (>= 3.7)
- **SUMO** (Simulation of Urban MObility)
- **Required Python Libraries**:
  - `tensorflow` or `pytorch` (for DQN implementation)
  - `numpy`
  - `matplotlib`
  - `traci`

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your_username/sumo_rl_project.git
   cd sumo_rl_project
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Ensure SUMO is installed and added to your PATH. Refer to the [SUMO installation guide](https://sumo.dlr.de/docs/Installing/index.html) for details.

## Usage

1. Configure the environment and algorithm in the respective script files.

2. Run the desired reinforcement learning algorithm:
   ```bash
   python algorithms/ql_2way-single-intersection.py
   ```
   or
   ```bash
   python algorithms/dqn_2way-single-intersection.py
   ```
   or
   ```bash
   python algorithms/sarsa_2way-single-intersection.py
   ```

4. Review simulation outputs in the `output/` folder and visualize performance metrics.

### Contact
For questions or feedback, please contact [Astha Soni](mailto:asthasoni161@gmail.com).
