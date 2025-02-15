# 🎬 IMDb Movie Rating Prediction

### Project Overview
This project aims to predict IMDb movie ratings using machine learning. By analyzing movie metadata, including genres, actors, directors, and budgets, we build regression models to estimate how well a movie will be rated.

### Why Do IMDb Ratings Matter?
- Helps streaming platforms and movie studios optimize content investment.
- Enhances recommendation systems by predicting likely high-rated movies.
- Supports film production teams in identifying key success factors.

### About the Dataset
Source: IMDb Dataset (Kaggle)  https://www.kaggle.com/datasets/raedaddala/imdb-movies-from-1960-to-2023/data

#### Key Features: 
'Rating': IMDb rating (scale of 1–10). (my target feature)
'Title': Movie title.
'Year': Year of release.
'Duration': Runtime (in minutes).
'MPA': Motion Picture Association rating (e.g., PG, R).
'Votes': Total user votes on IMDb.
'directors': List of directors.
'writers': List of writers.
'stars': Main cast members.
'genres': Movie genres.
'countries_origin': Countries of production.
'filming_locations': Primary filming locations.
'production_companies': Associated production companies.
'Languages': Languages spoken in the movie.
'nominations': Total award nominations.
'oscars': Oscar nominations.

### Project Steps
1) Data Collection & Processing: Handled missing values and removed outliers.
2) Feature Engineering:
- Transformed strings to numerical values to prep for machine learning.
- Extracted the first item from lists for features like directors, stars, and genres.
  - Frequency encoded these items to prep for machine learning. 
- One-hot encoded categorical variables like MPA.
- Binary encoded features like country of origin and filming locations.
3) Exploratory Data Analysis (EDA): Visualized correlations and feature distributions.
4) Feature Scaling & Selection: Scaled columns using Min Max Scaler to prep the data set for machine learning then selected the 15 features with the highest correlation to the target variable using RandomForestRegressor.
5) Modeling & Evaluation:
- Trained Random Forest, Decision Tree, and Gradient Boosting models.
- Tuned hyperparameters using RandomizedSearchCV.
- Evaluated using R², RMSE, MAE.
6) Results & Next Steps: Visualized results from my machine learning models, identified key features with high correlation to IMDb ratings, and identified possible improvements to the model.

### Key Findings
- Oscar nominations, the US as the country of origin, and the movie being rated R are the 3 factors that had the greatest impact on IMDb ratings.
- Gradient Boosting performed best (MSE = 0.574).
- Actor frequency did not have the impact on the model that I had anticipated.

### Next Steps
- Continue with further hyperparameter tuning of the XGBoost model.
- Experiment with deep learning models like LSTMs.
- Conduct further feature engineering - adding features based on ratios between existing features.

### About Me
- Name: Ret Taylor
- Email: rettaylor4@gmail.com
- LinkedIn: www.linkedin.com/in/ret-taylor
