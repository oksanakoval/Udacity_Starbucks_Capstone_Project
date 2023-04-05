# Starbucks Capstone Project

## Overview

The goal of the project is to build a model in order to predict whether a customer would complete an offer based on the demographic data. The project starts with a thorough data cleaning in order to deal with the specific challenges that occured during data collection. In the second step exploratory data analysis (EDA) is conducted. As a third step, several classification algorithms are used in order to train a model that could predict customer response to the offer based on the demographic data. 


A detailed report of analysis for this project is available [here](https://medium.com/@oksana.p.koval/predicting-customer-response-to-starbucks-offers-ca8dcf99ab7f).

## Datasets and Inputs

For this project, the data sets are provided by Starbucks and Udacity in the form of three JSON files. These contains simulated data that mimics customer behavior on the Starbucks rewards mobile app.
-   portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.)
-   profile.json - demographic data for each customer
-   transcript.json - records for transactions, offers received, offers viewed, and offers completed

Here is the schema and explanation of each variable in the files:

**portfolio.json**

-   id (string) - offer id
-   offer_type (string) - type of offer ie BOGO, discount, informational
-   difficulty (int) - minimum required spend to complete an offer
-   reward (int) - reward given for completing an offer
-   duration (int) - time for offer to be open, in days
-   channels (list of strings)

**profile.json**

-   age (int) - age of the customer
-   became_member_on (int) - date when customer created an app account
-   gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
-   id (str) - customer id
-   income (float) - customer's income

**transcript.json**

-   event (str) - record description (ie transaction, offer received, offer viewed, etc.)
-   person (str) - customer id
-   time (int) - time in hours since start of test. The data begins at time t=0
-   value - (dict of strings) - either an offer id or transaction amount depending on the record

## Files
The following files attached to this GitHub's repository include the following:
-   **Starbucks_Capstone_Project.ipynb**: This is the Jupyter Notebook with the analysis and modeling.

-   **data**: The folder contains the three JSON files provided by Starbucks / Udacity as noted above.

## Acknowledgements
Thanks to Starbucks and Udacity for providing the data utilized in this project!
