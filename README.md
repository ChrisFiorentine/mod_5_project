# mod_5_project
# Introduction
This project is to evalute baseball statistics and to provide analysis. The goal will be to determine important factors that go into winning MLB games, as well as trying to predict future MLB games. 

# The Data
1. MLB game log dataset from data.world.
Contains 171,907 games and 161 columns on those games dating back to 1871. 
2. Baseball dataset from kaggle with 1,232 rows(Teams) and 15 columns.

# Data Preparation
1. Dropped all rows before 2012 to have recent and relevant data.
2. Created Wins and Loss columns for each individual game  as well as Run Differential. 
3. Dropped any columns directly related to runs and wins. Ex. RBI’s, Earned Runs, etc. 
4. Summed each feature by team to have total statistics for every team. 
5. Split home and away games to determine if teams play differently. 

# EDA
1. No team has scored less than 669 runs and still made the playoffs
2. No team has allowed more than 860 runs and still made the playoffs
3. On average, a team that makes the playoffs will win 94 games, have an On Base Percentage of 0.341, a Slugging Percentage of    0.434, and a Batting Average of 0.269 

# Modeling
Used a Dummy Classifier, Logistic regression, a Decision Tree Classifier, Random Forest,  XGBoost, and Gridsearch CV to choose the best model to predict the outcome of a single game.

Used Linear Regression to predict total team wins for a season.

### Model Results 

Dummy Classifier - 0.5 Testing Accuracy
Logistic Regression - 0.96 Testing Accuracy
Decision Tree Classifier - 0.85 Testing Accuracy
Random Forest Classifier - 0.90 Testing Accuracy
XGBoost - 0.95 Testing accuracy 

Linear Regression - 0.80 Testing Accuracy

# Analysis of Features 

1. Hits and Walks were the most important features for scoring runs as well as winning games while the most destructive feature is hitting into double plays, leaving men on base, and being caught stealing. 
2. Some things to note are that home-runs did not have as high an impact which is surprising because the MLB is becoming a home-run driven league.
3. Also, stolen bases do very little to improve a teams chance of winning while being caught stealing is one of the leading factors of losing. 

# Future Steps 
1. Build an effective model that predicts the outcomes of games that haven’t happened yet. 
2. Further investigate how teams can gain an advantage over their opponents. ex . Types of players to scout and in game strategy.  

### Presentaion Link

https://docs.google.com/presentation/d/1D-qn6Vz3ywKHgeEhHijiWPj_06LqLqECHNfHTTJHC-Y/edit#slide=id.gc6f75fceb_0_60

### Sourcing 

https://data.world/dataquest/mlb-game-logs

https://www.kaggle.com/wduckett/moneyball-mlb-stats-19622012?select=baseball.csv





