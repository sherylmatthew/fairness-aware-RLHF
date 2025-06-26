# 🎯 Fair-RLHF: Fairness-Aware Offline Reinforcement Learning with Human Feedback

This repository contains the code for the paper **"Fairness-Aware Offline Reinforcement Learning with Human Feedback (Fair-RLHF): Mitigating Bias in Human Preferences"**.

The project develops a fairness-aware offline reinforcement learning model for **shopping recommendations**, aiming to mitigate bias in **human preferences across sensitive attributes**, specifically **Gender**.

---

## 📌 Project Overview

This work builds a **fair recommendation system** using **Offline Reinforcement Learning (RL)** and **Human Feedback (RLHF)**. The system suggests product categories like *Clothing* and *Footwear* while enforcing fairness in treatment across gender groups.

### Key Goals:
- Reduce recommendation bias through fairness-aware RL.
- Incorporate **simulated human preferences** into learning (RLHF).
- Evaluate model fairness using **Demographic Parity**.

---

## 🚀 Key Features

- **Offline RL**: Trains a PPO (Proximal Policy Optimization) model using a fixed dataset.
- **Fairness Integration**: Applies a fairness penalty in the reward signal to ensure demographic parity.
- **Human Feedback**: Integrates simulated user preferences to align with RLHF approaches.
- **Fairness Evaluation**: Uses `fairlearn` to compute fairness metrics like **Demographic Parity Difference (DPD)**.

---

## 🗂️ Repository Structure

