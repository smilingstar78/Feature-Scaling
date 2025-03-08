# Standardization vs. Normalization

## 📌 Introduction
Hello everyone! This guide will help you understand when to use **Standardization** and when to use **Normalization** in Machine Learning. Let's break it down in simple terms.

## 📌 Understanding Feature Scaling
Before diving into the differences, it's important to ask yourself a key question:

### 1️⃣ Is Feature Scaling Required?
To determine whether feature scaling is necessary, consider:
- **The type of data you are using.**
- **The type of algorithm you are implementing.**

Some machine learning algorithms, such as **Decision Trees**, do not require feature scaling, while others, like **Gradient Descent-based models (Logistic Regression, Neural Networks, etc.)**, perform better when feature scaling is applied.

Understanding how your algorithm works internally is crucial in making this decision.

### 2️⃣ Standardization or Normalization?
Once you've determined that feature scaling is needed, the next step is choosing between **Standardization** and **Normalization**.

## 🔹 Standardization
Standardization is generally preferred because it provides better results in most cases. It transforms the data to have **zero mean** and a **unit standard deviation**:

```math
X' = \frac{X - \mu}{\sigma}
```
where:
- \( \mu \) is the mean of the feature
- \( \sigma \) is the standard deviation

### ✅ When to use Standardization?
- When the data does not have a known minimum or maximum value.
- When data is normally distributed (Gaussian distribution).
- When using algorithms like **SVM, K-Means, PCA, Logistic Regression, and Linear Regression**.

## 🔹 Normalization
Normalization (Min-Max Scaling) scales data to a fixed range, usually **[0,1]** or **[-1,1]**:

```math
X' = \frac{X - X_{min}}{X_{max} - X_{min}}
```
where:
- \( X_{min} \) and \( X_{max} \) are the minimum and maximum values in the feature.

### ✅ When to use Normalization?
- When the minimum and maximum values of a feature are known.
- When data is not normally distributed.
- When using algorithms like **Neural Networks and Image Processing (CNNs)** where pixel intensity ranges from **0 to 255**.

## 🎯 Pro Tip:
If you're new to Machine Learning, try **both** techniques on different datasets to develop a deeper understanding of when to use each method.

---

## 🔗 Connect with Me
📌 **LinkedIn:** [Muskan Tariq](https://www.linkedin.com/in/muskan-tariq-095a50282)  
📌 **Instagram:** [@ai_enthusiast86](https://www.instagram.com/ai_enthusiast86?igsh=dnRyenAwdTBxdTZ6)  
📌 **YouTube:** [AI Enthusiast](https://youtube.com/@ai_enthusiast86?si=bYV1AgkBoCMVUBiK)  

🚀 **Happy Coding!**
