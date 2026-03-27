# Analyzing the Effect of Network Depth and Width on the Performance of Artificial Neural Networks

## Overview
This project investigates how the architecture of an Artificial Neural Network (ANN) influences its performance. The focus is on two key factors:

- Depth: Number of hidden layers  
- Width: Number of neurons in each layer  

Different ANN configurations are tested to analyse how model complexity affects prediction accuracy and learning behaviour.

## Objective
- Analyse the impact of network depth and width  
- Compare shallow and deep neural networks  
- Study how increasing neurons affects performance  
- Understand the balance between underfitting and overfitting  

## Dataset
A custom dataset containing 2000 rows is used.

Features:
- Study Hours  
- Attendance  
- Previous Scores  

Target:
- Pass / Fail (Binary classification)

## Model Used
Multilayer Perceptron (MLPClassifier)

Configurations:
- (3,)
- (5,)
- (5,5)

## Methodology
1. Load dataset  
2. Split data  
3. Apply scaling  
4. Train models  
5. Evaluate accuracy  
6. Plot graphs  

## Graphs
1. Accuracy Comparison  
2. Loss Curve  
3. Model Comparison  
4. Accuracy vs Complexity  
5. Study Hours vs Pass/Fail  

## How to Run
pip install pandas scikit-learn matplotlib  
python ann_model.py  

## Project Structure
dataset/  
code/  
report/  
README.md  

## Author
Massab Naeem
