# 🚀 Project Name

## 📌 Table of Contents
- [Introduction](#introduction)
- [Demo](#demo)
- [Inspiration](#inspiration)
- [What It Does](#what-it-does)
- [How We Built It](#how-we-built-it)
- [Challenges We Faced](#challenges-we-faced)
- [How to Run](#how-to-run)
- [Tech Stack](#tech-stack)
- [Team](#team)

---

## 🎯 Introduction
We are presenting one of the possible solutions to detect anomalies in financial transactions with the help FlowScope methods on static dataset.

## 🎥 Demo
🔗 [Live Demo](#) (if applicable)  
📹 [Video Demo](#) (if applicable)  
🖼️ Screenshots:

![Screenshot 1](link-to-image)

## 💡 Inspiration
Research on journals and internet resources on various machine learning models used in financial fraud detection. Models that matches our dataset are explored against its alternatives to determine the efficiency and drawbacks.

## ⚙️ What It Does
Our solution does assumption on sample dataset and its features. Our solution includes feature engineering to determine the relativeness of feature details present in the dataset. Based on the suggestion, we can pass the more valued features to model to determine the anomalies. Thus reducing the effort on processing featuring that are not required 

## 🛠️ How We Built It
Feature engineering is built on catBoost gradient descent along with optuna to automate the fine tuning of hyperparameters. Relevant features are then analysed through the principles of FlowScope model.

Temporal aggregation - aggregate transactions by company per week

Behavioral baselining - compute rolling statistics (mean & std) over a 4-week window.

Anomaly detection - use rolling z-scores and a threshold to flag anomalies

Multi-feature modelling - considered multiple features: count, total, avg amount, and transaction types.


## 🚧 Challenges We Faced
Computational resources are high to perform feature engineering, it was using higher memory and disk space. Executed them on Google Collab server running on T4-GPU device.

Higher version of Numpy > 1.23.5 had compatibility issues with catBoost libraries. It is mandatory to use Numpy version 1.23.5.

FlowScope neural network model efficiency on synthetic dataset is less efficient, hence we explored the methods of FlowScope and implemented on our dataset


## 🏃 How to Run
1. Uploaded syntactic dataset. Provide python code recognizes only this dataset. Install the pre-requisites packages.
2. Ensure packages catBoost, Numpy, optuna were installed on the environment.
3. Execute the blocks. 
4. Python script generates csv file that contains company name, risk score and confidence score


## 🏗️ Tech Stack
- 🔹 Backend: Python 


## 👥 Team
- **Kakumani, Venkata Suneel** - [GitHub](#) | [LinkedIn](#)
- **Chandrasekaran, Skandakumar** - [GitHub](#) | [LinkedIn](#)
- **Anandam, Madhu** - [GitHub](#) | [LinkedIn](#)