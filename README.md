# Introduction

This project aims to **build a predictive model** to accurately determine whether a patient will suffer from a newly discovered disease, Parasite Smith. In order to do this, access was granted to 800 training observations and 225 test observations obtained from a set of patients.

The prediction score is the percentage of cases that we predict correctly using the **f1 score**.

A small amount of sociodemographic, health and behavioural information obtained from patients is available.


# Datasets
We had access to two different data sets:

1. The training set: used to build the machine learning models. 
In this set, it also has the ground truth associated with each patient, i.e. if the patient has the disease (Disease = 1) or not (Disease = 0). 
It is composed of:

    - train demo.csv - the training set for demographic data and the target
    - train health.csv - the training set for health related data
    - train habits.csv - the training set for habits related data
    
    
2. The test set: used to see how well the model performs on unseen data. 
In this set there is no access to the ground truth, and the goal is to predict that value (0 or 1) using the model created using the training set. 
Is composed by:

    - test demo.csv - the test set for demographic data
    - test health.csv - the test set for health related data
    - test habits.csv - the test set for habits related data

The available data contains the following attributes:

##### Sociodemographic Data 

| Attribute  | Description |
|------------|-------------|
| PatientID  | The unique identifier of the patient |
| Birth Year | Patient Year of Birth |
| Name       | Name of the patient |
| Region     | Patient Living Region |
| Education  | Answer to the question: What is the highest grade or year of school you have? |
| Disease    | The dependent variable. If the patient has the disease (Disease = 1) or not (Disease = 0) |


##### Health Related Data

| Attribute       | Description  |
|-----------------|--------------|
| PatientID       | The unique identifier of the patient |
| Height          | Patient’s height |
| Weight          | Patient’s weight |
| Checkup         | Answer to the question: How long has it been since you last visited a doctor for a routine Checkup? [A routine Checkup is a general physical exam, not an exam for a specific injury, illness, or condition.] |
| Diabetes        | Answer to the question: (Ever told) you or your direct relatives have diabetes? |
| HighCholesterol | Cholesterol value |
| BloodP ressure  | Blood Pressure in rest value |
| Mental Health   | Answer to the question: During the past 30 days, for about how many days did poor physical or mental health keep you from doing your usual activities, such as self-care, work, or recreation? |
| Physical Health | Answer to the question: Thinking about your physical health, which includes physical illness and injury, for how many days during the past 30 days was your physical health not good to the point where it was difficult to walk?  |

##### Habits related Data

| Attribute      | Description |
|----------------|-------------|
| PatientID      | The unique identifier of the patient |
| Smoking_Habit  | Answer to the question: Do you smoke more than 10 cigars daily? |
| Drinking_Habit | Answer to the question: What is your behavior concerning alcohol consumption? |
| Exercise       | Answer to the question: Do you exercise (more than 30 minutes) 3 times per week or more? |
| Fruit_Habit    | Answer to the question: How many portions of fruits do you consume per day? |
| Water_Habit    | Answer to the question: How much water do you drink per day? |