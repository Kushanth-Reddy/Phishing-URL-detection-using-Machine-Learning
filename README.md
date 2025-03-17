# **Phishing Website Detection by Machine Learning Techniques**

## **Overview**

This notebook demonstrates the implementation of machine learning techniques to detect phishing websites. Phishing websites are malicious sites designed to steal sensitive information such as usernames, passwords, and credit card details. By analyzing various features of URLs and website behavior, machine learning models can classify websites as legitimate or phishing.

---

## **Dataset**

The dataset used in this notebook contains labeled data with features extracted from URLs. Each row represents a website, and the features include:

- **Ranking**: Website ranking based on popularity.
- **Is IP**: Whether the URL contains an IP address.
- **Valid**: Validity of the URL.
- **Active Duration**: Duration for which the website has been active.
- **URL Length**: Length of the URL.
- **Contains '@'**: Whether the URL contains the '@' symbol.
- **Is Redirect**: Whether the URL redirects to another page.
- **Contains Dash**: Whether the URL contains a dash ('-').
- **Domain Length**: Length of the domain name.
- **Number of Subdomains**: Count of subdomains in the URL.

The target variable indicates whether the website is phishing (`1`) or legitimate (`0`).

---

## **Steps in the Notebook**

### **1. Objective**

- Extract and preprocess features from website URLs.
- Train and evaluate machine learning models for phishing website detection.
- Compare the performance of different models to identify the most effective approach.

### **2. Data Loading**

- Load the dataset into a Pandas DataFrame.
- Display the first few rows to understand the structure of the data.

### **3. Data Preprocessing**

- Handle missing values, if any.
- Normalize or scale numerical features to ensure uniformity.
- Encode categorical features, if applicable.

### **4. Visualizing the data**

- Few plots and graphs are displayed to find how the data is distributed and the how features are related to each other.

### **5. Exploratory Data Analysis (EDA)**

- Visualize the distribution of features.
- Analyze correlations between features and the target variable.
- Identify any patterns or anomalies in the data.

### **6. Feature Selection**

- Select the most relevant features for training the models.
- Use techniques like correlation analysis or feature importance scores.

### **7. Model Training**

- Train multiple machine learning models, such as:
  - Logistic Regression
  - Decision Trees
  - Random Forest
  - Support Vector Machines (SVM)
  - Gradient Boosting (e.g., XGBoost, LightGBM)
  - Naive Bayes
  - Hybrid Models (LR-SVC, LR-DT, LR-SVC-DT, XGB-LR-SVC-DT)
- Split the data into training and testing sets to evaluate model performance.

- Evaluate models using metrics such as:
  - Accuracy
  - Precision
  - Recall
  - F1-Score
- Compare the performance of different models.

### **8. Comparision of Models**

- To compare the models performance, a dataframe is created. The columns of this dataframe are the lists created to store the results of the model.

### **9. Final Model Selection**

- Select the best-performing model based on evaluation metrics.
- Save the trained model for deployment.

---

## **Dependencies**

The following Python libraries are used in this notebook:

- `pandas`: For data manipulation and analysis.
- `numpy`: For numerical computations.
- `matplotlib` and `seaborn`: For data visualization.
- `scikit-learn`: For machine learning model implementation and evaluation.

---
