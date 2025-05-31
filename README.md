
# 🤖 Customer Satisfaction Prediction using Machine Learning

This project aims to **predict customer satisfaction** by analyzing historical support and service data using machine learning models. It provides valuable insights into what drives customer experience and allows organizations to proactively manage satisfaction levels.

---

## 📊 Project Overview

Customer satisfaction is a key indicator of a company’s health and performance. This project leverages machine learning techniques to analyze support ticket data and identify patterns that lead to dissatisfaction or delight.

### Objectives:

* Predict customer satisfaction based on past interactions
* Understand key factors driving customer sentiment
* Enable early interventions to improve service quality

---

## 🗂️ Dataset Description

The dataset includes **customer support records** with the following features:

| Feature                     | Description                                          |
| --------------------------- | ---------------------------------------------------- |
| `Customer ID`               | Unique identifier for each customer                  |
| `Age`, `Gender`, `Location` | Demographic info                                     |
| `Product Purchased`         | Product or service used                              |
| `Ticket Type`               | Nature of support ticket (technical, billing, etc.)  |
| `Issue Description`         | Text-based problem reported                          |
| `Response Time (hours)`     | Time taken to respond                                |
| `Resolution Time (hours)`   | Time taken to resolve                                |
| `Customer Satisfaction`     | Target variable (e.g., Satisfied/Unsatisfied or 1/0) |

---

## 🧪 Methodology

1. **Data Preprocessing**

   * Cleaned missing values
   * Encoded categorical variables
   * Normalized numerical features
   * Extracted features from text (e.g., TF-IDF from `Issue Description`)

2. **Exploratory Data Analysis (EDA)**

   * Visualized satisfaction distribution
   * Analyzed trends by ticket type, product, and response time
   * Identified key correlations

3. **Modeling**

   * Tried classification models:

     * Logistic Regression
     * Random Forest
     * Gradient Boosting
     * Support Vector Machines (SVM)
   * Chose best model based on:

     * Accuracy, Precision, Recall, F1-Score
     * ROC-AUC Curve

4. **Model Interpretation**

   * Used SHAP and feature importance plots to explain model decisions
   * Highlighted top drivers of satisfaction

---

## 📈 Results

* Best model achieved **X% accuracy** and **Y% F1-score** on validation data.
* Key factors influencing satisfaction:

  * Faster response & resolution times
  * Clear communication in issue descriptions
  * Type of ticket (e.g., technical issues had lower satisfaction)

---

## 📁 Project Structure

```
customer-satisfaction-prediction/
│
├── data/                   # Raw and processed datasets
├── notebooks/              # Jupyter notebooks for EDA and modeling
├── models/                 # Saved model objects (pickle files)
├── utils/                  # Helper functions
├── plots/                  # Charts and visuals
├── main.py                 # Pipeline to train and evaluate model
├── requirements.txt        # Python dependencies
└── README.md               # Project documentation
```

---

## ⚙️ Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/customer-satisfaction-prediction.git
   cd customer-satisfaction-prediction
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Run the notebook or main script:

   ```bash
   jupyter notebook
   # or
   python main.py
   ```

---

## 🧠 Technologies Used

* Python (Pandas, NumPy, Matplotlib, Scikit-learn)
* Natural Language Processing (TF-IDF, text cleaning)
* Machine Learning (classification models)
* SHAP for interpretability

---

