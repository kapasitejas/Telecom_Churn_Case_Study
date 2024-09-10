# Telecom Churn Case Study
>
>

## Table of Contents
* [General Info](#general-information)
* [Approach](#approach)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- Lending Club is the US based consumer finance company which specialises in lending various types of loans
- Consumer attributes and Loan attributes influence the tendency of default
- The case study aims to minimize financial losses for lending companies by identifying loan applicants who are likely to default. These defaulters are referred to as 'charged-off' customers. By using Exploratory Data Analysis (EDA), the study seeks to detect these risky applicants to reduce the incidence of credit loss, which occurs when borrowers fail to repay their loans.
- Loan data set provided to be used for this study. 

# 0. Problem statement

In the telecom industry, customers are able to choose from multiple service providers and actively switch from one operator to another. In this highly competitive market, the telecommunications industry experiences an average of 15-25% annual churn rate. Given the fact that it costs 5-10 times more to acquire a new customer than to retain an existing one, customer retention has now become even more important than customer acquisition.

For many incumbent operators, retaining high profitable customers is the number one business
goal. To reduce customer churn, telecom companies need to predict which customers are at high risk of churn. In this project, you will analyze customer-level data of a leading telecom firm, build predictive models to identify customers at high risk of churn, and identify the main indicators of churn.

In this competition, your goal is *to build a machine learning model that is able to predict churning customers based on the features provided for their usage.*

**Customer behaviour during churn:**

Customers usually do not decide to switch to another competitor instantly, but rather over a
period of time (this is especially applicable to high-value customers). In churn prediction, we
assume that there are three phases of customer lifecycle :

1. <u>The ‘good’ phase:</u> In this phase, the customer is happy with the service and behaves as usual.

2. <u>The ‘action’ phase:</u> The customer experience starts to sore in this phase, for e.g. he/she gets a compelling offer from a competitor, faces unjust charges, becomes unhappy with service quality etc. In this phase, the customer usually shows different behaviour than the ‘good’ months. It is crucial to identify high-churn-risk customers in this phase, since some corrective actions can be taken at this point (such as matching the competitor’s offer/improving the service quality etc.)

3. <u>The ‘churn’ phase:</u> In this phase, the customer is said to have churned. In this case, since you are working over a four-month window, the first two months are the ‘good’ phase, the third month is the ‘action’ phase, while the fourth month (September) is the ‘churn’ phase.

### Objective
- To Predict the customers who are about to churn from a telecom operator
- Business Objective is to predict the High Value Customers only
- We need to predict Churn on the basis of Action Period (Churn period data needs to be deleted after labelling) Churn would be based on Usage

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Approach

### 1. Data Understanding, Preparation and Pre-Processing.
- Data understanding, identification of potentially useful and non-useful attributes and variable importance and impact estimation
- Data preparation, performing data cleaning, missing values imputation, outlier removal, and column level standardization (for e.g., date, etc.) into one format

### 2. Exploratory Data Analysis
- Performing basic preliminary data analysis including finding the correlation between variables and scatter plots to identify relationships between variables
- Performing advanced data analysis, including plotting relevant heatmaps, histograms, and basic clustering to find patterns in the data

### 3. Feature Engineering and Variable Transformation
- Feature engineering and performing one or more methods on attributes that can lead to the creation of a new potentially useful variable; for e.g., day from the date
- Variable transformation and applying categorical variable transformations to turn into numerical data and numerical variable transformations to scale data

### 4. Model Selection, Model Building, and  Prediction
- Identifying the type of problem and making a list of decisive models from all available choices
- Choosing a training mechanism; for e.g., cross-validation, etc., and tuning hyperparameters of each model
- Testing each model on the respective model evaluation metric
- Choosing the best model based on the fit of the data set and output variable
- Using ensemble options to improve the efficacy based on the evaluation metric stated in the problem

## Conclusions

- Out of all the models Randomforest with PCA gives us the best result with known data. But with Unseen data Logistic regression with RFE is giving better accuracy. 

#### Key Indicators and Recommendations :
1. Customers in the telecom sector have access to a variety of service providers and can actively switch from one operator to another. The telecoms business has an average annual churn rate of 15 to 25 percent in this fiercely competitive market.

2. Customer retention is now even more crucial than acquiring new customers because it costs 5–10 times more to do so than to keep an existing customer.

3. We have identified customers who are more likely to churn and the variables that affect high churn in order to manage high value customer churn.

4. From the exploratory analysis, we found that in the Seventh month, which is the action phase, there is a significant decrease in recharge, call usage, and data usage. This is once more clear from the list of critical predictors affecting churn as follows:
    - 'loc_og_t2t_mou_6',
    - 'loc_ic_t2m_mou_6',
    - 'roam_og_mou_6',
    - 'arpu_7',
    - 'loc_ic_t2f_mou_7',
    - 'loc_og_t2t_mou_7',
    - '3g_vbc_6',
    - 'total_amt_7',
    - 'roam_og_mou_7'

5. STD and local The features that have the biggest effects on customer churn are minutes of usage (both incoming and outgoing).

6. Outgoing roaming calls made by clients in the 7th month also play key role in indicating churn.



<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- Python 3.0
- Pandas Library 
- Matplot Library 
- Seaborn Library 
- sklearn Libraries

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
- Huge thanks to Upgrad coaches and respected faculties from IIIT Bangalore, Also the expert lectures taken during the course 
- Credits to Upgrad buddy and live session coaches.
- References - Upgrad Modules


## Contact
Created by [@kapasitejas] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
