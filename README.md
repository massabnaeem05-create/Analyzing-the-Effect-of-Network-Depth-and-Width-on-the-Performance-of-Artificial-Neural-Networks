# Analyzing the Effect of Network Depth and Width on ANN Performance

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Scikit-Learn](https://img.shields.io/badge/Library-Scikit--Learn-orange)
![Status](https://img.shields.io/badge/Project-Completed-brightgreen)
![License](https://img.shields.io/badge/License-MIT-lightgrey)



  Project Overview

In this project, I investigated how the architecture of an Artificial Neural Network (ANN) influences its performance, focusing on two main aspects: depth (number of hidden layers) and width (number of neurons per layer).

Instead of only relying on theory, I implemented multiple models and compared their performance using a custom dataset. This helped me understand how increasing complexity affects accuracy, learning behaviour, and generalisation.



  Project Visualizations

  Effect of Network Complexity

![Effect of Network Complexity](graphs/effect_of_network_complexity.png)

This graph shows how different ANN architectures perform. Simpler models tend to underfit, while increasing the number of neurons improves accuracy. However, adding more layers results in only small improvements, showing diminishing returns.



###  Training Loss Behaviour

![Training Loss](graphs/training_loss.png)

This graph illustrates how loss decreases during training. The smooth downward curve indicates stable learning and proper convergence of the model.



###  Accuracy vs Model Complexity

![Accuracy vs Complexity](graphs/accuracy_vs_complexity.png)

This graph shows how accuracy changes with increasing complexity. Performance improves as the model becomes more expressive, but excessive complexity can lead to overfitting.



##  Objectives

* Analyze the impact of network depth
* Evaluate the effect of increasing width
* Understand underfitting and overfitting
* Explore the bias-variance trade-off
* Identify an optimal ANN architecture



## Dataset

* 2000 samples
* Features: study hours, attendance, previous performance
* Output: pass/fail (binary classification)
* Includes noise to simulate real-world data



##  Model Used

* MLPClassifier (Scikit-learn)

### Configurations Tested:

* (3,) → shallow network
* (5,) → wider network
* (5,5) → deeper network

### Key Parameters:

* max_iter = 500
* random_state = 42



##  Methodology

1. Split dataset into training and testing sets
2. Train models with different architectures
3. Evaluate performance using accuracy
4. Compare results using graphs



##  Code Approach

* Define multiple ANN configurations
* Use a loop to train models
* Store accuracy results
* Compare performance efficiently



##  Key Findings

* Small models → underfitting
* Moderate models → best performance
* Large models → diminishing returns
* Best results come from balanced complexity



##  How to Run

Clone the repository:
git clone https://github.com/massabnaeem05-create/Analyzing-the-Effect-of-Network-Depth-and-Width-on-the-Performance-of-Artificial-Neural-Networks

Install dependencies:
pip install numpy pandas scikit-learn matplotlib

Run the project:
python main.py



##  Project Structure

├── main.py
├── graphs/
│   ├── effect_of_network_complexity.png
│   ├── training_loss.png
│   ├── accuracy_vs_complexity.png
├── README.md



##  Author

Massab Bin Naeem



##  Conclusion

This project shows that increasing ANN complexity improves performance only up to a certain point. The best model is not the largest one, but the one that balances accuracy and generalisation.



