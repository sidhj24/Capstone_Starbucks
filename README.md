# Capstone_Starbucks
Capstone project with Starbucks data for promotion

### Objective and Solution:

This project focus on building a ML driven process to help user evaluate Offers run by Starbucks and gauge what are driving factors for opening and usage of the offers. This will also help us predict users likeliness of redeeming the offer
The solution leverage data modeling and feature engineering to be usable by various simple linear vs Tree based models. Eventually using Bagging and Boosting Techniques to get enhanced results

### Overall Description -

This Project is the Capstone project of Data Science Nanodegree Program by Udacity in collaboration with Starbucks. The Datasets contain are -

The data is contained in three files:

* portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.)
* profile.json - demographic data for each customer
* transcript.json - records for transactions, offers received, offers viewed, and offers completed

Here is the schema and explanation of each variable in the files:

**portfolio.json**
* id (string) - offer id
* offer_type (string) - type of offer ie BOGO, discount, informational
* difficulty (int) - minimum required spend to complete an offer
* reward (int) - reward given for completing an offer
* duration (int) - time for offer to be open, in days
* channels (list of strings)

**profile.json**
* age (int) - age of the customer 
* became_member_on (int) - date when customer created an app account
* gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
* id (str) - customer id
* income (float) - customer's income

**transcript.json**
* event (str) - record description (ie transaction, offer received, offer viewed, etc.)
* person (str) - customer id
* time (int) - time in hours since start of test. The data begins at time t=0
* value - (dict of strings) - either an offer id or transaction amount depending on the record

### Dependencies - 

* Python 3.5+
* Machine Learning Libraries: NumPy, SciPy, Seaborn, Pandas, Sciki-Learn, XGBoost
* Files in json format

### Execution - 

1. Run the Starbucks_Capstone_notebook_Final.ipynb file present in the master repository

### Acknowledgements -

1. Udacity for providing an amazing Data Science Nanodegree Program
2. Starbucks for providing the relevant dataset to train the model

### Other Details - 

1. ETL Pipeline -
	a. ETL pipeline process use basic concepts for Extracting, Transform and Loading. These concepts are used to load the data, clean it in required manner and save it in processed dataframe
	b. The files post ETL Transformation will be used for ML model build

2. ML Pipeline
	a. Build multiple models and picking best classifier model giving best results
	b. Evaluate and Summarize the outcomes of the model
	c. GridSearch to refine the model output
	
### Important Files
  a. data/ - Folder will have all 3 raw data files used for the analysis and model building
  b. pic1 + pic2 - visuals used to help us leverage the workspace for training
  c. Starbucks_Capstone_notebook_Final.ipynb file with all the relevant coding elements

