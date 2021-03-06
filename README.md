# Cardio Catch Diseases Company

# 1.0 Context

<h3> What are cardiovascular diseases? </h3>

Cardiovascular diseases are a group of diseases of the heart and blood vessels and include:

- Coronary disease - disease of the blood vessels that irrigate the heart muscle.

- Cerebrovascular disease - disease of the blood vessels that irrigate the brain.

- Peripheral arterial disease - disease of the blood vessels that irrigate the upper and lower limbs.

- Rheumatic heart disease - damage to heart muscle and heart valves due to rheumatic fever caused by streptococcal bacteria.

- Congenital heart disease - malformations in the structure of the heart existing since the moment of birth.

- Deep vein thrombosis and pulmonary embolism - blood clots in the leg veins that can dislodge and move to the heart and lungs.

Heart attacks and strokes are usually acute events caused mainly by a blockage that prevents blood from flowing to the heart or brain. The most common reason for this is the accumulation of fat deposits in the internal walls of blood vessels that irrigate the heart or brain. Strokes can also be caused by bleeding in the blood vessels of the brain or by blood clots.

<h3> What are the risk factors for cardiovascular diseases? </h3>

The risk factors for cardiovascular diseases are **inadequate diets, sedentariness, smoking and harmful use of alcohol**. These factors can manifest themselves in people through **hypertension, high glucose, hyperlipidemia, overweight and obesity.**


<h3> What are the main symptoms of cardiovascular diseases? </h3>
    
Often there are no symptoms of the underlying disease of the blood vessels. A heart attack or stroke may be the first warning.
The symptoms of heart attack include pain or discomfort in the center of the chest and pain or discomfort in the arms, left shoulder, elbows, jaw or back.

In addition, the person may have difficulty breathing or shortness of breath; feeling sick or vomiting; feeling faint or dizzy; cold sweat; and pallor. Women are more likely to experience shortness of breath, nausea, vomiting, and back or jaw pain.

The most common symptom of a stroke is a sudden weakness of the face and the upper and lower limbs, more frequent on one side of the body. Among the symptoms are:

- Numbness in the face, arms or legs, especially on one side of the body.

- Confusion, difficulty to speak or to understand.

- Difficulty to see with one or both eyes.

- Difficulty to walk, dizziness, loss of balance or coordination.

- Intense headache with no apparent cause.

- Fainting or unconsciousness.


<h3> Why are cardiovascular diseases a development problem in low and middle income countries? </h3>

Unlike of the people that live in high-become coutries, people of low and middle-income countries often do not have the benefit of integrated primary  care programs for the early detection and treatment of individuals exposed to risk factors. Thus, people that suffer from cardiovascular disease and other non-communicable diseases in low and middle-income coutries have less acess to effective and equitable health services that respond to their needs. As a result, many people of  low- and middle-income countries are diagnosed late and die prematurely at their most productive age due to cardiovascular disease and other non-communicable diseases.

The poorest people in low and middle income countries are the most affected. At the family level, evidence is emerging to prove that cardiovascular and other non-communicable diseases contribute to poverty due to catastrophic health expenditures and higher than planned expenditures. At the macroeconomic level, cardiovascular diseases create a heavy burden on the economies of low and middle income countries.


<h3> How can the number of cardiovascular diseases be reduced? </h3>

The number of cardiovascular diseases can be reduced by adopting measures such as:

- Comprehensive policies for tobacco control.

- Taxes to reduce the intake of food rich in fats, sugars and salt.

- Construction of paths for walking and cycling, with the aim of increasing the practice of physical activities.

- Strategies to reduce the harmful use of alcohol.

- Providing healthy meals for children in the school environment.


<h3> How can artificial intelligence help fight cardiovascular disease? </h3>

As many underdeveloped countries cannot cope with the health of the population due to its high cost, artificial intelligence can guide the allocation of scarce resources in the health area and facilitate the efficient and accurate identification of decisions that favor the individualization of care based on the flow of information that emerges from an integrated and complex ecosystem: it is precision medicine. Therefore, it can be inferred that the practice of cardiovascular sciences will have significant impacts, which will translate into a personalized approach and better results.


# 2.0 Business Problem

Cardio Catch Diseases is a company specialized in detecting heart disease in the early stages. Its business model lies in offering an early diagnosis of cardiovascular disease for a certain price.

Currently, the diagnosis of cardiovascular disease is manually made by a team of specialists. The current accuracy of the diagnosis varies **between 55% and 65%**, due to the complexity of the diagnosis and also the fatigue of the team who take turns to minimize the risks. The cost of each diagnosis, including the devices and the payroll of the analysts, is around $1,000.00.

The price of the diagnosis, paid by the client, varies according to the precision achieved by the team of specialists.

| Exam Accuracy | Price  | Rules                                  | Example          |
|:---------------|:---------------------|:---------------------------------------|:----------------|
| Above 50%     | min \$500\.00          | \+\$500 for each additional 5% accuracy | Accuracy = 55% \-> \$1.000\.00 |
| Up to 50%     | $0\.00                | N/A                                    | N/A               |

Thus, we see that **different values in the exam precision**, given by the team of specialists, make the company either have a profitable operation, revenue greater than the cost, or an operation with a loss, revenue less than the cost. This instability of the diagnosis makes the company to have an **unpredictable cashflow**.

The company has the objective of **creating a tool that increases diagnostic accuracy and that this accuracy is stable for all diagnoses**. Therefore, the function of this project is to create a patient classification tool with stable accuracy.Together with this tool, the CEO of Cardio Catch Diseases requested a report, reporting the results to answer the following questions:

- **What is the accuracy and precision of the tool?**


- **What will be the company's revenue with the new tool?**


- **How reliable is the data result of the new tool?**

<h2> Presenting Data </h2>

This work will be using the data set is available in this [link](https://www.kaggle.com/sulianova/cardiovascular-disease-dataset).

<h2> Objectives </h2>

- Create a tool that increases the accuracy of disease diagnosis.


- The accuracy of this tool should be stable for all diagnostics.


- Create a report with the results generated by the tool.


- Answer the questions.

# 3.0 The Solution 

In this project, we developed a model that classifies people with cardiovascular diseases or not. This solution can be implemented in the company Cardio Catch Diseases to help solve your business problem. The model has an precision between 74.93% and 78.11%.

## 3.1 Main Steps

### 3.1.1 Data Describe - Statistics Descriptive

#### Numerical Variables

![01](https://github.com/nickolasdias/Cardio-Catch-Diseases/blob/master/image/01.png)

**Important Observations:**

- People are between 30 and 65 years old, with an average of 53 years and a median of 54 years. By the proximity of the position measurements, this variable approaches a **normal distribution**.

- People are between 55 cm and 250 cm high, with an average of 164 cm. However, the minimum height is suspect, as there are no records of children. 

- People weigh between 10 kg and 200 kg, with an average of 74 kg. However, the minimum weight is suspect, since there are no records of children.

- The measurement of -150 and 11.000 **diastolic pressure** is suspect, since it is out of reality.

- The measure of -70 and 16.070 of **systolic pressure** is suspect, since it is out of reality.


#### Categorical Variables

![02](https://github.com/nickolasdias/Cardio-Catch-Diseases/blob/master/image/02.png)

**Observations:**

- The age range of people with cardiovascular disease is 38 to 65 years, with a median over 55 years. And the age range of people without cardiovascular disease is 30 to 65 years old, with a median under 55 years old.

- The height range of people with cardiovascular disease is practically the same as the height range of people without cardiovascular disease. There are also significant outliers that are below the minimum height of both. 

- The weight range of people with cardiovascular disease is greater than the weight range of people without cardiovascular disease, no matter the difference is minimal with the presence of outliers.

- The age range of people with normal, above normal and well above normal cholesterol are similar. However, the age range of 52 to 60 years old is more concentrated for people with cholesterol well above normal. The concentration of people with normal cholesterol is between 48 and 58 years. And the concentration of people with above-normal cholesterol is between 50 and 57 years old. 

- The concentration of height ranges for people with any level of cholesterol is practically the same. However, there are many outliers in the height range of people who have normal cholesterol. These heights include being below 150 cm.

- The concentration of people with cholesterol well above normal in relation to weight is greater than the concentration of people with higher than normal cholesterol and people with normal cholesterol.

- The age range people with normal glucose, above normal and well above normal are similar. However, the age range from 50 to 60 years old, people with glucose above normal are more concentrated. The concentration of people with glucose well above the normal is between 52 and 60 years. And the concentration of people with normal glucose is between 48 and 58 years.

- The concentration of the height ranges of people with any glucose level is practically the same. However, there are many outliers in the height range of people who have normal glucose. These heights include being below 150 cm.

- The concentration of people with glucose above normal in relation to weight is greater than the concentration of people with glucose well above normal and people with normal cholesterol.

### 3.1.2 Mental Hypothesis Map

![hip](https://github.com/nickolasdias/Cardio-Catch-Diseases/blob/master/image/Cardiovascular_Diaseases.png)


### 3.1.3 Exploratory Data Analysis

**Univariate Analysis - Target**

![03](https://github.com/nickolasdias/Cardio-Catch-Diseases/blob/master/image/03.png)

**Observation:**

- Number of people with CVDs: 50.65 %

- Number of people without CVDs: 49.35 %



**Univariate Analysis - Numerical**

![04](https://github.com/nickolasdias/Cardio-Catch-Diseases/blob/master/image/04.png)

**Observations:**
- The ages are between 38 and 65 years.
- The highest height concentration is between 1.60 m and 1.70 m.
- The weight is concentrated between 60 kg and 80 kg.
- Presents a blood pressure of 120 for diastolic and 80 for sistolic which means elevated to high blood pressure.
- The highest body mass index is concentrated between 20 and 30.


**Univariate Analysis - Categorical**

![05](https://github.com/nickolasdias/Cardio-Catch-Diseases/blob/master/image/05.png)

**Observations:**
- There many more people presenting of the **female gender**.
- There many more people presenting **normal levels** for both `cholesterol` and `glucose`.
- The great majority of people **don't smoke neither intakes alcohol**.
- The majority of people **are physically active**.


**Bivariate Analysis - Validation of the Hypothesis**

**H1. There are more cases of cardiovascular diseases among older people. (FALSE)**

![06](https://github.com/nickolasdias/Cardio-Catch-Diseases/blob/master/image/06.png)

Looking at the graph above, there are more cases of cardiovascular diseases among adults than older people. 
> Therefore, a hyphotese is **FALSE**.

**H2. There is no relationship between the appearance of cardiovascular diseases and people's hight. (TRUE)**

![07](https://github.com/nickolasdias/Cardio-Catch-Diseases/blob/master/image/07.png)

Looking at the graph above, there is no relationship between the appearance of cardiovascular diseases and people's height.
> Therefore, the hypothesis is **TRUE**.

**H3. There are more cases of cardiovascular diseases among obesity people. (TRUE)**

![08](https://github.com/nickolasdias/Cardio-Catch-Diseases/blob/master/image/08.png)

Looking at the graph above, there are more cases of cardiovascular diseases among people with obesity than people without obesity.
> Therefore, the hyphotese is **TRUE**.

**H4. There are more cases of cardiovascular diseases among people of the female gender. (TRUE)**

![09](https://github.com/nickolasdias/Cardio-Catch-Diseases/blob/master/image/09.png)

Looking at the graph above, there are more cases of cardiovascular diseases among female people than male people.
> Therefore, a hyphotese is **TRUE**.

**H5. There are more cases of cardiovascular diseases among people who do not do physical activity. (FALSE)**

![10](https://github.com/nickolasdias/Cardio-Catch-Diseases/blob/master/image/10.png)

Looking at the graph above, there are more cases of cardiovascular diseases among people who practice physical activity than people who do not practice physical activity.
> Thus, the hyphotese is **FALSE**.

**H6. There are more cases of cardiovascular diseases among people who intake alcohol. (FALSE)**

![11](https://github.com/nickolasdias/Cardio-Catch-Diseases/blob/master/image/11.png)

Looking at the graph above, there are more cases of cardiovascular diseases among people who do not use alcohol than people who use alcohol. 
> Thus, the hyphotese is **FALSE**.

**H7. There are more cases of cardiovascular diseases for people presenting high cholesterol. (FALSE)**

![12](https://github.com/nickolasdias/Cardio-Catch-Diseases/blob/master/image/12.png)

Looking at the picture, there are more cases of cardiovascular disease for people who have normal cholesterol than high cholesterol. 
> Therefore, the hyphotese is **FALSE**.

**H8. There are more cases of cardiovascular diseases among people who smoking. (FALSE)**

![13](https://github.com/nickolasdias/Cardio-Catch-Diseases/blob/master/image/13.png)

Looking at the graph above, there are more cases of cardiovascular diseases in people who do not smoke. 
> Therefore, the hyphotese is **FALSE**.

**H9. There are more cases of cardiovascular diseases for people presentig high glucose. (FALSE)**

![14](https://github.com/nickolasdias/Cardio-Catch-Diseases/blob/master/image/14.png)

Looking at the graph above, there are more cases of cardiovascular diseases in people that have 
 normal glucose. 
 > Therefore, the hyphosis is **FALSE**.

**H10. There are more cases of people with elevated blood pressure. (FALSE)**

![15](https://github.com/nickolasdias/Cardio-Catch-Diseases/blob/master/image/15.png)

Looking at the graph above, there are more cases of people with normal than high pressure. 
> Therefore, the hyphotese is **FALSE**.

**Bivariate Analysis - Summary Hyphoteses**

![16](https://github.com/nickolasdias/Cardio-Catch-Diseases/blob/master/image/16.png)

**Multivariate Analysis - Numerical Variables**

![17](https://github.com/nickolasdias/Cardio-Catch-Diseases/blob/master/image/17.png)

**Relevants Observations:**
- `ap_hi` and `ap_lo` present **high positive correlation (0.72)**.
- `height` and `weight` present **weak positive correlation (0.30)**.
- `bmi` and `weight` present **high positive correlation (0.86)**.

**Multivariate Analysis - Categorical Variables**

![18](https://github.com/nickolasdias/Cardio-Catch-Diseases/blob/master/image/18.png)

**Relevants Observations:**

- `smoke` and `gender` present **weak positive correlation (0.34)**.
- `cholesterol` and `gluc` present **weak positive correlation (0.39)**.
- `alco` and `smoke` present **weak positive correlation (0.34)**

**Multivariate Analysis - Numerical Variables and Binary Variables**

![19](https://github.com/nickolasdias/Cardio-Catch-Diseases/blob/master/image/19.png)

**Relevants Observations**:

- `height` and `smoke`: **weak positive correlation**.
-  All the others correlations are nulls.

### 3.1.4 Machine Learning

Tests were made using different algorithms.

#### Performance Metrics

![20](https://github.com/nickolasdias/Cardio-Catch-Diseases/blob/master/image/20.png)

As observed, for the context of our project, we have:

- On the **business** side, aiming for precision, as each 5% more on precision translates to \$500 more from each diagnostic made.

- On the **patient** side, aiming for recall, as we are trying to minimize the false negative rate.

In addition, we are trying to achieve a balance between accuracy and recall. We can make use of f1-score as a metric that can provide us with this balance. Thus, we have two algorithms that satisfy this need. They are them: **Catboost Classifier and LGBM Classifier**.

For having a little better performance, we will use the **LGBM Classifier** algorithm.


#### Confusion Matrix

![21](https://github.com/nickolasdias/Cardio-Catch-Diseases/blob/master/image/21.png)

We can observe through the confusion matrices that models such as **Catboost** and **SGD Classifier** have behaviors that cannot be ruled out, however, as the **LGBM Classifier** presents a better accuracy, we will choose this model as the work solution.

#### ROC Curves

![22](https://github.com/nickolasdias/Cardio-Catch-Diseases/blob/master/image/22.png)

Analyzing the ROC curves above, the **LGBM** and **Catboost** models are close, but with different confusion matrices. Therefore, as mentioned before, we will choose the **LGBM** model to work.

#### Cross-Validation Scoring - LGBM Classifier

- Average precision: 0.7637 (+/- 0.0137)
- Average recall: 0.6963 (+/- 0.0258)
- Average f1-score: 0.7284 (+/- 0.0162)
- Average ROC AUC: 0.8079 (+/- 0.0148)


### 3.1.5 Hyperparameter Fine Tuning

In machine learning, hyperparameter optimization or tuning is the problem of choosing a set of optimal hyperparameters for a learning algorithm. A hyperparameter is a parameter whose value is used to control the learning process. By contrast, the values of other parameters (typically node weights) are learned.

Therefore, we will use the RandomSearchCV algorithm beacuse, the method described herein is a type of local random search, where every iteration is dependent on the prior iteration's candidate solution. So, we will spend less time to obtain the result.

In our best algorithm, we apply the technique to find the best parameters. Below, we can see its performance with the chosen parameters. 

![29](https://github.com/nickolasdias/Cardio-Catch-Diseases/blob/master/image/29.png)

#### Roc Curve

![23](https://github.com/nickolasdias/Cardio-Catch-Diseases/blob/master/image/23.png)

#### Confusion Matrix

![24](https://github.com/nickolasdias/Cardio-Catch-Diseases/blob/master/image/24.png)

#### Cross Validation Score

- Average precision: 0.7630 (+/- 0.0166)
- Average recall: 0.6986 (+/- 0.0239)
- Average f1-score: 0.7293 (+/- 0.0167)
- Average ROC AUC: 0.8073 (+/- 0.0145)

### 3.1.6 Evalution of the Best Model

To evaluate of the best model, we will calibrate the curves and metrics of the model. And finally, we will do the cross validation.

#### Calibrating Curves

![25](https://github.com/nickolasdias/Cardio-Catch-Diseases/blob/master/image/25.png)

We can see that the calibrated model fits better to the tuned model.

#### Calibrating Model Metrics

![30](https://github.com/nickolasdias/Cardio-Catch-Diseases/blob/master/image/30.png)

By calibrating the metrics of the model, we can see that there is no increase in its performance.

#### Calibrating Model - ROC Curve and Confusion Matrix

![26](https://github.com/nickolasdias/Cardio-Catch-Diseases/blob/master/image/26.png)

![27](https://github.com/nickolasdias/Cardio-Catch-Diseases/blob/master/image/27.png)

#### Calibrating Model - Cross Validation Score

- Average precision: 0.7652 (+/- 0.0159)
- Average recall: 0.6948 (+/- 0.0255)
- Average f1-score: 0.7282 (+/- 0.0181)
- Average ROC AUC: 0.8079 (+/- 0.0145)

### 3.1.7 Anwering the Questions

#### What is the accuracy and precision of the tool ?


| Model | Average Precision  | Average Recall | Average F1-Score | Average ROC AUC |
|:---------------|:---------------------|:---------------------------------------|:----------------|:---------------|
| LGBM Classifier | 0.7637 (+/- 0.0137) | 0.6963 (+/- 0.0258) | 0.7284 (+/- 0.0162) | 0.8079 (+/- 0.0148) |
| LGBM Classifier Best Model | 0.7630 (+/- 0.0166)  | 0.6986 (+/- 0.0239) | 0.7293 (+/- 0.0167) | 0.8073 (+/- 0.0145) |
| LGBM Classifier Calibration | 0.7652 (+/- 0.0159)| 0.6948 (+/- 0.0255) | 0.7282 (+/- 0.0181) | 0.8079 (+/- 0.0145) |

Analyzing the summary of the model, we can verify that **LGBM Classifier Calibration** model has a better **precision** than the other models, although the **f1-score** and **recall** have a score lower. In addition, for being calibrated, the model will be more stable and confident. This is good for both business and patients.

> Therefore, the **precision** is of 76.52%.

#### What will be the company's revenue with new toll ?

The price of the diagnosis, paid by the client, varies according to the precision achieved by the team of specialists.

| Exam Accuracy | Price  | Rules                                  | Example          |
|:---------------|:---------------------|:---------------------------------------|:----------------|
| Above 50%     | min \$500\.00          | \+\$500 for each additional 5% accuracy | Accuracy = 55% \-> \$1,000\.00 |
| Up to 50%     | $0\.00                | N/A                                    | N/A               |


Our full original data set contains the records of 70.000 patients. Suppose we were to make them go through the clinic procedure to check if they have a cardiovascular disease, our model have reached an accuracy of `0.7652 (+/- 0.0159)` [74.93% , 78.11%] which is higher than the 55% to 65% that we have on today's procedures. Thus, translating it to business numbers.

|| Worst Scenario | Best Scenario |
|---|--------------------------------------|-------------------------------------|
|Today | \$35.000.000                         | \$105.000.000                      |
|Our model | \$174.476.786                         | \$196.768.971                      |

This means that having a portfolio of 70.000 patients that would go through the clinical procedure to check whether they have or not a cardiovascular disease, in the worst business scenario the portfolio would generate a profit of **\\$174.476.786 million** and in the best scenario **\$196.768.971 million**, in contrast to today's procedure that has an accuracy of 65% and would generate a total of \\$105 million, that's a difference of \\$91.768.971 million!

#### How reliable is the data result of the new tool ?

![28](https://github.com/nickolasdias/Cardio-Catch-Diseases/blob/master/image/28.png)

## References

### Context

- https://www.healthline.com/health/high-cholesterol/levels-by-age#adults

- https://www.paho.org/bra/index.php?option=com_content&view=article&id=5253:doencas-cardiovasculares&Itemid=1096

- https://hilab.com.br/blog/principais-doencas-cardiovasculares/

### Business Problem

- https://sejaumdatascientist.com/projeto-de-data-science-diagnostico-precoce-de-doencas-cardiovasculares/

### Suplementary Materials

- https://machinelearningmastery.com/calibrated-classification-model-in-scikit-learn/

- https://machinelearningmastery.com/roc-curves-and-precision-recall-curves-for-classification-in-python/

- https://machinelearningmastery.com/smote-oversampling-for-imbalanced-classification/
