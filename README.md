
---

# **Weather Classification Model**

### **Description**
This project aims to predict the type of weather based on several atmospheric and environmental factors. The dataset used for this project was sourced from Kaggle, and the model is built using Support Vector Machines (SVM) with GridSearch to optimize hyperparameters. The model achieved an accuracy of 91%.

### **Library Used**
The following library are used in this project:
- **Pandas**
- **Numpy**
- **Seaborn**
- **Matplotlib**
- **Sklearn**

### **Dataset**
The dataset was obtained from Kaggle: https://www.kaggle.com/datasets/nikhil7280/weather-type-classification 
It includes the following features:
- **Temperature**
- **Humidity**
- **Wind Speed**
- **Precipitation**
- **Cloud Cover**
- **Atmospheric Pressure**
- **UV Index**
- **Season**
- **Visibility**
- **Location**

The target variable is the **weather type**, which the model predicts based on these features.

### **Feature Engineering**
Dummy variables were created for the following categorical features:
- **Cloud Cover**
- **Season**
- **Location**

These dummy variables were necessary to allow the SVM model to handle categorical data effectively.

### **Modeling Approach**
We used a **Support Vector Machine (SVM)** for weather classification. The model's performance was optimized using **GridSearchCV** to find the best combination of the `C` and `gamma` hyperparameters.

- **Hyperparameters Tuned**:
  - `C`: [0.1, 1, 10, 100, 1000]
  - `gamma`: [1, 0.1, 0.01, 0.001, 0.0001]

### **Model Performance**
The final model achieved an accuracy of **91%** on the test set, demonstrating good performance in classifying weather types based on the given features.


---
