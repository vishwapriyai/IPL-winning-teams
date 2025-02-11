# IPL winning teams prediction

![Screenshot of the Application](Screenshot%202025-02-11%20143429.png)

# IPL Win Predictor

## Overview
This project implements a machine learning model to predict the probability of winning for teams in the Indian Premier League (IPL) based on match statistics. The model uses historical match data to provide insights into the likelihood of a team winning given the current match conditions.

## Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Streamlit
- Pickle

## Dataset
The project uses two datasets:
1. `matches.csv`: Contains information about IPL matches, including teams, toss winners, and match results.
2. `deliveries.csv`: Contains detailed information about each delivery in the matches, including runs scored, wickets taken, and other relevant statistics.

## Setup
To set up the environment, install the required libraries:

```bash
pip install pandas numpy scikit-learn streamlit
```

## Usage
### Data Preparation
- Load the datasets:
```bash
import pandas as pd
match = pd.read_csv('matches.csv')
delivery = pd.read_csv('deliveries.csv')
```
- Process the data to create a model-ready dataset, including calculating total runs, current score, runs left, balls left, and wickets.

- Train a machine learning model (e.g., Logistic Regression or Random Forest) using the processed data.

## Running the Streamlit Application
- Ensure that the trained model is saved as pipe.pkl.
- Run the Streamlit application by executing the following command in your terminal:
```bash
streamlit run app.py
```
Open your web browser and go to http://localhost:8501/ to access the application.

## Making Predictions
-Select the batting team and bowling team from the dropdown menus.
- Choose the host city and enter the target score.
- Input the current score, overs completed, and wickets lost.
- Click the "Predict Probability" button to see the winning probabilities for both teams.
  
## Conclusion
This project demonstrates the implementation of a predictive model for IPL matches, allowing users to estimate the chances of winning based on real-time match data.
