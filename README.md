🏏 WPL 2026 Score Estimation using Machine Learning
📌 Project Overview

This project explores how Machine Learning can estimate future outcomes without using future data, using the Women’s Premier League (WPL) as a case study.

The goal is not to predict match winners or exact scores.
Instead, this project estimates expected runs per ball for simulated WPL 2026 match scenarios, using patterns learned from past WPL seasons.

Since no WPL 2026 data exists, the model relies entirely on historical ball-by-ball data and scenario-based forecasting, a standard approach used in real-world ML systems.

🎯 What This Model Predicts (Very Important)

✅ Expected runs per ball
❌ Not match results
❌ Not final scores
❌ Not future data guesses

The output represents average expected scoring behavior under similar match conditions.

🧠 How the Approach Works

Train a regression model on historical WPL ball-by-ball data

Learn scoring patterns based on:

Batting team

Bowling team

Over & innings context

Venue

Player combinations

Create simulated future match scenarios

Use the trained model to estimate:

“If a similar ball is bowled in WPL 2026, how many runs are statistically expected?”

This ensures:

No future data leakage

Honest forecasting assumptions

Realistic ML behavior

📊 Example Output Interpretation

The model produces numeric values such as:

Predicted Value	Interpretation
0.6	Likely dot ball or single
1.2	Single most probable
2.3	Higher scoring opportunity

These are expected values, not exact outcomes — which is how regression-based forecasting works in practice.

🧪 Machine Learning Pipeline

Data Cleaning & Preprocessing

Feature Encoding

Train–Test Split

Baseline Model: Linear Regression

Final Model: Random Forest Regressor

Evaluation Metric: Mean Absolute Error (MAE)

Cross-Validation for robustness

Scenario-based future prediction (2026)

📈 Why Random Forest?

Linear Regression used as a baseline

Random Forest chosen due to:

Better MAE performance

Ability to capture non-linear scoring patterns

R² is intentionally not over-emphasized due to the stochastic nature of ball-by-ball cricket data

🧰 Tech Stack

Python

Pandas

NumPy

Scikit-learn

Matplotlib

Jupyter Notebook

⚠️ Important Notes

This is a learning-driven ML project

Predictions are data-based simulations

Results are not guaranteed real-world outcomes

The project prioritizes clarity, correctness, and honesty

📂 Dataset

Historical WPL ball-by-ball data

Source: <Add Kaggle dataset link here>

🚀 Future Improvements

Include player form and recent performance

Add pitch and weather conditions

Predict over-level or innings-level scores

Quantify uncertainty using prediction intervals

Apply time-aware validation strategies

🙌 Acknowledgements

This project was built as part of a learning-in-public journey to better understand:

Forecasting without future data

Regression-based ML systems

Ethical ML practices in sports analytics

Feedback and suggestions are always welcome.

📬 Contact

If you’d like to discuss this project or provide feedback:

LinkedIn: <www.linkedin.com/in/rishibans-panigrahi-0aa0a2324>
