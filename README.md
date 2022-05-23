# Insomnia-Analysis-
We submitted a questionnaire to the students enrolled at Msc in data science concerning sleep problems. Using python, we then analysed the results 

# Insomnia Analysis

We submitted a questionnaire to the students enrolled at Msc in data science concerning sleep problems. Using python, we then analysed the results

# 1. Introduction

Our project concerns the prediction of whether a person had sleep problems according to the answers we collected through the questionnaire. The prediction is done through the k-nearest neighbours (KNN)

We believe that this is an important topic to address because Covid-19 has radically changed our lifestyles, particularly that of students and workers. Just try to think about how many hours we spend in front of our screens and how much anxiety and uncertainty this pandemic has generated in us, these are all factors that can then lead to difficulty in falling asleep, concentration and many others.

# 2. Methods
Data collection:

the project started with the administration of a questionnaire on Google forms concerning the use of mobile phones, focusing more on the habits and the time spent on the screen of everyone.
Then it was supplemented with answers from other questionnaires that we managed to receive from our colleagues on the course.
Discussion/features:

Sessions were then carried out to understand which variables to take from the questionnaire and decide on which issues to implement our algorithm. To predict whether a person has had problems falling asleep recently, we used three variables:

    Phone daily usage (expressed in units of time)

    Study daily hours (expressed in units of time)

    Stress level (from a scale of 1 to 7).

#Feature engineering:

Before starting to implement the algorithm to our dataset, we proceeded as the data science process dictates with feature work.
We transformed the variable "sleeping difficulty" via the "one hot encoding" method into 1 if a person had problems recently 0 otherwise. Then for the independent variables, we brought them on the same scale since the KNN chooses the k closest to the neighbours and then based on that, it assigns the class or predicts a value.

#Algorithm:

Among the most plausible algorithms for our classification problem are logistic regression and knn. The reasons why we chose knn: First, we have a small dataset of 30 data points. Second, we have appropriately labelled data because we are predicting someone is having sleeping disorder or not, the outcome can be 1 or 0.
Finally, we choose knn because it is a non-parametric method, and it is suitable when we are considering the order of something, where even if the numerical data change, but the outcome may remain the same.

#Model training:

Before proceeding to model training, we performed the data split, 25% as test data. This process is necessary to test the performance of the model we are going to implement.
Then as a performance metric we chose k = 5 following the elbow method, which is one of the most popular methods of determining the optimal value of k.

#Authors

- Enrico Romano
- Simone Lu
