
# Phase II: Oral Insulin Auralin Trials

> *(Disclaimer: The clinical dataset is fabricated for the sake of data wrangling practice on Udacity. It is constructed to simulate real-world dataset with the consults of real doctors. The 'auralin' and 'novodra' are NOT real insulin products, however, it mimics the real clinical trial for an inhaled insulin, Afrezza.)*

## Introduction
Diabetes is a chronic medical condition characterized by elevated blood glucose levels due to the body's inability to properly regulate insulin, a hormone responsible for controlling blood sugar. It is a global health concern, affecting millions of individuals worldwide. Proper management of diabetes is crucial in preventing complications such as heart disease, kidney failure, and vision problems.

One of the cornerstones of diabetes management is insulin therapy. Insulin is a hormone that helps regulate blood sugar by facilitating glucose absorption into cells. Many individuals with diabetes rely on insulin injections to maintain healthy blood sugar levels.

In the pursuit of optimizing diabetes management and enhancing patient care, the project focuses on the evaluation of the Auralin insulin treatment. To ensure the safety and effectiveness of Auralin, we will employ a rigorous comparative analysis, using Novodra as the standard insulin against which Auralin's safety and effectiveness will be measured.

## Goal of the Project

> To conduct a comprehensive analysis on oral insulin Auralin effectiveness, dosage optimization, side effects analysis, and patient demographic impact, with the objective of enhancing the personalized care of patients with diabetes.

## Problem Statements

In this project, we seek to answer the following questions:

>1. **Effectiveness Comparison**: Compare the effectiveness of Auralin and Novodra in reducing HbA1c levels. Are there statistically significant differences between the two groups in terms of HbA1c reduction? 

>2. **Dose Optimization**: Determine if there is an optimal dosage range for Auralin and Novodra that leads to the best HbA1c reduction. Is there a correlation between the initial dose, final dose, and HbA1c reduction?

>3. **Side Effects Analysis**: Analyze the side effects experienced by patients in both groups. Are there differences in the type and severity of side effects between Auralin and Novodra? Are there correlations between factors like gender,  weight and BMI and the likelihood of side effects?

## Outcome
By harnessing statistical techniques and Python programming, I have been able to unearth latent patterns within the dataset. Armed with this valuable information, I am poised to make data-driven decisions that will facilitate informed assessments of the safety and efficacy of auralin.

## Skills and Tools Used
* Programming Language: Python
* Project Management: Trello Board
* Data Manipulation
* Data Visualization
* Data Cleaning
* Data Exploartion 

## Data Preprocessing Issues
The dataset presented a multitude of challenges related to both data structure and data quality. Some of the issues include:

#### Duplicated Entries

> A comprehensive examination for duplicate entries shows a very unique form of duplicated entries. John Doe is a single patient with six different patient ID. 

![Duplicated entries](https://github.com/Bankrid/Auralin-clinical-trial/blob/main/Auralin/duplicated%20enteries.PNG)



#### Structural Anomaly

> Three distinct features: 'treatment', 'start_dose' and 'end_dose' are reported as two features: 'auralin' and 'novodra'.

![structure Anomaly](https://github.com/Bankrid/Auralin-clinical-trial/blob/a05e0ccc5bdd557ce5db8d5ef050097e68f48b1d/Auralin/structural%20anomaly.PNG)


### Cleaned Dataset
Following the comprehensive cleaning process aimed at addressing the identified dataset issues, here are the resultant outcomes.

![Cleaned Dataset](https://github.com/Bankrid/Auralin-clinical-trial/blob/main/Auralin/cleaned%20dataset.PNG)


## Insights

Below are some of the remarkable insights gleaned from this investigation.

#### Are patient on novodra or auralin has higher hba1c_change?


> There is a statistically significant difference (t = 3.08, p = 0.002, $\alpha$ = 0.05) in HbA1c changes between Novodra and Auralin treatments. Therefore, we reject the null hypothesis, concluding that 
Novodra leads to a significantly higher HbA1c change compared to Auralin.

![Hba1c Change](https://github.com/Bankrid/Auralin-clinical-trial/blob/main/Auralin/hba1c%20change.png)

#### Are adverse effects observed depend on the dose of auralin or novodra?

> Only Auralin causes adverse effects such as throat irritation and nausea. Also, these side effects tend to be more prevalent with higher doses of auralin. 

![Side Effect](https://github.com/Bankrid/Auralin-clinical-trial/blob/main/Auralin/side%20effects.png)


#### Does increase dose of auralin or novodra translate to increase HbA1c Reduction?

> There is an inverse relationship between the dosage of auralin (Corr. Coef. = -0.0730) and 
its corresponding impact on the HbA1c levels, whereas novodra (Corr. Coef. = 0.0898) demonstrates a direct proportional relationship with the response. Using  minimum effective dose of auralin, can mitigate the side effects. 

![Dose Correlation](https://github.com/Bankrid/Auralin-clinical-trial/blob/main/Auralin/dose%20correlation.png)                    



## Acknowledgements

 - [Awesome Readme Templates](https://awesomeopensource.com/project/elangosundar/awesome-README-templates)
 - [Awesome README](https://github.com/matiassingers/awesome-readme)
 - [How to write a Good readme](https://bulldogjob.com/news/449-how-to-write-a-good-readme-for-your-github-project)


## Authors

- [@octokatherine](https://www.github.com/octokatherine)


## Documentation

[Documentation](https://linktodocumentation)

