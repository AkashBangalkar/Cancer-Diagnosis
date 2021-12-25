# Personalized Cancer Diagnosis

### Business Problem
Data: Memorial Sloan Kettering Cancer Center (MSKCC)

Download training_variants.zip and training_text.zip from Kaggle.

**Context:**
Source: https://www.kaggle.com/c/msk-redefining-cancer-treatment/discussion/35336#198462

**Problem statement:**
Classify the given genetic variations/mutations based on evidence from text-based clinical literature.

### Real-World/Business Objectives and Constraints
- No low-latency requirement.
- Interpretability is important.
- Errors can be very costly.
- Probability of a data-point belonging to each class is needed.

### Data Overview
- **Source:** https://www.kaggle.com/c/msk-redefining-cancer-treatment/data
- We have two data files: one conatins the information about the genetic mutations and the other contains the clinical evidence (text) that human experts/pathologists use to classify the genetic mutations.
- Both these data files are have a common column called ID
**Data file's information:**
  - training_variants (ID , Gene, Variations, Class)
  - training_text (ID, Text)
 
*Preprocessing Text Data

*Checking Null Values

**Merging both gene variations and text data**

*Perform Exploratory Data Analysis

**Univariate Analysis
- Response Coding with Laplace Smoothing
- Univariate Analysis on Gene Feature
- Featurizing Gene Feature
- Univariate Analysis on Variation Feature
- Featurizing Variation Feature
- Univariate Analysis on Text Feature

[Click Here](https://github.com/akashbangalkar/cancer_diagnosis/blob/main/Cancer_Diagnosis.ipynb) To Check Total Work on Case Study.

### Machine Learning Models
*Stacking all the three types of features

| Model         | Log Loss |
| ------------- | -------- |
| Naive Bayes  | 1.3007  |
| KNN Classification | 1.0827  |
| Logistic Regression (With Class Balancing) | 1.2266 |
| Logistic Regression (Without Class Balancing) | 1.2201 |
| Linear Support Vector Machines | 1.2283 |
| Random Forest Classifier | 1.1755 |
| Stacking Model | 1.2749 |
| Maximum Voting Classifier | 1.2356 |





