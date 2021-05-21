# Data-driven prediction of chronic disease development

We use modern techniques in data science to build a predictive model for the identification of Chronic Obstructive Pulmonary Disorder (COPD) from clinical and laboratory data. COPD is a leading cause of deaths worldwide, esp. in highly urbanized regions. 

## Installation

The libraries used are `sklearn`, `numpy`, `xgboost`, and `pandas`. It is recommended to use the Anaconda distribution of Python. The code should run with no issues using Python versions 3.*.

## Motivation

COPD is becoming more prevalent as our society is increasing getting more affluent and more people are exposed to low physical activities. It is also one major concern during this pandemic because it could make one more likely to get severely ill from COVID-19 - see CDC advice [here](https://www.cdc.gov/coronavirus/2019-ncov/need-extra-precautions/people-with-medical-conditions.html).


## Files

* `CRISP-DM Analysis.ipynb` - main notebook for analysis
* `finaldata.csv` - the dataset used
* `*.png` - images for blog post

## Results

There are three main business questions in the analysis:
1. What are the clinical features that are predictive of COPD?
2. Which ML model can predict COPD from clinical and genetic data?
3. Which are the most important features that play major role in the predictive model?

These questions are important because COPD (which often co-occurs with other chronic diseases such as cardiovascular disease and diabetes) is becoming more prevalent as our society becomes more affluent and lethal diseases are being eradicated. Because COPD is incurable and progressive, an early detection of the disease could be a life-saver.

In summary, the important clinical features are age, sex, and smoking status. kNN, XGB, logistic regression, neural network, SVM, and decision tree can predict COPD well from SNPs and patient data. It turns out that air quality index (using location as surrogate feature) is the most important predictor of COPD. For more details, please see the blog post and notebook.

## Acknowledgements

We use regression and boosted tree models on [data from the Chinese population](https://translational-medicine.biomedcentral.com/articles/10.1186/s12967-020-02312-0).