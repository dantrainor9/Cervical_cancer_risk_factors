# Cervical_cancer_risk_factors
Data was retrieved from the UCI Machine Learning repository, original survey conducted at Hospital Universitario de Caracas in Caracas, Venezuela. Each feature column represents a question on a survey, each row represents one participant's responses. Participants were kept anonymous and were permitted to skip survey questions. 

This is a classification project to build a model able to predict whether a person will have a positive diagnosis of cervical cancer based on risk factors. Four diagnostic tests were available as targets, Hinselman and Schiller tests, cytological examination, and biopsy. Initially, biopsy was used as the target for model development (see video presentation for more information).

![image](https://user-images.githubusercontent.com/91214731/156416571-220ce538-7052-4082-986b-5ffb288c90c9.png)

Some insights from the exploratory data analysis include that more than half of the participants had a history of use of hormonal contraceptives.

![image](https://user-images.githubusercontent.com/91214731/156416724-28caa324-6699-48a1-a8b0-7d172b744830.png)

However, most of the participants who used hormonal contraceptives used them for less than 5 years, with the most participants using them for 0-1 years.

![image](https://user-images.githubusercontent.com/91214731/156416914-29dedfb7-157f-4665-95a7-574f6c5820d8.png)

Most of the participants reported never having an STD. The majority of the questions in this survey revolve around specific STD's, this indicates that this survey design has issues with gathering useful data. 

![image](https://user-images.githubusercontent.com/91214731/156417643-3f466e4c-27f6-4fff-a468-2dadd0020df7.png)

For example, above is the distribution of participants with any previous diagnoses of HPV. Survey revision for the next round of data gathering is recommended to improve model performance.

Some tree based models and neural networks both proved to have difficulty predicting the positive class of the target variable (in this case, positive biopsy for cervical cancer). This is primarily due to aforementioned class imbalances in the dataset. Despite this, LGBClassifier and RandomForestClassifier both were able to classify correctly 95% of the negative class and more than half of the positive class, based on F1 score, recall, and precision metrics. With improved data, this model can be further improved.
