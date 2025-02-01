# Insurance-Pricing-Forecast
We can get insurance in many different forms, including motor, property, travel, and 
health. Small amounts of money known as premiums are collected periodically by 
insurance companies from an individual or an organization. These premiums are 
then used to pay the individual or organization for any losses that the insurance 
company covers. It is up to the insurance companies to decide how much premium 
to charge investors.

If insurance companies wind up overcharging their investors, it is natural that those 
investors will prefer to buy insurance from their competitors. In this project we use
regression analysis to determine the best rates for insurance premiums by analyzing 
data on past events, like accidents and natural disasters, we aim to help insurance 
companies set fair prices that balance risk and affordability. 

Data In hand:

The dataset used in this project contains 1338 observations (rows) and 7 features 
(columns). The dataset contains 4 numerical features (age, bmi, children and 
expenses) and 3 nominal features (sex, smoker and region) that were converted into 
factors with numerical value designated for each level.

 age: age of primary beneficiary

 sex: insurance contractor gender, female, male

 bmi: Body mass index, providing an understanding of body, weights that are 
relatively high or low relative to height.

 children: Number of children covered by health insurance / Number of 
dependents.

 smoker: Smoker or not.

 region: the beneficiary's residential area in the US, northeast, southeast, 
southwest, northwest.

 charges: Individual medical costs billed by health insurance.

Analysis:

We began our analysis by exploring the dataset, how many observations are there 
and what are the feature variables, among which, which are the numerical and which 
are the nominal, and we saw sex, smoker and region was nominal so it was 
converted into factors then we checked whether there are any missing values or not,
but there were no missing values. Then we plotted Heatmap to see dependency of
Dependent feature (i.e. medical charges) on Independent features (i.e. other
features) and we see that Smoker, BMI and Age are most important factor that 
determines – Charges. Also we see that Sex, Children and Region do not affect the 
Charges. We might drop these 3 columns as they have less correlation. Now we are 
confirmed that there are no other values in above pre-processed column, We can 
proceed with EDA.

Then we plotted skewness and kurtosis. By doing that we saw that there might be 
few outliers in Charges but then we cannot say that the value is an outlier as there 
might be cases in which Charge for medical was very less actually!
Then we were preparing data - We can scale BMI and Charges Column before 
proceeding with Prediction and we divide the total data into train and test data and 
then applied different regression methods. Here we used Linear Regression, Support 
Vector Machine, Ridge Regressor and Random Forest Regressor and compare
different scores like RMSE, R^2 for train and test data, Cross Validation scores.
According to these scores Random Forest Model is the best fit for the given data. 
Now we again divide the whole data into train and test data and now we didn’t scale 
the data and we used random classifier and used the Random Forest Regressor 
model for train and test data and we saw that the model accuracy is nearly 88% for 
both train and test data. So, we can use this model for further prediction purpose of 
insurance price.

Conclusion:

In conclusion, the project has successfully developed a predictive model to assist 
insurance companies in setting accurate pricing for their policies. By analyzing 
historical data and trends, we have provided valuable insights that enable better risk
assessment and pricing strategies. This will ultimately lead to more fair and 
competitive insurance offerings for customers while ensuring the financial stability of 
insurance providers. Moving forward, ongoing refinement and adaptation of the 
model will be essential to maintain its effectiveness in an ever-evolving insurance 
landscape.
