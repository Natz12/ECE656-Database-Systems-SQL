This program tries to predict the probability of a player being nominated to the Hall of Fame using a Naive Bayes classifier. This particular exercise disregards if the player is inducted or not and focuses on predicting if the player was nominated. The Python portion is only for visualizing the data, the predictions are calculated using SQL directly.

Setup:
-- MYSQL
1. In MySQL, run the lahman-mysql-dump.sql file in order to create a new Lahman Baseball database with the name ProjectNB. (lahman-mysql-dump.sql can be obtained from http://www.seanlahman.com/baseball-archive/statistics/)

2. Run the Procedures.sql file in order to create the required stored procedures for the Database.

-- The required python packages can be found in the requirements.txt file located within this project's folder.

To automatically install these dependencies the following command can be used:
   pip install -r requirements.txt
   

Instructions to use:

Run ECE656_Project.py

1. Press "Enter" to access the program.

2. Enter the database information (host, user, password and database name) so that it can access the baseball database. A copy of it can be accessed in the accompanying .sql file, which when run using the workbench will create a copy of the database calling it ECE656_Project. After entering all the required information, press "Open DB".

3. Select the table to use for the classification, either "Batting", "Pitching" or "Managers".

4. A list of possible features to use for the classification will be displayed in the listbox. Select any number of features that you want to use.

5. Select the percentage that will be used for the train - test split. This percentage of the samples will be used to train the classifier, with the remaining used to test it.

6. Press the "Create Classifier" button and wait for the server to return a result. The textbox after the button will show the classifier performance scores obtained by using the selected features.

7. Using the following listbox, select a player for which you want to predict if they are going to be nominated to the Hall of Fame.

8. Press the "Predict Class" button to predict if the selected player will be nominated to the Hall Of Fame. This will also show the real outcome (Class) of the sample.

   

