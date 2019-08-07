# DU_Machine_Learning_Project
Submission for the final project of the DU Data Science Bootcamp.

This is my submission for the DU Bootcamp Final Project. 

Project Goal: To write a model that will analyze real League of Legends game data to predict a winner in future matches.

Data: All data was pulled from http://oracleselixir.com/match-data/ which pulls real game data from the League of Legends 
site and updates weekly. Data had to be cleaned and merged for analysis. 

Data Cleaning: Used Pandas and Matplotlib to clean and analyze the data. The data was structured to fit one of three
predictive regression models: (1) a prematch model which studied champion matchups, (2) a 10 minute model, which 
reviewed stats a 10 mintues, and (3) a 15 minute model which reviewed stats at the 15 minute mark. Please see all 
data cleaning notebooks.

Pre-Match Model: Using a dataset that studied the matchups from each of the games in the dataset, the model makes predictions
based on the real champion matchups. The model predicts at a 57% rate, which is marginally better than the 55% win rate that
the blue side already has going into a match. While the progress is marginal at best, it does show that a more complete
dataset (studying games from high ELO matches) could yield a higher score. Also absent from the model are the player stats,
which happened due to time constraints of the project. The model allows a user to input data.

10/15 Minute Match Model: These models review game stats from 10 and 15 minutes respectively. Real game data was input
into the model and the match is successfully predicted at a rate consistent with the score it received. 

Key Takeaways: League of Legends matches make for a great dataset to learn machine learning concepts. The data is reliable
and consistent. To improve the models, player data should be taken included, as well as datasets from the League API 
in order to get a more compreshensive idea of champion matchup stats. Matchup stats could also include winrates
of team makeup, instead of analyzing purely the matchup. 
