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
1. [Problem Statement](#1-Problem-Statement)
2. [Data Cleaning](#2-Data-Cleaning)
3. [Exploratory Data Analysis](#3-Exploratory-Data-Analysis)
4. [Machine Learning Models](#5-Machine-Learning-Models)
5. [Conclusion](#5-Conclusion)
6. [References](#6-References)
   
# 1)Problem Statement
The project aims to develop a machine learning model to identify the key variables influencing lung cancer prevalence in individuals. By analyzing various demographic, environmental, and behavioral factors, the model seeks to discern patterns and predictors that are significantly associated with the incidence of lung cancer. 

# 2)Data cleaning
- Remove NULL values 
- Remove duplicates 
- Replace numerical value with the corresponding category label (1 and 2 with "No" and "Yes")

# 3)Exploratory Data Analysis

- Positive Cases Distribution by Age and splitting by gender
Lung cancer risk increases with age due to prolonged exposure and effects of cellular damage over time. Analyzing how this risk manifests across different age groups can help in identifying key age ranges that are particularly vulnerable.We split the Distributions by Age, split into both genders. Men and women may have different biological susceptibilities to lung cancer. For instance, some studies suggest that women might be more susceptible to the carcinogenic effects of certain types of tobacco and other lung carcinogens than men, even if exposed to lower levels. Gender differences in the presentation of lung cancer symptoms might require different approaches in screening and diagnostics to improve early detection rates.

![image](https://github.com/ilovecakes120/SC1015-mini-Project/assets/165972972/8894aab8-df88-4ae8-9f58-708658a869e0)




# 4)Machine learning models
- Support vector machine
- Logistic Regression 
  
# 5)Conclusion
Using what we have learnt from out insights and machine learning models, we can conclude that smoking and alcohol consumption are one of the most influential variables affecting lung cancer. Based on the Machine Learning models, alcohol consumption was shown to be the top variable for logistic regression and second most influential variable in SVM. Secondly, from the insights we can see that more than 50% of smokers had lung cancer in our dataset. Lastly, from both our insights and machine learning models we can see that fatigue and coughing symptoms emerge as top variables in lung cancer cases. Thus, to have early detection of lung cancer, we recommend that individuals facing fatigue/coughing symptoms for a prolonged period to go for a hospital checkup. To reduce the lung cancer, individuals reduce their alcohol consumption whenever possible and stop smoking.

# 6)References
- https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html
- https://scikit-learn.org/stable/modules/svm.html
- https://www.kaggle.com/code/sandragracenelson/lung-cancer-prediction
