
# 🏠 Boston Housing Price Prediction using Neural Network (Regression)

## 📌 Project Overview

This project implements a **Neural Network Regression model** using **TensorFlow (Keras)** to predict house prices from the **Boston Housing dataset**.
The task is a **supervised regression problem**, where the output is a continuous value representing the median house price.

---

## 📂 Dataset Description

* **Dataset Name:** Boston Housing Dataset
* **Source:** TensorFlow / Keras built-in dataset
* **Total Samples:** 506
* **Training Samples:** 404
* **Testing Samples:** 102
* **Number of Input Features:** 13
* **Target Variable:** Median value of owner-occupied homes (in $1000s)

All features are numerical and directly used as input to the neural network.

---

## ⚙️ Technologies Used

* Python
* TensorFlow / Keras
* NumPy
* Jupyter Notebook

---

## 🧪 Data Preprocessing

* The dataset is loaded directly using TensorFlow’s dataset API.
* No feature normalization or standard deviation scaling is applied.
* Raw numerical feature values are fed directly into the neural network.
* The default train-test split provided by Keras is used.

> **Note:** The model is trained without normalization to demonstrate basic neural network regression using raw input features.

---

## 🧠 Model Architecture

The neural network model is defined using Keras `Sequential` API with the following structure:

* **Input Layer:**

  * Accepts 13 numerical features
* **Hidden Layer:**

  * Dense layer with 10 neurons
* **Output Layer:**

  * Dense layer with 1 neuron (regression output)

The model uses a simple feed-forward architecture suitable for introductory regression tasks.

---

## ⚡ Model Configuration

* **Random Seed:** 42 (for reproducibility)
* **Optimizer:** Adam
* **Loss Function:** Mean Absolute Error (MAE)
* **Evaluation Metric:** Mean Absolute Error (MAE)

MAE is used as both the loss function and evaluation metric since it directly measures prediction error in regression tasks.

---

## 🚀 Model Training

* **Epochs:** 100
* **Batch Size:** Default
* **Training Data:** `x_train`, `y_train`

The model learns to minimize the absolute difference between predicted and actual house prices over multiple epochs.

---

## 📊 Model Evaluation

The trained model’s performance is evaluated using **Mean Absolute Error (MAE)**.

* MAE represents the average absolute difference between predicted and true house prices.
* Lower MAE values indicate better predictive performance.

---

## 🔮 Prediction

After training, the model can be used to predict housing prices for unseen test data samples.
Predicted values are continuous and represent estimated house prices.

---

## 📁 Project Structure

* `Boston_housing_dataset.ipynb`

  * Dataset loading
  * Neural network model creation
  * Model compilation
  * Training and evaluation

---

## 🎓 Learning Outcomes

* Understanding neural networks for regression problems
* Implementing a simple feed-forward neural network using Keras
* Using MAE as a loss function for regression
* Training neural networks without normalization
* Interpreting regression model performance

---

## 📌 Conclusion

This project demonstrates a basic neural network regression model trained on the Boston Housing dataset without applying feature normalization or standard deviation scaling. Despite the simplicity of the architecture, the model is capable of learning meaningful patterns and predicting housing prices with reasonable accuracy.

