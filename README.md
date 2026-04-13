# IPL-Score-Predictor
🏏 IPL Score Prediction | Machine Learning project using Linear Regression to predict T20 cricket final scores from powerplay and first 10 overs data | Python · Pandas · NumPy · Scikit-learn · Matplotlib

This project leverages the IPL Complete Dataset (2008–2024) to predict the final score of a team in the first innings based on match performance in the first 10 overs.

Using ball-by-ball data, the model learns scoring patterns and provides accurate predictions of final totals.

🎯 Objective

To build a Machine Learning model that:

Predicts final innings score using early match data
Analyzes how initial performance impacts total score
Provides actionable insights into scoring trends

📊 Dataset
Dataset Name: IPL Complete Dataset (2008–2024)
Source: Ball-by-ball IPL data
Files Used:
deliveries.csv (ball-level data)

🔹 Key Columns Used
match_id
inning
over
total_runs
player_dismissed

⚙️ Tech Stack
Language: Python
Environment: Google Colab
Libraries:
Pandas
NumPy
Matplotlib
Scikit-learn
🧠 Machine Learning Approach
🔹 Model Used
Linear Regression
🔹 Feature Engineering

Features created from first 10 overs:
runs_so_far → Total runs scored
wickets_lost → Total wickets fallen
run_rate → Runs per over
wickets_remaining → Remaining wickets

🔄 Workflow
Load and preprocess dataset
Filter first 10 overs data
Aggregate match-level features
Merge with final innings score
Train-test split
Train Linear Regression model
Evaluate performance
Visualize results

📈 Model Evaluation
MAE (Mean Absolute Error) → Measures prediction error
R² Score → Measures model performance

📊 Visualizations
🔹 Actual vs Predicted Plot
Shows how close predictions are to actual scores
Ideal predictions lie along the diagonal line
🔹 Residual Plot
Shows prediction errors
Helps analyze model reliability
🔮 Sample Predictions
Score after 10 overs	Predicted Final Score
87/2	~170–185
54/4	~130–150
102/1	~190–210

💻 How to Run
Open the notebook in Google Colab
Upload deliveries.csv
Run all cells sequentially

🛠️ Prediction Function
predict_score(runs, wickets)

Example:
predict_score(87, 2)

📌 Key Insights
Teams scoring 80+ runs in first 10 overs tend to reach high totals
Early wickets significantly reduce scoring potential
Run rate is a strong indicator of final score
Consistency matters more than occasional big hits

📁 Output Files
ipl_prediction.png → Actual vs Predicted visualization
residual_plot.png → Residual analysis
