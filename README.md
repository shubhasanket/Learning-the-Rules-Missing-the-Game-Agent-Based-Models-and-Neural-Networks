# Learning the Rules, Missing the Game: Agent-Based Models and Neural Networks

This repository contains the code for our project on learning agent-based dynamics using machine learning models.

## Authors

- Shubha Sanket Samantaray
- Vibhu Dalal

## Project Overview

In this project, we study whether neural networks trained on data can reliably reproduce the dynamics of interacting systems. We use the synchronous voter model on a graph as a controlled test case and compare three supervised learning models:

- Logistic Regression
- Multilayer Perceptron (MLP)
- Graph Neural Network (GNN)

The models are trained to predict the next state of the system from the current state. We evaluate them at three levels:

1. One-step prediction accuracy
2. Multi-step rollout stability
3. Emergent macroscopic behaviour, especially consensus formation

The main finding is that good one-step prediction does not necessarily imply faithful long-term simulation. Although the models learn the local transition rule reasonably well, their recursive rollouts often drift away from the true agent-based model and fail to reproduce stable consensus behaviour.

## Code

The project code is available in this repository:

[Code Repository](https://drive.google.com/drive/folders/1-VziWdDk6Xid_ugEddWXrZOlz0tOgVA2)

## Report and Plots

A detailed explanation of the methodology, experiments, results, and conclusions is provided in the project report.

The more detailed plots and quantitative results can be found directly in the report:

[Project Report](./Interactions_project.pdf)

## Main Takeaway

Learning accurate local transition rules is not sufficient to recover the long-term dynamics of an interacting system. Capturing emergent behaviour requires models that preserve the structural properties of the original system, such as stochasticity, graph structure, and absorbing states.
