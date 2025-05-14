# stock_prediction
# 📈 Stock Price Direction Prediction using Random Forest (AAPL)

This project is a part of my journey to understand financial modeling, machine learning, and how AI can be applied in stock market predictions. As someone exploring quant roles without a formal background in financial engineering, I used online resources, AI tools, and documentation to build this model from scratch.

---

## 🧠 Problem Statement

The goal of this project is to predict whether the **next day's closing price of Apple Inc. (AAPL)** stock will go **up or down**, based on historical price trends and technical indicators. This is a classic **binary classification** problem where:

- `1` indicates the price went up
- `0` indicates the price went down

---

## 📊 Features Used

- **Lag_1:** Yesterday’s price
- **MA_3, MA_7:** 3-day and 7-day moving averages
- **RSI:** Relative Strength Index (14-day)
- **Volatility:** 30-day rolling standard deviation
- **Log_Return:** Log of daily return

---

## 🧪 Model & Results

Model used: **Random Forest Classifier**

**Performance on Test Set:**

- **Accuracy:** ~57.16%
- **Precision (Up):** 56%
- **Recall (Up):** 60%
- **F1 Score (Up):** 58%

### 🔹 Confusion Matrix

|                | Predicted Down | Predicted Up |
|----------------|----------------|--------------|
| **Actual Down** | 199 (TN)        | 168 (FP)      |
| **Actual Up**   | 143 (FN)        | 216 (TP)      |

The model shows a balanced performance and lays the foundation for future improvement using more advanced techniques.

---

## 📌 Key Learnings

- Built a full ML pipeline using `sklearn`, `pandas`, `yfinance`
- Learned about feature engineering with technical indicators
- Understood model evaluation using confusion matrix & classification report
- Practiced interpreting model performance on noisy financial data

---

## 🛠️ Next Steps

- Try time-series aware models (XGBoost, LSTM)
- Incorporate macroeconomic data
- Tune hyperparameters and use cross-validation

---

## 🤖 Note

This is a **learning project** and not financial advice. It's part of my self-guided effort to break into the quant and data science space, and I’m continuously improving my understanding of both finance and machine learning.

