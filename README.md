# Reinforcement Learning-Based Distributed Server Load Balancer

## 📌 Introduction
The increasing demand for computational resources in cloud computing environments necessitates efficient load balancing solutions. Traditional approaches struggle with scalability and adaptability. This project integrates **Reinforcement Learning (RL)** into a **Distributed Server Load Balancer** to optimize resource utilization dynamically.

Using the **Multi-Agent Deep Deterministic Policy Gradient (MADDPG)** algorithm, the system improves performance and enhances resource management. The experimental setup includes **35 users and 10 servers**, showcasing improved load distribution.

🔗 **GitHub Repository:** https://github.com/xtremislv/Reinforcement-Learning-Based-Distributed-Server-Load-Balancer

## 📊 Key Features

- **Dynamic Load Balancing:** Real-time allocation of user requests across multiple servers.
- **Multi-Agent RL Approach:** Implements **MADDPG** for distributed decision-making.
- **Optimized Resource Utilization:** Efficiently distributes computational tasks to balance server load.
- **Scalable Environment:** Capable of handling multiple users and servers.

## 🛠️ System Architecture

1. **Environment:** Users interact with servers to complete computational tasks.
2. **User States:**
   - Start task
   - Task in transmission
   - Task processing
   - Task return
   - Disconnection
   - Task migration
3. **State Variables:**
   - Bandwidth availability
   - Server resources
   - User connections
   - User location
4. **Actions:**
   - Resource Allocation
   - Bandwidth Allocation
   - Task Offloading

## 📐 MADDPG Algorithm

The **Multi-Agent Deep Deterministic Policy Gradient (MADDPG)** algorithm extends **DDPG** to a multi-agent setting:

- **Decentralized Actor:** Learns individual policies for each agent.
- **Centralized Critic:** Evaluates joint actions for better coordination.
- **Shared Replay Buffer:** Collects experiences from all agents for training.
- **Target Networks:** Stabilizes learning through slowly updated networks.

## 📊 Experimental Setup & Results

- **Configuration 1:** 35 users, 10 servers (resource limit: 4)
- **Configuration 2:** 35 users, 20 servers (resource limit: 4)

### 🧪 Results:
- Improved load distribution and reduced latency.
- Enhanced system throughput with adaptive decision-making.

## 🧰 Technology Stack

- **Python** (TensorFlow, Keras, PyTorch)
- **Data Processing:** Pandas, NumPy
- **Visualization:** Matplotlib
- **Simulation Data:** CRAWDAD dataset

## 📈 Challenges Faced

- **Environment Simulation:** Accurately replicating real-world cloud dynamics.
- **Data Quality:** Handling missing and noisy datasets.
- **Training Time:** High computational demand for RL convergence.

## 🚀 Future Scope

- Explore heterogeneous servers requiring **multi-actor, multi-critic** models.
- Optimize resource consumption for energy efficiency.
