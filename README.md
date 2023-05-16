# Automatic Ticket Classification
> Create a model that can automatically classify customer complaints based on the products and services that the ticket mentions.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
For a financial company, customer complaints carry a lot of importance, as they are often an indicator of the shortcomings in their products and services. If these complaints are resolved efficiently in time, they can bring down customer dissatisfaction to a minimum and retain them with stronger loyalty. This also gives them an idea of how to continuously improve their services to attract more customers. 

 

These customer complaints are unstructured text data; so, traditionally, companies need to allocate the task of evaluating and assigning each ticket to the relevant department to multiple support employees. This becomes tedious as the company grows and has a large customer base.

The financial company wants to automate its customer support tickets system. As a financial company, the firm has many products and services such as credit cards, banking and mortgages/loans. 

With the help of non-negative matrix factorization (NMF), an approach under topic modelling, we will detect patterns and recurring words present in each ticket. This can be then used to understand the important features for each cluster of categories. By segregating the clusters, we will be able to identify the topics of the customer complaints.



<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
Since the given data was not labelled, we needed to apply NMF to analyse patterns and classify tickets into the following five clusters based on their products/services:

* 1.Credit card / Prepaid card
* 2.Bank account services
* 3.Theft/Dispute reporting
* 4.Mortgages/loans
* 5.Others 

With the help of topic modelling, we are be able to map each ticket onto its respective department/category. 

We use multiple classification model for predition and observe following
Observations :
* Logistic regression : Accuracy is 0.92 , f1-scores are 0.93, 0.93, 0.91 ,0.90 and 0.93 for classess "Bank account services", "Credit card / Prepaid card", "Others", "Theft/Dispute reporting", "Mortgages/loans" respectively.

* Decision Tree : Accuracy is 0.79 , f1-scores are 0.80, 0.81, 0.75, 0.74 and 0.82 for classess "Bank account services", "Credit card / Prepaid card", "Others", "Theft/Dispute reporting", "Mortgages/loans" respectively.

* Random Forest : Accuracy is 0.72 , f1-scores are 0.79, 0.73, 0.06, 0.73 and 0.79 for classess "Bank account services", "Credit card / Prepaid card", "Others", "Theft/Dispute reporting", "Mortgages/loans" respectively.

* Naive Bayes (optional) : Accuracy is 0.35 , f1-scores are 0.33,0.39, 0.23, 0.38 and 0.47 for classess "Bank account services", "Credit card / Prepaid card", "Others", "Theft/Dispute reporting", "Mortgages/loans" respectively.

From above analysis , we can see that Logistic regression is giving best accuracy and f1-scores.
<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- Numpy
- Pandas
- nltk
- seaborn 
- matplotlib
- sklearn

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
Give credit here.
- This project was inspired by upGrade AI & ML course case study

## Contact
Created by @sandipanp - feel free to contact me!


