# Cervical_cancer_risk_factors
Data was retrieved from the UCI Machine Learning repository, original survey conducted at Hospital Universitario de Caracas in Caracas, Venezuela. Each column represents a question on a survey, each row represents one participant's responses. Participants were kept anonymous and were permitted to skip survey questions. 

This is a classification project to build a model able to predict whether a person will have a positive diagnosis of cervical cancer based on risk factors. Four diagnostic tests were available as targets, Hinselman and Schiller tests, cytological examination, and biopsy. 

![image](https://user-images.githubusercontent.com/91214731/155193429-777fc581-af17-4472-bd07-9f78e0e2be5a.png)

Some insights from the exploratory data analysis include that more than half of the participants had a history of use of hormonal contraceptives.

![image](https://user-images.githubusercontent.com/91214731/155192816-2234d98b-fd6e-4e87-9037-e6a4284d2ee8.png)

However, the grand majority of participants who used hormonal contraceptives used them for less than 5 years.

![image](https://user-images.githubusercontent.com/91214731/155193485-7e9c9439-6e37-408a-8f40-a897d5ff3c4a.png)

Most of the participants reported never having an STD. The majority of the questions in this survey revolve around specific STD's, this indicates that this survey design has issues with gathering useful data. Revision of questions for the next application of data gathering is recommended.

Some tree based models and neural networks both proved to have difficulty predicting the positive class (positive biopsy for cervical cancer). This is primarily due to aforementioned class imbalances in the dataset. Despite this, LGBClassifier and RandomForestClassifier both were able to classify correctly more than half of the positive class, based on F1 score, recall, and precision metrics.
