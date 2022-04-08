# Aviro_health_challenge
## Problem Statement

We must find innovative ways that are easy and safe to get testing and treatment done and prevent new infections, or we will see another generation with millions forced to live with HIV. In this project, we are going to have a machine learning model to determine the likelihood a test been positive or Negative and identifying the factors(features) that makes a test to be positive or negative.

## Solution

**Title**:
**Determine the likelihood of a diagonistics test been positive or negative using machine learning and interpretable machine learning**

**Steps in solving the problem**

1. identify the problem in the dataset
2. Setting appropriate evaluation metrics (ROC_AUC curve)
3. Data Exploration
4. Data Analysis
5. Statistical inference on some features
6. Data Transformation and cleaning
7. Feature Selection
8. Cross validation
9. Building Xgboost Machine Learning model.
10. Interpreting machine learning model using Shap.

### Findings

**Uni-Variate Analysis**
1. Most of the test are Negative with 92.9% and 7.1% positive test
![image](https://user-images.githubusercontent.com/35523815/162517195-dbc11aaf-6561-41aa-89dd-65a43b066418.png)
2. Most patient last tested
![image](https://user-images.githubusercontent.com/35523815/162517412-6bcc9517-cb0d-48ac-a12a-eae2dcc96b08.png)
3. Female Gender visit the clinic the Male
![image](https://user-images.githubusercontent.com/35523815/162517547-433a0dde-1151-45fe-8c3e-1f0f142121e2.png)

**Bi-Variate Analysis**

1. The tested within short time are negative and while more than a 6 month tested are more positive.
![image](https://user-images.githubusercontent.com/35523815/162517910-1ac1f846-9615-4fb6-89e5-7039ef6004d5.png)
2. Most tested postitve speaks **Sesotho** and **Xhosa**
![image](https://user-images.githubusercontent.com/35523815/162517982-e2f4232a-a560-4dea-b474-cb593df7eafa.png)

**Diagonistics (Statistical Inference)**

**art_number_issued, art_initiation, initiation_handover, confirmatory_test_done, last_tested, gender_male, covid_screening_fever, gender_female, oraquick_dentures, covid_screening_pain_headache, appointment** Have significant impact on result response

While

**gender_other, gender_rather_not_say, covid_screening_shortness_of_breath, covid_screening_travel, oraquick_mouthwash, covid_screening_contact, covid_screening_cough, oraquick_bleeding_gums, covid_symptoms** Did not have significant impact on the result response.
![image](https://user-images.githubusercontent.com/35523815/162518371-70e25453-6a50-4875-9a5a-32d7e394fe09.png)

## Result

ROC_AUC Score 90%
![image](https://user-images.githubusercontent.com/35523815/162518461-4b603500-8537-4352-87fe-d4b4b65faa93.png)

Feature Importance 
![image](https://user-images.githubusercontent.com/35523815/162518528-e8fa6b91-93e8-42d7-9f70-288c0d391575.png)

**Interpretable Machine Learning with Shap**

The base value is **Expected Value: -3.2963135**

The top 5 features for determining whether a test response will be positive or negative are:

1. Confirmatory test

2. last_tested

3. engage time difference

4. appointment

5. how ease to use a tool
![image](https://user-images.githubusercontent.com/35523815/162518728-3a2e70b0-746c-4c75-8cb1-3e16a2899273.png)

![image](https://user-images.githubusercontent.com/35523815/162518761-1764cdba-4cd3-49c3-b5e7-6ff5627a8aef.png)


