# AI-Driven Predictive Failure Detection in Progressive Kubernetes Deployments

## Project Overview
This repository contains the machine learning experiments for our research project at the University of Sri Jayewardenepura.

Our goal is to develop an AI-based approach to predict potential failures during progressive Kubernetes deployments.

## Current Implementation
We have developed an initial log classification pipeline using:

- Random Forest
- XGBoost
- TF-IDF feature extraction
- Google Colab

## Dataset
- 13,300 log records
- 89 unique log patterns
- Normal/non-server-error logs (Class 0)
- Server-error logs (Class 1)
- Includes synthetic error logs

## Model Evaluation
The Random Forest model achieved 91.82% accuracy on an unseen-pattern split, but server-error recall was only 3.74%.

This indicates that additional data diversity and model improvements are required.

XGBoost training has been completed, with evaluation to follow.

## Future Work
- Compare machine learning algorithms
- Improve log dataset diversity
- Collect real-time logs using Loki and Prometheus
- Extract time-based features during canary deployments
- Predict failure risks and support continue, pause, or rollback decisions

## Technologies
Python, Scikit-learn, XGBoost, Google Colab, Kubernetes, Prometheus, Loki and Grafana.
