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

## Key Features

- **Offline RL**: Trains a PPO (Proximal Policy Optimization) model using a fixed dataset.
- **Fairness Integration**: Applies a fairness penalty in the reward signal to ensure demographic parity.
- **Human Feedback**: Integrates simulated user preferences to align with RLHF approaches.
- **Fairness Evaluation**: Uses `fairlearn` to compute fairness metrics like **Demographic Parity Difference (DPD)**.

---

## Repository Structure


/src
├── preprocess_data.py
│   └─ Preprocesses the raw dataset (shopping_behavior_updated.csv) and saves it as preprocessed_shopping_data.csv.
│
├── train_model.py
│   └─ Trains a PPO model using the preprocessed data and saves it as ppo_shopping_model.zip.
│
├── evaluate_fairness.py
│   └─ Evaluates the fairness of the model's recommendations using fairlearn and visualizes results.
│
├── incorporate_human_feedback.py
│   └─ Fine-tunes the model with simulated human feedback and saves it as ppo_shopping_model_with_feedback.zip.
│
└── README.md
    └─ This file, providing an overview and usage instructions.
```



---

## Prerequisites

- Python **3.8+**
- Recommended: Run in **Google Colab**
- Install dependencies manually:

```bash
pip install pandas numpy gymnasium stable-baselines3 scikit-learn fairlearn matplotlib seaborn google-colab
