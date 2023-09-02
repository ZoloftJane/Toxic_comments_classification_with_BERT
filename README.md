# Toxic_comments_classification_with_BERT
## ML for Text project from Practicum by Yandex
The goal of this project was to develop a model that classifies comments into toxic and nontoxic.

The F1 score on the test set should be at least 0.75.

This project's repo includes the project's jupyter notebook (Movie_reviews_classification_with_BERT.ipynb).

We have completed the following steps in this project:

1.Descriptive statistics

2.Data preprocessing

We removed a few missing values and checked the data for duplicates. We have also normalized the comments by removing any digits, punctuations marks etc. and converting them to lower case letters.

3.EDA

We analyzed distributions of toxic and nontoxic comments. External imbalance classes: strong comments are 10 times less than non-toxic ones. This must be taken into account when modeling.

Also we made the frequency analysis of toxic comments and wordClouds with bad and good word.

4.Splitting the data

Data was split into train and test sets with the 25/75 ratio.

5.Model selection

We tried 2 libraries for text preprocessing - nltk and spaCy. Logistic Regression, RandomForest and LightGBM models were used. We used pipeline for vectorizing texts and GridSearch for fittng hyperparameters.
And we used the toxic_BERT model.

6. Results

Based on our research, the Logistic Regression model showed the best test F1 score - over 75%. 

The toxic BERT showed the highest F1 score 91%.
