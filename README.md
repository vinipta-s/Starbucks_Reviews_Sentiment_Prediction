# Starbucks Reviews Sentiment Prediction Project

Starbucks store reviews consisted of customer 'name', store 'location', 'Date'. 'Rating' from 1-5, 'Review' and 'Image_links'. 

In this project, the data was cleaned and filtered for US Starbucks reviews and a sentiment label categorical columns (1: positive, 0: negative) was created. Two text processing methods were used to build models and determine the best method and model for accurate sentiment prediction. For comparision and shorter run time, the first 50 padded sequences and embeddings of each review was used as the features. 

Models used: Dummy Classifier, Logistic Regressor, Random Forest Classifier and Light Gradient Boosting Model Classifier. 

Project overview:
1. Libraries
2. Load Data
3. Data Cleaning
4. Filtering US Starbucks reviews
5. Data Visualization
   * reviews count per state
   * pi chart of ratings
6. Traditional text processing: Tokenization, Stopword removal, Lemmatization, bi-grams
7. Most frequent Bigrams
8. Functions: upsampling and model evaluation (Accuracy, F1, APS, AUC_ROC)
9. Method 1: padded sequences were used to train and evaluate models
  * Best model on the test set: Random Forest Classifier
10. Method 1: BERT embeddings were used to train and evaluate models
  * Best model on the test set: Logistic Regressor
11. Overall the tuned Logistic Regressor trained with Bert embeddings performed the best on the test set wiht 0.94 accuracy, 0.92 ROC AUC and F1 score and APS of 0.85 and 0.86 respectively.
    
