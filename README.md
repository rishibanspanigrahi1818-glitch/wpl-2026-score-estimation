# 🏏 WPL 2026 Score Estimation using Machine Learning

## 📌 Project Overview

This project explores how **Machine Learning can estimate future outcomes without using future data**, using the **Women’s Premier League (WPL)** as a case study.

The goal is **not** to predict match winners or exact scores.  
Instead, the model estimates **expected runs per ball** for **simulated WPL 2026 match scenarios**, using patterns learned from past WPL seasons.

Since **no WPL 2026 data exists**, the model relies entirely on **historical ball-by-ball data** and **scenario-based forecasting**, a standard approach used in real-world ML systems.

---

## 🎯 What This Model Predicts (Very Important)

✅ **Expected runs per ball**  
❌ Not match results  
❌ Not final scores  
❌ Not future data guesses  

The output represents **average expected scoring behavior** under similar match conditions.

---

## 🧠 How the Approach Works

1. Train a regression model on **historical WPL ball-by-ball data**
2. Learn scoring patterns based on:
   - Batting team  
   - Bowling team  
   - Over and innings context  
   - Venue  
   - Player combinations  
3. Create **simulated future match scenarios**
4. Estimate:
   > *“If a similar ball is bowled in WPL 2026, how many runs are statistically expected?”*

---

## 📊 Example Output Interpretation

| Predicted Value | Interpretation |
|----------------|----------------|
| 0.6 | Likely dot ball or single |
| 1.2 | Single most probable |
| 2.3 | Higher scoring opportunity |

These are **expected values**, not exact outcomes —  
which is how regression-based forecasting works in practice.

---

## 🧪 Machine Learning Pipeline

- Data Cleaning and Preprocessing  
- Feature Encoding  
- Train–Test Split  
- Baseline Model: **Linear Regression**  
- Final Model: **Random Forest Regressor**  
- Evaluation Metric: **Mean Absolute Error (MAE)**  
- Cross-Validation for robustness  
- Scenario-based future prediction (2026)

---

## 📈 Why Random Forest?

- Linear Regression used as a **baseline**
- Random Forest chosen due to:
  - Lower MAE performance
  - Ability to capture **non-linear scoring patterns**
- R² is intentionally **not over-emphasized** due to the stochastic nature of ball-by-ball cricket data

---

## 🧰 Tech Stack

- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib  
- Jupyter Notebook  

---

## ⚠️ Important Notes

- This is a **learning-driven ML project**
- Predictions are **data-based simulations**
- Results are **not guaranteed real-world outcomes**
- The project prioritizes **clarity, correctness, and honesty**

---

## 🚀 Future Improvements

- Include player form and recent performance
- Add pitch and weather conditions
- Predict over-level or innings-level scores
- Quantify uncertainty using prediction intervals
- Apply time-aware validation strategies

---

## 📂 Dataset

- Historical WPL ball-by-ball data  
- Source: *([Add Kaggle dataset link here](https://www.kaggle.com/datasets/aravindas01/wpl-india))*

---

## 📬 Contact

- LinkedIn: *(www.linkedin.com/in/rishibans-panigrahi-0aa0a2324)*  
- GitHub: *([Your GitHub profile](https://github.com/rishibanspanigrahi1818-glitch/wpl-2026-score-estimation.git))*  
