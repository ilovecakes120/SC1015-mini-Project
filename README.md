# SC1015 PREDICTIVE ANALYSIS OF LUNG CANCER RISK FACTORS

School of Computer Science and Engineering
Nanyang Technological University \
Lab: FCE2 \
Group : 6

# Contributors

- Ng Hock Wee Jeremy @JeremyNgHockWee (Machine learning model, slides and video)
- Lee Zheng Wee @ilovecakes120 (cleaning of dataset, data insights , slides and video)
- Lim Yee Herng Reuben @reureuthegreat (cleaning of dataset, data insights, slides and video)
  
# Data Source
- <https://www.kaggle.com/code/sandragracenelson/lung-cancer-prediction>

### Table of Contents:
1. [Hypothetical Variables Chosen](#1-Hypothetical-Variables-Chosen)
2. [Problem Statement](#2-Problem-Statement)
3. [Data Cleaning](#3-Data-Cleaning)
4. [Exploratory Data Analysis](#4-Exploratory-Data-Analysis)
5. [Machine Learning Models](#5-Machine-Learning-Models)
6. [Conclusion](#5-Conclusion)
7. [References](#6-References)

# Hypothetical Variables Chosen

Chosen Variables and insights to choosing them¶ \
Smoking \
is the most well-documented and significant risk factor for lung cancer. It is responsible and a key factor of lung cancer cases. The carcinogens in tobacco smoke damage the cells lining the lungs, and over time, the damage can cause cells to act abnormally and develop into cancer. \

Alcohol Consumption (consuming) \
Excessive alcohol consumption can lead to behaviors and physiological changes that indirectly increase lung cancer risk. For example, heavy drinkers might also be smokers, and alcohol can impair the body's ability to metabolize and clear carcinogens. Hence, we have chosen alcohol due to its potential relation with smoking. \

Fatigue \
in the context of lung cancer could be a symptom reflecting the body’s response to the developing disease. It may also signal other underlying health problems that could be contributing factors, such as sleep apnea or poor oxygenation.\

Chronic Disease \
might play a big key role in prediction due to its common risk factors it has with lung cancer such as smoking. These conditions may exacerbate the risk of developing lung cancer or complicate its management. \

Coughing \
Chronic coughing is a common symptom of lung cancer, often caused by the irritation of air passages or even the presence of a tumor. Studying the patterns and severity of coughing can provide early diagnostic clues. \

# 1)Problem Statement
The project aims to develop a machine learning model to identify the key variables influencing lung cancer prevalence in individuals. By analyzing various demographic, environmental, and behavioral factors, the model seeks to discern patterns and predictors that are significantly associated with the incidence of lung cancer. 

# 2)Data cleaning
- Remove NULL values 
- Remove duplicates 
- Replace numerical value with the corresponding category label (1 and 2 with "No" and "Yes")

# 3)Exploratory Data Analysis

- **Positive Cases Distribution by Age and splitting by gender**
Lung cancer risk increases with age due to prolonged exposure and effects of cellular damage over time. Analyzing how this risk manifests across different age groups can help in identifying key age ranges that are particularly vulnerable.We split the Distributions by Age, split into both genders. Men and women may have different biological susceptibilities to lung cancer. For instance, some studies suggest that women might be more susceptible to the carcinogenic effects of certain types of tobacco and other lung carcinogens than men, even if exposed to lower levels. Gender differences in the presentation of lung cancer symptoms might require different approaches in screening and diagnostics to improve early detection rates.

![image](https://github.com/ilovecakes120/SC1015-mini-Project/assets/165972972/8894aab8-df88-4ae8-9f58-708658a869e0)

Both histograms show an increase in the number of lung cancer cases as age increases, up to a certain point, before the number of cases begins to decrease.

This is consistent with the understanding that lung cancer risk increases with age due to longer exposure to risk factors. It aligns with our expectations


**Merging Genders for Age Distribution**

![image](https://github.com/ilovecakes120/SC1015-mini-Project/assets/165972972/0ff2029c-906f-4de7-bdc6-4051ccdadb8b)

To give a better visualisation, the two distributions are merged to compare based on the ages and increase.

**Analysing Each Data Variable**

![image](https://github.com/ilovecakes120/SC1015-mini-Project/assets/165972972/813e420b-d61a-4375-8f35-6e8a77b9a468)

![image](https://github.com/ilovecakes120/SC1015-mini-Project/assets/165972972/3e3a357a-5a0d-4b23-8cff-083b06a9126d)



When exploring data variables and plotting charts in the context of a study on lung cancer, we aim to understand the relationships, patterns, and distributions that exist within the dataset. By exploring each variable and using appropriate visualizations, we can extract meaningful insights, identify patterns and outliers, and make data-driven decisions will allow us to find out more on which variables serve a deeper purpose toward prediction for lung cancer. Each chart serves to break down complex data into understandable and actionable information.

**HeatMap and Co-relation Matrix for positive lung cancer case**

![image](https://github.com/ilovecakes120/SC1015-mini-Project/assets/165972972/d0365fff-02e5-4403-b571-b97866e3d86b)

The heatmap effectively communicates the strength and direction of relationships between variables, but it’s important to approach the interpretation with caution. While some variables show stronger correlations with lung cancer, correlation alone does not establish causation, and further analysis would be necessary to draw any conclusions about the nature of these relationships. Additionally, the context of the data, including how variables were measured and the population from which the data was collected, is crucial for accurate interpretation.

# 4)Machine learning models
- Support vector machine

the next model we used is the support vector machine model.
in our output we printed out the top 5 variable. the confusionmatrix and the classification report consisitng of the same metrics to evaluate the model.
The accuracy of SVM model is 93% which is similar to the 96% of the logistics regression model'
in the barchat we can see that coughing is the most fluential factor in predicitng lung cancer using SVM follow by alcohol consumption,peer pressure fatigue and allergy.

![image](https://github.com/ilovecakes120/SC1015-mini-Project/assets/165972972/024851d1-a1b3-415e-9a37-6177ed5a77dc)


- Logistic Regression
THe first model we did is logistic regression as the nature of 
the dataset consists of categoerical values.This is the result of the logistic regression model where it has
a accuracy of 96% and the model is evaluated in the classificationreport using metrics such as precision, recall, f1-score, and support
Below we have printed out the top 5 variables use by the model to predict lung cancer
In the barchat here, we can see that alcohol consuming is themost influential factor follow by allergy fatigue anxiety and
swallowing difficulty as the higher the coefficient value the more influence it has

![image](https://github.com/ilovecakes120/SC1015-mini-Project/assets/165972972/62bb795a-f2bd-4375-95a2-ef4ce33fe5cc)

  
# 5)Conclusion
Using what we have learnt from out insights and machine learning models, we can conclude that smoking and alcohol consumption are one of the most influential variables affecting lung cancer. Based on the Machine Learning models, alcohol consumption was shown to be the top variable for logistic regression and second most influential variable in SVM. Secondly, from the insights we can see that more than 50% of smokers had lung cancer in our dataset. Lastly, from both our insights and machine learning models we can see that fatigue and coughing symptoms emerge as top variables in lung cancer cases. Thus, to have early detection of lung cancer, we recommend that individuals facing fatigue/coughing symptoms for a prolonged period to go for a hospital checkup. To reduce the lung cancer, individuals reduce their alcohol consumption whenever possible and stop smoking.

# 6)References
- https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html
- https://scikit-learn.org/stable/modules/svm.html
- https://www.kaggle.com/code/sandragracenelson/lung-cancer-prediction
