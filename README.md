# 🎬 IMDb Movie Rating Prediction

### Project Overview
This project aims to predict IMDb movie ratings using machine learning. By analyzing movie metadata, including genres, actors, directors, and budgets, we build regression models to estimate how well a movie will be rated.

### Why This Matters
- Helps streaming platforms and movie studios optimize content investment.
- Enhances recommendation systems by predicting likely high-rated movies.
- Supports film production teams in identifying key success factors.

### About the Dataset
Source: IMDb Dataset (Kaggle)
Features Used:
🎭 Genre, Director, and Cast
💰 Budget, Revenue, Box Office Performance
🕒 Runtime, Release Year, Language
🔢 IMDb Votes, Metascore

### Project Steps
1️⃣ Data Collection & Cleaning: Handled missing values, removed outliers.
2️⃣ Exploratory Data Analysis (EDA): Visualized correlations, feature distributions.
3️⃣ Feature Engineering:
- Extracted director & actor popularity scores.
- Created budget-to-box-office ratio.
- One-hot encoded categorical variables.
4️⃣ Modeling & Evaluation:
- Trained Random Forest, Decision Tree, and Gradient Boosting models.
- Tuned hyperparameters using GridSearchCV.
- Evaluated using R², RMSE, MAE.
5️⃣ Results & Insights: Identified key drivers of high IMDb ratings.

### Key Findings
- Budget, director popularity, and genre significantly impact ratings.
- Ensemble models like Gradient Boosting performed best (R² = X.XX).
- Adding sentiment analysis from reviews could further enhance accuracy.

### Next Steps
- Integrate NLP sentiment analysis from reviews.
- Experiment with deep learning models (e.g., LSTMs).
- Deploy as an interactive web app using Flask/Streamlit.

### About Me
- Name: Ret Taylor
- Email: rettaylor4@gmail.com
- LinkedIn: www.linkedin.com/in/ret-taylor
