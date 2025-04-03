# 📊 Diabetes Dataset - Linear Regression Model

This repository contains an implementation of a **Linear Regression Model** on the **Diabetes Dataset** from `sklearn.datasets`. The goal of this project is to predict diabetes progression based on given medical features.

---

## 📌 Dataset Overview
The **Diabetes dataset** consists of 10 medical features used to predict the diabetes progression measured one year after baseline.

📂 **Dataset Source**: Scikit-learn's built-in Diabetes dataset

---

## 🛠 Implementation Details

🔹 **Model Used:** Linear Regression  
🔹 **Libraries Used:** `numpy`, `pandas`, `matplotlib`, `seaborn`, `sklearn`

---

## 📊 Model Performance
Below are the key evaluation metrics for the trained model:

| Metric | Value |
|--------|------|
| **Mean Squared Error (MSE)** | `2790.81` |
| **Coefficient of Determination (R² Score)** | `0.51` |
| **Intercept** | `152.89112210923963` |

---

## 📈 Scatter Plot of Predictions
To visualize the model's predictions, we created a scatter plot comparing actual values (`y_test`) and predicted values (`y_pred`).

```python
import seaborn as sns
import matplotlib.pyplot as plt

plt.figure(figsize=(8,6))
sns.scatterplot(x=y_test, y=y_pred)
plt.xlabel("Actual Values (y_test)")
plt.ylabel("Predicted Values (y_pred)")
plt.title("📉 Actual vs Predicted Diabetes Progression")
plt.show()
```

---

## 🔍 Key Observations
✅ A strong diagonal trend in the scatter plot would indicate **accurate predictions**.  
⚠️ High dispersion from the diagonal suggests **room for improvement**.  
📌 **Feature Importance (Coefficients):**

| Feature Index | Coefficient Value |
|--------------|------------------|
| **0** | `-34.3289` |
| **1** | `-233.2862` |
| **2** | `487.0310` |
| **3** | `375.6326` |
| **4** | `-446.9244` |
| **5** | `184.5480` |
| **6** | `-51.4008` |
| **7** | `234.6145` |
| **8** | `606.5197` |
| **9** | `44.7123` |

> 📌 The **most influential feature** appears to be **Feature 8**, having the highest coefficient value of `606.5197`.

---

## 🚀 Possible Improvements
To further improve the model, consider:
- 🔄 **Trying Polynomial Regression** to capture non-linearity.
- 📏 **Implementing Feature Scaling** for better performance.
- 🧮 **Exploring Ridge/Lasso Regression** to handle multicollinearity.

---

## 👤 Author
📌 **Rohit Parihar** 
🔗 LinkedIn: [Your Profile](www.linkedin.com/in/rohitpariharr)

---

## 📜 License
This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

---

✨ **Feel free to modify and enhance this project as needed. Happy coding!** 🚀

