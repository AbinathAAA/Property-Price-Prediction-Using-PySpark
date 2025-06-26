# 🏡 Property Price Prediction Using PySpark

## 📌 Project Overview

This project explores the use of **Linear Regression models** in **PySpark** to predict property prices based on key features commonly associated with real estate valuation. The goal was to test how well different combinations of features impact the model's prediction accuracy, and to evaluate the results using metrics like **R²**, **Mean Squared Error (MSE)**, and **Root Mean Squared Error (RMSE)**.

---

## 🔍 Feature Selection

Five features were selected from the dataset based on domain knowledge and expected influence on property prices:

- `Square_Footage`
- `Num_Bedrooms`
- `Num_Bathrooms`
- `Year_Built`
- `Lot_Size`

These features were tested in different combinations to understand their individual and collective impact on the model’s performance.

---

## ⚙️ Model Comparison

I developed three different regression models:

1. **Basic Model** – using only two features  
2. **Intermediate Model** – using four features  
3. **Full Model** – using all five selected features

The full model outperformed the others by achieving the **highest R² score**, demonstrating that including more relevant features typically improves prediction performance. However, it also emphasized the importance of avoiding irrelevant or redundant features, which can introduce noise or lead to overfitting.

---

## 🧱 Challenges and Solutions

### 🔸 Handling Missing Data
Some records contained null or missing values that interfered with model training. To resolve this, I cleaned the dataset using PySpark’s `.dropna()` method to remove incomplete rows.

### 🔸 Understanding PySpark ML Pipeline
Initially, it was challenging to grasp the structure of PySpark's ML pipeline. Over time, I became comfortable with key stages like:

- Feature assembly using `VectorAssembler`
- Data scaling
- Applying the regression algorithm

This understanding helped streamline the experimentation process.

---

## 📚 Key Learnings

- **Thoughtful Feature Selection** is critical — even a small change in the features used can significantly affect model accuracy.
- **PySpark Pipelines** are powerful for managing large-scale machine learning workflows in a reusable and modular way.
- **Evaluation Metrics** like R², MSE, and RMSE are essential for assessing and comparing model performance fairly.

---

## ✅ Conclusion

This project was a valuable hands-on experience in predictive modeling and big data processing using PySpark. It helped me strengthen my understanding of machine learning pipelines, improve my data preprocessing skills, and build confidence in deploying regression models for real-world problems.

---

> 🚀 Ready to contribute? Fork the repo, create a new branch, and let’s build smarter property pricing models together!

