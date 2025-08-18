---
title: "Machine Learning in MATLAB"
excerpt: "Clustering and reinforcement learning with k-means, DBSCAN, and Value Iteration in MATLAB.<br/><img src='/images/portfolio/ml_ul_rl.png'>"
collection: portfolio
date: 2023-07-14
---

## Overview
As part of the *Machine Learning* course at HTWG Konstanz, I worked on two hands-on projects involving **unsupervised learning** (clustering) and **reinforcement learning**.  
The tasks were implemented and analyzed using **MATLAB**, focusing on applying machine learning techniques in real-world inspired scenarios with structured evaluations.

## Unsupervised Learning: Clustering Animal Data

Using a dataset of 342 animals with 7 features each, I applied and compared **k-means** and **DBSCAN** clustering methods. The goal was to match clusters as closely as possible to the true animal classes.  
→ [**Clustering Repository**](https://github.com/cfeng-dev/Species_Clustering_Analysis)

### Methods & Insights
- **Data preprocessing:** feature selection (columns 4–6), z-score normalization
- **k-means:** 3 clusters assumed, `sqEuclidean` distance, relabeling for evaluation  
- **DBSCAN:** parameter tuning for `epsilon` and `MinPts`, noise filtering
- **Evaluation:** confusion matrix for both algorithms

## Reinforcement Learning: Value Iteration & Policy Evaluation

A custom **Markov Decision Process (MDP)** with 12 states and 4 actions was implemented in MATLAB.  
The task included computing the value function under a fixed policy (“always move up”), and using **Value Iteration** to derive the optimal policy.  
→ [**Reinforcement Learning Repository**](https://github.com/cfeng-dev/Path_Seeker)

### Methods & Implementation
- Created a grid-world-like MDP in MATLAB
- Implemented the Bellman equation for policy evaluation
- Developed a custom **Value Iteration** function
- Compared policies and value functions across iterations
