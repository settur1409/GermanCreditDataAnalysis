<p>Problem Description:<br>
Given German Creditcard applicant data, Problem to appropriately classify the applicants as “Good” and “Bad”.</p>
<p>Methodology:<br>
Followed CRISP-DM framework and below are the components. Also described achievments and approach followed in each component.</p>
<p>Business Objective:<br>
Using German Creditcard data and applying data definition rules, objective is to evaluate/predict the class of applicants based on historical data. Also stated that, risk of labling “Good” customer as “Bad”, is acceptable rather marking “Bad” customers as “Good”.</p>
<p>Data understanding:<br>
Exploratory Data Analysis (EDA), is performed in various levels such as univariate, bi-variate and multivariate to understand the data<br>
and to understand the driving factors that impacts ‘customerclass’. Below is the highlevel snapshot of given data. German credit data is very clean data having no missing values but, based on data definition, the given dataset is to be expanded for further analysis.</p>
<p>Data preparation:<br>
Worked according to data definition to expand given attributes and its respective values. Renamed all the column names appropriately and<br>
column values are expanded appropriately according to data definition. This made data ready for analysis.</p>
<p>WoE Analysis:<br>
Performed analysis on WoE plots, to identify the impact of ‘customerclass’ on each of the attribute in given data. Created Wieght of Evidence (WoE) values for each attribute on given data. Populated WoE values in given data for futher model building.</p>
<p>Information Value Analysis:<br>
Created InformationValue for each of the attribute to measure the level of significancy of individual attributes on ‘customerclass’.<br>
Followed the bench mark convention, to identify the significance of attributes.</p>
<p>Dummy value creation:<br>
Generated a new dataset simiar to given dataset by expanding the given dataset into its respective dummy values. After this conversion, this data is used for further modelling and performing predictions.</p>
<p>Modeling:<br>
Evaluation:<br>
Created two approaches of RandomForest models with two different data perceptions. One model, say RandomForest_ModI, is created with the expanded/replaced values from WoE and observed more than 95% of classification error to predict the “Bad” customers. This approach is ignored and proceeded with building another model using dummy dataframe retrieved from given dataset and named as RandomForest_ModII. During RandomForest_ModII evaluation, found that, error of classification for “Bad” customers is 0 and found a maximum error of 17% while predicting “Good” customers. This satisfies the business problem.</p>
<p>Deployment: NA</p>
