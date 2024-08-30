# Fall_Detection_Wearable-Sports

The link to the dataset:
### https://www.kaggle.com/datasets/kmknation/mobifall-dataset-v20

With the proliferation of wearable sports technology, there is a growing interest in leveraging
predictive analytics to enhance user experience and safety. This project focuses on the
application of predictive analytics using the MobiFall dataset, aiming to develop robust
models for detecting and predicting falls in the context of wearable sports devices. The
MobiFall dataset, a rich collection of accelerometer and gyroscope data captured during
various fall scenarios, serves as the foundation for training and evaluating predictive models.
The project encompasses data preprocessing, feature engineering, and the implementation of
machine learning algorithms to analyse patterns within the sensor data. The predictive models
aim not only to identify falls accurately but also to provide insights into the context
surrounding the falls, such as the type and intensity of physical activity leading up to the
event. Furthermore, the project explores the integration of real-time data from wearable
devices to enable proactive alerts and interventions, contributing to the overall safety and
performance optimization of athletes and sports enthusiasts.

## Data Collection
In this study, the MobiFall dataset is used as the primary source of data for predictive
analytics in the context of wearable sports technology. The MobiFall dataset is a well-known
dataset in the field of fall detection and activity recognition, but it can be adapted for the
purposes of injury prediction in sports due to its rich accelerometer data.
MobiFall Dataset
The MobiFall dataset includes data collected from wearable sensors (smartphones) worn by
individuals during various activities, including falls. This dataset contains the following key
components:
· Accelerometer Data: Accelerometer readings from the smartphone sensors
provide information about changes in acceleration along the x, y, and z axes.
These readings are collected at regular intervals (e.g., 100Hz) during different
activities, including falls.
· Activity Labels: Each data point is associated with an activity label, which
indicates the specific activity being performed at that time (e.g., walking, running,
standing, or falling). The dataset provides a ground truth for the activities,
including fall events.

## Data Preprocessing
Adapting the MobiFall dataset for injury prediction in sports requires specific preprocessing
steps:
· Data Selection: Relevant portions of the MobiFall dataset are extracted, focusing
on activities that are analogous to sports-related movements and scenarios. This
includes activities that involve rapid accelerations or movements similar to those
in sports.
· Data Transformation: Accelerometer data is transformed to represent relevant
features for injury prediction. This may involve calculating metrics such as peak
accelerations, jerk, or spectral analysis to capture the characteristics of movements
that are indicative of injury risk.

## Predictive Model Development
With the preprocessed MobiFall dataset, the development of predictive models for injury
prevention in sports proceeds as follows:
· Feature Engineering: Features specific to sports-related injury prediction are
engineered from the transformed accelerometer data. For example, features related
to impact forces, abrupt changes in direction, or irregular movements are created
to capture injury risk factors.
· Model Selection: Various machine learning algorithms are considered for
building predictive models. Given the nature of the data and the problem,
algorithms such as decision trees, random forests, support vector machines, or
deep learning models may be evaluated for their suitability.
· Model Training: The selected predictive model(s) are trained using the modified
dataset. Training involves optimizing model parameters to accurately predict
injury risks based on the engineered feature.

## Implementation
1. Import libraries for dataset creation
2. Delete folders that are not related to our project: Activities like Standing(STD),
Walking (WAL), Sit Chair(SCH), Car Step In(CSI), Car Step Out(CSO) and Fall type
such as Back Sitting Chair(BSC)
3. Combine the data from all 15 subjects
   ![image](https://github.com/user-attachments/assets/7479dc49-44bc-44eb-89be-d0838ec34184)
   ![image](https://github.com/user-attachments/assets/83691a72-9e84-458c-b6e0-f56d6c2e1603)


4. Perform preprocessing operations like handling nulls, standardizing timestamps, dropping unused features and inserting a whether a fall has ocured column to get final dataset
5. Perform Exploratory Data Analysis to get insight of the distribution of the various
sensor data
![image](https://github.com/user-attachments/assets/69126b2b-4bb4-4760-a464-ea0e595b98e2)
![image](https://github.com/user-attachments/assets/37bb4ed8-ea04-4233-aec1-a80e306bd587)
![image](https://github.com/user-attachments/assets/06f92603-bdb1-4837-b0a4-518e1599b396)
![image](https://github.com/user-attachments/assets/6b938ba2-0e0e-4ed3-a6d8-725320bcdea2)
![image](https://github.com/user-attachments/assets/0d435af1-9855-4485-a630-27d448c249d9)
![image](https://github.com/user-attachments/assets/3bc56f6a-3912-47c3-9771-c2f244984eac)
![image](https://github.com/user-attachments/assets/b98e7ffd-d601-4a74-b811-7e784070d5d2)
![image](https://github.com/user-attachments/assets/4ac0c062-2b5b-47f4-94d9-59d11a5bedf7)
6. Obtain features such as Mean, Variance, Skewness and Kurtosis values as a feature
matrix
7. Impute missing values with the mean of existing values
8. Split the data for train and test
9. Splitting data into features and labels to use Isolation Forest Regression
10. Prediction of anomalies and derive anomaly scores
11. Visualise anomaly score distribution
![image](https://github.com/user-attachments/assets/9c20af35-acfe-4cb0-bf97-a3752561eb69)
12. Display accuracy
13. Testing the model with own input and using feature extraction
![image](https://github.com/user-attachments/assets/bdacb3c3-b7a7-46e0-8459-e71dff28fe17)
14. Using our model to predict whether the input is anomaly or not
![image](https://github.com/user-attachments/assets/206b94ee-b768-448d-bcb8-66c9411093e4)

