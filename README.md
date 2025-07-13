# PREDICTIVE-ANALYSIS-USING-MACHINE-LEARNING

*COMPANY* : CODTECH IT SOLUTIONS

*NAME* : BABULAL JANGID

*INTERN ID* : CT06DF2423

*DOMAIN* : DATA ANALYTICS

*DURATION* : 6 WEEKS

*MENTOR* : NEELA SANTOSH


# 🤖 Predictive Analysis Using Machine Learning – Walmart Dataset

This repository contains Task 2 of a data analytics internship project, focusing on predictive analysis using **Machine Learning**. The task involves building a classification model using **scikit-learn** in **Google Colab** to predict whether a Walmart store's weekly sales are considered **high** or **low** based on various external and internal features.

---

## 📌 Objective

The goal of this project is to:
- Perform end-to-end machine learning on the Walmart Sales dataset.
- Create a binary target label for sales performance.
- Use a classification algorithm to predict high-performing sales weeks.
- Analyze and visualize key factors affecting predictions.

---

## 📁 Dataset Used

- **Dataset Name**: Walmart Retail Sales Forecasting
- **Source**: [Kaggle](https://www.kaggle.com/)
- **File**: `Walmart_Sales.csv`

### Key Features:
- `Store`: Store ID
- `Date`: Weekly record
- `Weekly_Sales`: Total sales during the week
- `Holiday_Flag`: 1 if the week includes a holiday
- `Temperature`: Weather temperature
- `Fuel_Price`: Fuel cost in the area
- `CPI`: Consumer Price Index
- `Unemployment`: Local unemployment rate

---

## 🛠️ Technologies Used

- **Python 3.x**
- **Google Colab**
- **Pandas, NumPy** – Data manipulation
- **Matplotlib, Seaborn** – Visualization
- **scikit-learn** – Machine learning (Logistic Regression, scaling, evaluation)

---

## 🔍 Key Tasks Performed

1. **Data Cleaning**:
   - Handled missing values
   - Removed unnecessary columns (e.g., `Date` and `Weekly_Sales` to avoid leakage)

2. **Feature Engineering**:
   - Created a new binary column `High_Sales`
   - Defined threshold using the mean of `Weekly_Sales`

3. **Train-Test Split & Preprocessing**:
   - Used `train_test_split()` to create training and test sets
   - Applied `StandardScaler` for normalization

4. **Modeling**:
   - Trained a `LogisticRegression` model
   - Predicted `High_Sales` on test data

5. **Evaluation**:
   - Accuracy: **~61.3%**
   - Classification Report and Confusion Matrix
   - Predicted new sample sales classification

6. **Visualization**:
   - Distribution of `Weekly_Sales` with mean line
   - Heatmap of feature correlations
   - Top 10 stores by average weekly sales

---

## 📊 Insights

- The Logistic Regression model achieved reasonable accuracy with balanced precision and recall.
- Some features like CPI and Unemployment had low correlation with weekly sales.
- Store-wise performance varies significantly, with a few stores consistently outperforming others.
- Sales are not necessarily higher during holidays, contrary to common belief.

---

## ▶️ How to Run

1. Open [Google Colab](https://colab.research.google.com/)
2. Upload the notebook and dataset (`Walmart_Sales.csv`)
3. Install required packages (if not available):
```python
!pip install -q pandas scikit-learn matplotlib seaborn
```
4. Run the cells in sequence to execute the full pipeline.

---

## 📬 Author & Contact

**Author**: Babulal Jangid  
**Email**: jangidbabulal760@gmail.com  


---

## 📜 License

This project is licensed under the MIT License. You are free to use, share, and adapt with attribution.

---
