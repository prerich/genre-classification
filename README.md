# genre-classification

A machine learning program that learns to classify 12 music genres
genres:  ['electric', 'pop', 'rock', 'dance', 'folk', 'classical', 'traditional', 'jazz', 'metal', 'dj', 'latin', 'country']
by a short english description.

the dataset is called MusicCaps from https://www.kaggle.com/datasets/googleai/musiccaps it includes an aspect list and a caption from a musician


Summary:
Its a multilabel classiication problem.

The model uses Count Vectorizer to extract all the captions into a matrix, where each row represents a caption and each column represents a unique word in the corpus. The value in each cell is the number of occurrences of that word in that caption. The model also uses logistic regression to detect the presence or absence of genres, based on the frequency of words associated with each genre. The model uses a threshold of 50% probability to determine whether a genre is present, and the probability calculation is done using the limited-memory Broyden-Fletcher-Goldfarb-Shannon algorithm. 


Results:
The model was trained on a dataset of captions and their corresponding genres, with 12 genres in total. The model achieved an overall accuracy score of 0.70 and the individual scores for each genre varied between 0.54 and 0.96. The genres with the highest scores were electric, classical, and latin, while the genres with the lowest scores were dj and metal. The frequency of labels in the dataset was also provided, with electric being the most frequent and traditional being the least frequent.

***Score for each label****
score: 0.7075892857142857
              precision    recall  f1-score   support

    electric       0.98      0.95      0.96       175
         pop       0.94      0.77      0.85       104
        rock       0.88      0.89      0.89        84
       dance       0.78      0.67      0.72        73
        folk       0.88      0.86      0.87        43
   classical       1.00      0.88      0.94        41
 traditional       0.96      0.60      0.74        40
        jazz       1.00      0.73      0.84        33
       metal       0.88      0.58      0.70        24
          dj       0.77      0.42      0.54        24
       latin       0.92      0.96      0.94        23
     country       1.00      0.86      0.93        22

   micro avg       0.92      0.81      0.86       686
   macro avg       0.91      0.76      0.83       686
weighted avg       0.92      0.81      0.86       686
 samples avg       0.90      0.86      0.86       686
