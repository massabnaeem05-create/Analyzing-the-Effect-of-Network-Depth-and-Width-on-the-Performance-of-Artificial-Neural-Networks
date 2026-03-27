# Analyzing the Effect of Network Depth and Width on the Performance of Artificial Neural Networks

## Overview
This project explores how the architecture of an Artificial Neural Network (ANN) affects its performance. The focus is on two key factors:

- **Depth**: Number of hidden layers  
- **Width**: Number of neurons in each layer  

Different ANN configurations are tested to analyse how model complexity impacts accuracy, learning behaviour, and generalisation.

---

## GitHub Repository
You can access the full project here:  
https://github.com/massabnaeem05-create/Analyzing-the-Effect-of-Network-Depth-and-Width-on-the-Performance-of-Artificial-Neural-Networks

---

## Objectives
- Analyse how network depth affects model performance  
- Evaluate the impact of width on learning capacity  
- Compare different ANN configurations  
- Understand underfitting and overfitting  
- Identify the best balance between model complexity and performance  

---

## Dataset
A custom dataset (`student_data_2000_unique.csv`) is used.

### Features:
- Study Hours  
- Attendance  
- Previous Score  

### Target:
- Pass / Fail (Binary classification)

---

## Model Used
Multilayer Perceptron (MLPClassifier) from Scikit-learn.

---

## Model Configurations
The following ANN architectures were tested:

- (3,) → Single hidden layer with 3 neurons  
- (5,) → Single hidden layer with 5 neurons  
- (5,5) → Two hidden layers with 5 neurons each  

---

## Methodology
The project follows these steps:

1. Load dataset  
2. Split data into training and testing sets  
3. Apply feature scaling using StandardScaler  
4. Train ANN models with different configurations  
5. Evaluate performance using accuracy  
6. Visualise results using graphs  

---

## Code Example
   model = MLPClassifier(hidden_layer_sizes=config, max_iter=500, random_state=42)
    model.fit(X_train, y_train)
    
    y_pred = model.predict(X_test)
    acc = accuracy_score(y_test, y_pred)
    
    print(f"Model {config} Accuracy: {acc:.4f}")
