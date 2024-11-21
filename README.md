# Iris Flower Classification 

This project demonstrates how to classify Iris flowers into three species (`Iris-setosa`, `Iris-versicolor`, `Iris-virginica`) using machine learning, specifically TensorFlow. The model is built, trained, and evaluated on the well-known Iris dataset, and various evaluation metrics (accuracy, recall, confusion matrix) are used to assess performance.

---

## Table of Contents

1. [Introduction](#introduction)  
2. [Data Exploration](#data-exploration)  
3. [Data Preprocessing](#data-preprocessing)  
4. [Model Building](#model-building)  
5. [Training and Evaluation](#training-and-evaluation)  
6. [Conclusion](#conclusion)  

---

## Introduction

The Iris dataset is one of the most famous datasets for classification tasks, often used as a benchmark in machine learning. The goal of this project is to predict the species of an Iris flower based on four features:  
- Sepal Length  
- Sepal Width  
- Petal Length  
- Petal Width  

I utilized a simple feed-forward neural network built with **TensorFlow** and train it to classify Iris flowers into one of three species.

---

## Data Exploration

The dataset contains 150 samples of Iris flowers, with four feature columns and one target column (`species`). The species labels are:
- **Iris-setosa**  
- **Iris-versicolor**  
- **Iris-virginica**  

### Key Insights:
- The frequency distribution of each species is visualized.  
- Distributions for features like `petal_length`, `petal_width`, `sepal_length`, and `sepal_width` are analyzed using histograms and pair plots.  
- The data is divided into three main categories based on flower species, and visualizations show clear separations in feature distributions.

---

## Data Preprocessing

1. **Loading the Data**:  
   The dataset is loaded using **Pandas**.  
2. **Label Encoding**:  
   The categorical `species` variable is encoded into numerical labels using **LabelEncoder**.  
3. **Train-Test Split**:  
   The dataset is split into training and testing sets (80-20 split).  
4. **TensorFlow Conversion**:  
   The feature arrays (`X_train`, `X_test`) and label arrays (`y_train`, `y_test`) are converted into **TensorFlow tensors**.

---

## Model Building

We use a simple **Feedforward Neural Network** for the classification task:

- **Layer 1**: Dense layer with 5 units and ReLU activation.  
- **Layer 2**: Dense layer with 3 units and ReLU activation.  
- **Output Layer**: Dense layer with 3 units to represent the three classes.  

The model is compiled with the **Sparse Categorical Cross-Entropy** loss function and the **Adam optimizer**.  

---

## Training and Evaluation

1. **Training Loop**:  
   - The model is trained for **200 epochs**.  
   - The loss is calculated during each epoch and plotted for visualization.  

2. **Test Loss**:  
   The final test loss is calculated after training, using the test data.  

3. **Prediction**:  
   The model is used to predict the class of new, unseen data.  

4. **Metrics**:  
   The following metrics are calculated:  
   - **Accuracy**: The percentage of correct predictions.  
   - **Recall**: The ability to identify all relevant instances.  
   - **Confusion Matrix**: A table to evaluate the performance of the classification algorithm.

---

## Conclusion

This project demonstrates the power of neural networks for solving classification problems. Key takeaways include:  
1. **Model Performance**: The neural network model performs well with a high accuracy score and reasonable recall.  
---
