Problem Description:
Given German Creditcard applicant data, Problem to apropriately classify the applicants as “Good” and "Bad.
Methodology:
Followed CRISP-DM framework and below are the components. Also described achievments and approach followed in each component.
Business Objective:
Using German Creditcard data and applying data definition rules, objective is to evaluate/predict the class of applicants based on historical data. Also stated that, risk of labling “Good” customer as “Bad”, is acceptable rather marking “Bad” customers as “Good”.
Data understanding:
Exploratory Data Analysis (EDA), is performed in various levels such as univariate, bi-variate and multivariate to understand the data and to understand the driving factors that impacts ‘customerclass’. Below is the highlevel snapshot of given data. German credit data is very clean data having no missing values but, based on data definition, the given dataset is to be expanded for further analysis.
Data preparation:
Worked according to data definition to expand given attributes and its respective values. Renamed all the column names appropriately and column values are expanded appropriately according to data definition. This made data ready for analysis.
WoE Analysis:
Performed analysis on WoE plots, to identify the impact of ‘customerclass’ on each of the attribute in given data. Created Wieght of Evidence (WoE) values for each attribute on given data. Populated WoE values in given data for futher model building.
Information Value Analysis:
Created InformationValue for each of the attribute to measure the level of significancy of individual attributes on ‘customerclass’. Followed the bench mark convention, to identify the significance of attributes.
Dummy value creation:
Generated a new dataset simiar to given dataset by expanding the given dataset into its respective dummy values. After this conversion, this data is used for further modelling and performing predictions.
Modeling:
Evaluation:
Created two approaches of RandomForest models with two different data perceptions. One model, say RandomForest_ModI, is created with the expanded/replaced values from WoE and observed more than 95% of classification error to predict the “Bad” customers. This approach is ignored and proceeded with building another model using dummy dataframe retrieved from given dataset and named as RandomForest_ModII. During RandomForest_ModII evaluation, found that, error of classification for “Bad” customers is 0 and found a maximum error of 17% while predicting “Good” customers. This satisfies the business problem.
Deployment: NA
