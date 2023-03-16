Microsoft Cloud Challenge
https://developer.microsoft.com/en-US/offers/30-days-to-learn-it

# GLA-ICT
ICT Training Materials

AI 900 Study Materials
https://learn.microsoft.com/en-us/certifications/exams/ai-900/

git clone https://github.com/MicrosoftLearning/AI-900-AIFundamentals ai-900

https://azure.microsoft.com/en-us/contact/#contact-sales

Custom Vision Portal
https://www.customvision.ai/

Object Detection Training Images 
https://github.com/MicrosoftLearning/mslearn-ai900/blob/main/data/object-detection/object_training.zip

Bike Rentals Dataset 
https://aka.ms/bike-rentals

Diabetic Dataset
https://aka.ms/diabetes-data

Sample Data to be entered 
 PatientID,Pregnancies,PlasmaGlucose,DiastolicBloodPressure,TricepsThickness,SerumInsulin,BMI,DiabetesPedigree,Age
 1882185,9,104,51,7,24,27.36983156,1.350472047,43
 1662484,6,73,61,35,24,18.74367404,1.074147566,75
 1228510,4,115,50,29,243,34.69215364,0.741159926,59


import pandas as pd

def azureml_main(dataframe1 = None, dataframe2 = None):

    scored_results = dataframe1[['Scored Labels', 'Scored Probabilities']]
    scored_results.rename(columns={'Scored Labels':'DiabetesPrediction',
                                'Scored Probabilities':'Probability'},
                        inplace=True)
    return scored_results
