# Applying-Machine-Learning-Enron

In 2000, Enron was one of the largest companies in the United States. 
By 2002, it had collapsed into bankruptcy due to widespread corporate fraud. 
The company hid the financial losses of the trading business and other operations of the company using mark-to-market accounting. 
This technique measures the value of a security based on its current market value instead of its book value.

In the resulting Federal investigation, a significant amount of typically confidential information entered into the public record, including tens of thousands of emails and detailed financial data for top executives.
This data has been combined with a hand-generated list of persons of interest in the fraud case, which means individuals who were indicted, reached a settlement or plea deal with the government, or testified in exchange for prosecution immunity. 
This data has created a dataset of 21 features for 146 employees.

For this project, a correlation matrix was created to get a direct visualization of how each of the 21 features were related to one another. 
The correlation matrix was useful in predicting one attribute from another and impute missing values. Additionally, it was used as a basic quantity for many modelling techniques.

In part with an exploratory analysis, I used the K-Means algorithm to help cluster the POI data; however, since the POI feature was a boolean value, I found that randomly selecting two clusters would not effectively apply to this dataset because this dataset had too many dimensions. For this reason, I moved on from the K-Means project early on in the process. However, for the purpose of this project, it is important to include the entire scope of the analysis. 

In addition to the K-Means Algorithm, I performed a hierarhical analysis on the POI feature. By looking at the hierarchy of the POI, I was able to better visualize the spread between someone who is considered a Person of Interest (POI) and someone who is not. 

Following an analysis of the target feature, POI, I took off with a predictive aalysis algorithm - Logistic Regression. This algorithm is based on the conept of probability. Logistic Regression is beneficial in this case as it provides an unbiased data testing point. For this project, this statistical method is used for predicting binary classes. 


