# E-Commerce LTV Prediction Hackathon
This repository contains the solution notebook for the E-Commerce LTV Prediction Hackathon. The goal of this hackathon is to build a model that can predict customers' Long Term Value (LTV) using anonymized and obfuscated real-world data from an e-commerce website.

# Data
The data is stored in two datasets in BigQuery: mh-hackathon.ga4_data.ga4_train and mh-hackathon.ga4_data.ga4_test. The training dataset contains ~4.2 million records, while the testing dataset is used for making predictions.

The column that needs to be predicted is 'ltv', which is available in the training data. The user_pseudo_id is the ID of the users coming to the website. Each user can have multiple pseudo_ids, but for this competition, each ID is assumed to be a separate user. Each user does multiple events based on their event_date and event_timestamp, and the details of those events are stored in event_name and event_params.

# Approach
The primary language used in this hackathon is standard SQL. The approach for building the LTV prediction model includes the following steps:

Data exploration and preprocessing
Feature engineering
Building the model using BigQuery ML
Evaluating the model's performance
Predicting LTV for the test data
Creating a submission file
The solution notebook contains detailed code and explanations for each of these steps.

# Requirements
The following tools and libraries were used in this hackathon:

Google Cloud Platform
BigQuery
Colab
Pandas
Matplotlib
Seaborn
Scikit-learn
Getting started
To get started with this repository, follow these steps:

Clone the repository.
Open the solution notebook in Colab.
Run the notebook to reproduce the results.

# Results
The final predictions on the test data were submitted and scored in the top 1% of the hackathon leaderboard.

# Credits
This hackathon was organized by Google in collaboration with MachineHack. The data was sourced from the BigQuery Ga4 Public Datasets.

