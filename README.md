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

The Naive Bayes classifier was thought of as a logical approach to use as there is a strong independent assumption when having a dataset that has multiple features. This classifier is highly scalable, and since the Enron dataset has multiple parameters it has proved to be most appropriate for this project. 

As a result of using Naive Bayes, the following conclusions have been found as to who was predicted to be a POI and who was actually a POI. 

1.) Jeffrey Skilling, CEO, served a 12 year sentence as a POI. The Naive Bayes model correctly predicted that he would be a POI. 
2.) Kevin Hannon, COO, served a two-year prison sentence. The same model correctly predicted he would be a POI. 
3.) Interestingly enough, Scott Yeager, an employee, was convicted in the original dataset while this predictive model predicted him as not being a POI. He was acquitted of all charges after a long legal battle that went to the Supreme Court. 
4.) Chris Calgar, another employee, was listed as a POI on the dataset, while this model predicted he was not a POI. Sure enough, his charges were dismissed. 
5.) John Baxter, who was found dead in his car before he was to testify before Congress, was listed as a non-POI, while the model predicted it to be true. 
6.) James Derrick was on the general counsel of Entron. While he testified before congress, the model predicted that he would be found as a POI as well. 

Given the sample information above, the Naive Bayes model demonstrated to be most effective in revealing what this dataset had to offer. Overall, it was also found that a majority of the POI's have no deferred payments. Additionally, deferred salary payments made employees unsecured creditors of the company, exposing them to losing most of all of their money in their accounts. Additionally, most POI's had a higher bonus-to-salary ratio. Finally, some POI's were sending a lot of emails leading up to bankruptcy... by no coincidence, the CEO was receiving majority of those. 
