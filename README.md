
# Disease prediction from drug review sentiments

This project's goal is to categorize patient conditions using drug reviews. The most frequent 10 diseases were considered from a total of 150 diseases.

## Features:

DrugName (categorical): The name of the medication under review by the patient. This feature will be used to categorize reviews by substance and evaluate how well each medication works for various ailments.

Condition (categorical): The diagnosis for which the patient is evaluating the medication. Reviews pertaining to depression, high blood pressure, and type 2 diabetes will be found using this tool.

Review (text): The drug's evaluation by the patient. This function will be used to gather information on the efficacy and potential negative effects of medications for particular illnesses.

Rating (in numbers): a patient rating of 10 stars indicating their overall happiness with the medication. This function will be employed to comprehend the degree of patient satisfaction with various medications for particular ailments.

Date: The date that the review was submitted. This function will be used to examine patterns in patient evaluations and ratings over time.

UsefulCount (numerical): The number of users who thought the review informative is called the "UsefulCount" (numerical). The reviews that are most likely to be useful in evaluating the efficacy and possible side effects of medications for particular diseases will be identified using this feature.



## Data Cleaning


1. Removed HTML characters since the data was obtained via webscraping.

2. Removed Symbols

3. Removed Stopwords

4. Stemmatized the data using Porter Stemmer

## Word Embedding and Model Building

TF-IDF was applied to the review column to create a feature matrix. Multinomial Naive-Bayes was used to predict the disease from the review.
