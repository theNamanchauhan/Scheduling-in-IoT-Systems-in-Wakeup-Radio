# Adaptive Energy-Efficient Control of IoT Wake-Up Radio Systems using Deep Reinforcement Learning and DQN

This project focuses on enhancing energy efficiency in IoT networks by implementing intelligent scheduling for wake-up radio systems. Utilizing **Deep Q-Networks (DQN)** and **Reinforcement Learning (RL)** techniques, this model aims to optimize wake-up schedules, reduce energy consumption, and prolong the lifespan of IoT devices. This framework has broad applications in IoT systems across domains such as smart homes, healthcare, and transportation.

## Project Overview

IoT wake-up radio systems are crucial for managing device power states efficiently. This research uses a DQN-based RL model to intelligently schedule wake-up events, balancing system performance with minimized energy demand. 

### Key Features
- **RL and DQN Framework**: Trains an RL agent to optimize scheduling decisions using system state data, sensor battery levels, and statistical patterns.
- **Custom Simulation Environment**: Developed with OpenAI’s Gymnasium and Stable Baselines 3 for seamless model testing and training.
- **Model Comparisons**: Includes baseline algorithms (Random, Round-Robin, Q-Learning) to evaluate the performance of the DQN model.
- **Performance Metrics**: Assesses average reward, time latency, and scheduling efficiency across different algorithms.

## Methodology

### 1. Environment Setup
The custom environment simulates a wireless sensor network, where sensor nodes respond to scheduling requests based on state data and wake-up protocols.

### 2. Scheduling Algorithms
The project evaluates the following scheduling algorithms:
- **Random Scheduler**: Baseline scheduler with random event allocation.
- **Round Robin**: Cycles through all sensors for fair event distribution.
- **Q-Learning**: Reinforcement-based scheduler for improved selection.
- **Deep Q-Network (DQN)**: Utilizes a neural network to model optimal scheduling actions.
- **Stable Baselines 3**: A robust, pre-trained DQN model to evaluate further optimization potential.

### 3. Metrics and Evaluation
The effectiveness of each algorithm is analyzed based on:
- **Reward scores** (indicating efficiency of energy use),
- **Latency** (response time for scheduling events),
- **Energy efficiency** (sensor battery optimization).

## Results

The DQN model demonstrated significant improvements in managing wake-up schedules with a lower average latency and increased reward scores compared to baseline methods. However, Round Robin achieved slightly better minimum latency in some cases. This highlights the trade-offs between different scheduling techniques.

## Future Scope

Future work will focus on integrating more complex environmental factors, real-world testing, and alternative RL architectures to further enhance scheduling adaptability in IoT networks.

## Getting Started

### Prerequisites
- Python 3.x
- Gymnasium (OpenAI Gym)
- Stable Baselines 3
- PyTorch

### Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/IoT-WakeUp-Radio-DQN.git
    ```
2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

### Usage
1. Run the simulation with:
    ```bash
    python main.py
    ```
2. Adjust hyperparameters in the configuration file as needed.

## Contributing

Please submit a pull request or open an issue if you'd like to contribute!
