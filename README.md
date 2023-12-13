
## Project Title

# Stroke-Prediction-ML-Model
## Overview

The goal of this ML model is to figure out if a person will experience a stroke on the basis of age, nature of work, urban/rural residency, marital status, and several clinical parameters.
## File Structure

- Stroke ML Prediction Model.ipynb: Python Notebook containing the trained models.

- README.md: Project documentation providing an overview, usage instructions, and other relevant information.
## Steps

All the steps to process data and prepare for model are explained in python notebook. For quick learning, you can run this python codes on Kaggle.
## Dataset Description

### Data Set Characteristics

- **Number of Instances:** 4088
- **Number of Attributes:** 10 numeric and categorical, the target [categorical]

### Attribute Information

1. Gender: "Male", "Female" or "Other"
2. Age: age of the patient
3. Hypertension: 0 if the patient doesn't have hypertension, 1 if the patient has hypertension
4. Heart_disease: 0 if the patient doesn't have any heart diseases, 1 if the patient has a heart disease
5. Ever_married: "No" or "Yes"
6. Work_type: "children", "Govt_jov", "Never_worked", "Private" or "Self-employed"
7. Residence_type: "Rural" or "Urban"
8. Avg_glucose_level: average glucose level in blood
9. Bmi: body mass index
10. Smoking_status: "formerly smoked", "never smoked", "smokes" or "Unknown"*
11. Target variable: Stroke: 1 if the patient had a stroke or 0 if not (Prediction)

### Missing Attribute Values

BMI - 162

### Source

This dataset is part of Kaggle Competition. [Link to the Competition](https://www.kaggle.com/competitions/stroke-prediction-by-123-of-ai-dec-2023/overview)
## **Machine Learning Steps** 

We will run various machine learning techniques to prepare and optimize the model.

### **Supervised learning**

We will employ supervised learning techniques. Specifically, the model methods that can handle categorical and numerical values.

Step 1: Data preprocessing
- Data has null value: BMI column has 162 null values. 162 is just 4% of sample, however we will fill this null cell with mean of BMI.
- We will convert categorical values to on-hot encoding.
- We will drop few redundant and unrequired columns. ['Residence_type_Rural','Residence_type_Urban','gender_Other', 'gender_Male', 'gender_Female','ever_married_No']
- Check for Duplicate row values

Step 2: Model Training and Internal Evaluation
Here, we have listed following models to test stroke prediction capability.
- Logistic Regression
- Decision Tree
- Random Forest
- Gradient Boosting Classifier
- Support Vector Machine
- Neural Network
- K-Nearest Neighbors

All the steps and procedure to run this model is given in the python notebook.

On top of internal evaluation parameters, we will test this models to test new data available at competition. Based on that, we will select the best performing model.

Gradient Boosting Classifier resulted best score of 0.2352.

While this is not a good score, our learning is still on and expect improvement in this models. As of now, only beginer level of model optimization was carried out. Will move towards advanced optimzation techniques and select best performance.
Learning is still on.
## Acknowledgements

 - [Scikit-learn](https://scikit-learn.org/stable/about.html)
 - [123ofAI](https://123ofai.com/)
 - [Readme Editor](https://readme.so/editor)
## License

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
