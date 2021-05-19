Project 6 of the Data Scientist Nanodegree Program - Starbucks Capstone Challenge
This project uses demographic, transaction and offer data to find demographic groups which respond best to certain offer types.

Installations
Put the files in the data directory into a folder of your choice
Install following python libraries:
pandas, numpy, matplotlib, nltk, sqlalchemy, pickle,sklearn, plotly
pip install numpy
pip install pandas
pip install matplotlib
pip install nltk
pip install sqlalchemy
pip install pickle
pip install plotly

Project Motivation
In this last project of the Data Scientist Nanodegree Program these data sets were used to determine which demographic groups respond best to which offer types.

File Description
Data about offers and requirements to complete offers
data/portfolio.json

Demographic data
data/profile.json

Information about descriptions of offers and transaction data 
data/transcript.json

Loads and cleans data
Merges both csv-files
Saves data as database file
models/train_classifier.py

Loads data from database file
Trains models and prints out evaluation metrics
app/run.py

Building the web page
Using data to display visuals
Using model to predict categories of new messages
master.html

Web page with visuals
go.html

Web page with classification method
Usage
Opem the command terminal

Set your chosen folder as the workingspace

Run the following commands in terminal:

Loading and cleaning of the data and saving data in a db-file
python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db
Loading the data from the db file and training a model with an evaluation of that model
python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl
Run this model in an application
python app/run.py
Go to http://0.0.0.0:3001/ or https://view6914b2f4-3001.udacity-student-workspaces.com/ and type in the message you want to classify

I tried: "There is a storm!"
Summary
The most common category is 'related' and the least common category is 'child_alone'
The evaluation of the model seem good
The classification could be better
Licensing, Authors, Acknowledgement
This analysis was made by me, an Udacity student with the data provided by Udacity
The results and the code can be used in any way
Please contact me for feedback
Contact:
LinkedIn: https://www.linkedin.com/in/eren-altun91/

Resources:
https://www.kaggle.com/depture/multiclass-and-multi-output-classification
https://towardsdatascience.com/how-to-tune-a-decision-tree-f03721801680
https://scikit-learn.org/stable/modules/multiclass.html
https://www.saltycrane.com/blog/2007/09/how-to-sort-python-dictionary-by-keys/
