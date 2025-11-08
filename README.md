# 🏏 First Innings Score Prediction - IPL

## 🧠 Overview

This project predicts the first innings score of an IPL (Indian Premier League) match based on various match-related and team-specific features. Using machine learning regression techniques, it aims to estimate the target score that can be expected from a team's performance in the first innings.

## 🚀 Features

- Cleaned and preprocessed IPL match data (`ipl.csv`)
- Exploratory Data Analysis (EDA) with Matplotlib and Seaborn
- Feature encoding using OneHotEncoder for categorical variables like team names, venue, and toss winner
- Model training and evaluation using regression algorithms
- Performance comparison between different models based on standard error metrics

## 📊 Dataset

The dataset (`ipl.csv`) contains match-level and innings-level information, such as:

| Feature | Description |
|---------|-------------|
| `batting_team` | Name of the batting team |
| `bowling_team` | Name of the bowling team |
| `venue` | Stadium/venue of the match |
| `runs` | Current runs at a point |
| `wickets` | Current wickets at a point |
| `overs` | Number of overs completed |
| `runs_last_5` | Runs scored in the last 5 overs |
| `wickets_last_5` | Wickets lost in the last 5 overs |
| `total` | (Target variable) Total runs scored in the first innings |

## 🧩 Technologies Used

- Python 3.x
- NumPy, Pandas — Data analysis and preprocessing
- Matplotlib, Seaborn — Data visualization
- Scikit-learn — Model building and evaluation

## ⚙️ Machine Learning Models

The notebook implements and compares multiple regression models:

- 🧮 Linear Regression
- 🌲 Random Forest Regressor
- 📈 Decision Tree Regressor
- 🔥 XGBoost Regressor (optional)

Each model is evaluated using:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- R² Score

## 🧠 Workflow

### 1. Data Loading
- Import the IPL dataset (`ipl.csv`) using Pandas.

### 2. Data Preprocessing
- Handle categorical variables (team names, venue, etc.) using OneHotEncoder.
- Remove irrelevant or redundant columns.
- Split the data into training and test sets.

### 3. Model Training
- Train multiple regression models using Scikit-learn.
- Optimize model parameters to improve prediction accuracy.

### 4. Evaluation
- Compare models using MAE, MSE, and R² Score.
- Visualize predictions vs. actual scores using plots.

## 📈 Results

- Random Forest Regressor often provides the best performance with the lowest MAE and highest R² score.
- Predictions are generally accurate within ±10–15 runs of the actual first innings total.

**Example Result Visualization:**

## Actual vs Predicted First Innings Scores

- Actual: 175 | Predicted: 168
- Actual: 182 | Predicted: 185

  
## 🌟 Visualizations

The project includes:

- Correlation heatmaps
- Distribution plots for numerical features
- Feature importance charts (for tree-based models)
- Actual vs Predicted score comparison plots
