This program tries to predict the probability of a player being nominated to the Hall of Fame using a Naive Bayes classifier. This particular exercise disregards if the player is inducted or not and focuses on predicting if the player was nominated. The Python portion is only for visualizing the data, the predictions are calculated using SQL directly.

Setup:
-- MYSQL
1. In MySQL, run the DBCreation.sql file in order to create a new Lahman Baseball database with the name ProjectNB.

2. Run the Procedures.sql file in order to create the required stored procedures for the Database.

-- The required python packages can be found in the requirements.txt file located within this project's folder.

To automatically install these dependencies the following command can be used:
   pip install -r requirements.txt
   

