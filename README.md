# Disaster Response Pipeline Project

# Project components:
The project consists of three components

1. ETL Pipeline

Loads the messages and categories datasets
Merges the two datasets
Cleans the data
Stores it in a SQLite database

2. ML Pipeline

Loads data from the SQLite database
Splits the dataset into training and test sets
Builds a text processing and machine learning pipeline
Trains and tunes a model using GridSearchCV
Outputs results on the test set
Exports the final model as a pickle file

3. Flask web app

categorize new messages
visualisations of the training set genres, categories and social media categories.

# Instructions:

1. Run the following commands in the project's root directory to set up your database and model.

a)  To run ETL pipeline that cleans data and stores in database python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db

b) To run ML pipeline that trains classifier and saves python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl

2. Run the following command in the app's directory to run your web app. python run.py

3. Go to http://0.0.0.0:3001/

# File structure:
Here's the file structure of the project:

## app

1. template

2. master.html # main page of web app

3. go.html # classification result page of web app

4. run.py # Flask file that runs app

## data

1. disaster_categories.csv # data to process

2. disaster_messages.csv # data to process

3. process_data.py

4. DisasterResponse.db # database to save clean data to

## models

1. train_classifier.py

2. classifier.pkl # saved mode

3. README.md

# Acknowledgements

1. Data has been provided by Figure Eight

2. Tutorials from Pandas and Sklearn were used developing the code:

a) http://pandas.pydata.org/
b) http://pandas.pydata.org/Pandas_Cheat_Sheet.pdf
c) http://scikit-learn.org/stable/modules/model_evaluation.html#classification-report
d) http://scikit-learn.org/stable/modules/classes.html#module-sklearn.ensemble
e) https://www.udacity.com/
