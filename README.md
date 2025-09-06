# Behavioral Cloning & DAgger for Imitation Learning (MuJoCo, CS285 Inspired)

This project implements **imitation learning** techniques — **Behavioral Cloning (BC)** and **DAgger (Dataset Aggregation)** — to train locomotion agents in MuJoCo.  
It is based on the [CS285 Homework 1 assignment](https://rail.eecs.berkeley.edu/deeprlcourse/deeprlcourse/static/homeworks/hw1.pdf) from UC Berkeley’s Deep Reinforcement Learning course.

---

## 📌 Overview
- **Behavioral Cloning (BC):**  
  - Supervised learning approach using expert demonstrations only.  
  - Agents copy expert trajectories but often fail to generalize to unseen states.  

- **DAgger (Dataset Aggregation):**  
  - Iteratively queries the expert during training to add new corrective data.  
  - Prevents compounding errors and improves long-horizon stability.  

---

## 🚀 Results

### 🐜 Ant-v4
- **Behavioral Cloning:** The agent initially learns a **crawling gait**.  
  ![Ant crawling gait](https://i.imgur.com/aUkDuvV.gif)  
- **DAgger:** With aggregated corrections, the agent learns a much more natural **bounding gait**.  
  ![Ant bounding gait](https://i.imgur.com/6cWj1Mu.gif)  

---

### 🚶 2D Walker
- **Behavioral Cloning:** The walker struggles to balance and **falls over**.  
  ![Walker falling](https://i.imgur.com/kG9AQ5i.gif)  
- **DAgger:** The walker achieves a surprisingly stable and **cartoonish running gait**.  
  ![Walker running](https://i.imgur.com/kAIqnzB.gif)  

---

## 🛠️ Tech Stack
- **Languages:** Python  
- **Frameworks/Tools:** PyTorch, Gymnasium, MuJoCo  
- **Algorithms:** Behavioral Cloning, DAgger  

---

## 📚 Learning Outcomes
- Implemented **policy cloning with supervised learning** on expert trajectories.  
- Demonstrated the **compounding error problem** in BC.  
- Showed how **DAgger improves locomotion stability** by continuously querying the expert.  

---

## 🔗 References
- [CS285 Deep RL Course – Homework 1](https://rail.eecs.berkeley.edu/deeprlcourse/deeprlcourse/static/homeworks/hw1.pdf)  
- [DAgger: Dataset Aggregation](https://arxiv.org/abs/1011.0686)  

