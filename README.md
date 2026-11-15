AI in Cybersecurity – Lab Assignment 3

Neural Network-Based Cyber Activity Classification

This repository contains my Lab Assignment 3 for AI in Cybersecurity. The project focuses on understanding neural network concepts and implementing a Dense Neural Network to classify cyber activities as Normal or Attack.

📌 Project Overview

The objective of this assignment is to build and evaluate a neural network model for basic cyber activity classification using Python and TensorFlow.

The notebook covers data preprocessing, feature scaling, neural network training, model evaluation, new predictions, and comparison with a Decision Tree classifier.

🎯 Objectives

Understand CNN, RNN/LSTM, GAN and Dense Neural Network concepts.
Prepare and preprocess a cybersecurity dataset.
Split data into training and testing sets.
Apply feature normalization using StandardScaler.
Build and train a Dense Neural Network.
Visualize training and validation accuracy and loss.
Predict whether new cyber activities are Normal or Attack.
Compare Neural Network and Decision Tree performance.
🛠️ Technologies Used

Python
Google Colab
NumPy
Pandas
Matplotlib
TensorFlow / Keras
Scikit-learn
📂 Dataset Information

The project uses a cybersecurity activity dataset containing 100 records.

Input Features:

failed_logins – Number of failed login attempts.
login_hour – Hour at which login activity occurs.
new_device – Indicates whether a new device is detected.
data_transfer_mb – Amount of data transferred in MB.
Target Variable:

0 – Normal Activity
1 – Attack Activity
The record_id column is excluded from model training because it is an identifier.

🧠 Model Architecture

A Dense Neural Network with the following architecture is implemented:

4 → 8 → 4 → 1

Layer	Configuration
Input Layer	4 Features
Hidden Layer 1	8 Neurons (ReLU)
Hidden Layer 2	4 Neurons (ReLU)
Output Layer	1 Neuron (Sigmoid)
Training Configuration:

Optimizer: Adam
Loss Function: Binary Crossentropy
Evaluation Metric: Accuracy
Epochs: 20
Batch Size: 8
Validation Split: 20%
⚙️ Implementation Workflow

Import required Python libraries.
Upload and load the cybersecurity CSV dataset.
Select input features and target labels.
Split the dataset into 75% training and 25% testing data.
Normalize features using StandardScaler.
Build and train the Dense Neural Network.
Plot training and validation accuracy and loss.
Evaluate the model using test data.
Predict classifications for three new cyber activity records.
Compare Neural Network results with a Decision Tree classifier.
📊 Model Evaluation

The assignment evaluates model performance using:

Training Accuracy
Validation Accuracy
Testing Accuracy
Training and Validation Loss
Classification Report
Confusion Matrix
Decision Tree Accuracy Comparison
Actual evaluation results are available in the Jupyter Notebook after execution.

🚀 How to Run

Option 1: Google Colab

Download the .ipynb notebook from this repository.
Open Google Colab.
Upload the notebook.
Run all cells sequentially.
Upload the required simple_cyber_activity.csv dataset when prompted.
Review the generated outputs, graphs, and predictions.
Option 2: Jupyter Notebook

Clone this repository.
Install the required dependencies.
Open the notebook in Jupyter.
Run the cells in order and provide the dataset when prompted.
