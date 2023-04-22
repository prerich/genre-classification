# genre-classification

A machine learning program that learns to classify 12 music genres
genres:  ['electric', 'pop', 'rock', 'dance', 'folk', 'classical', 'traditional', 'jazz', 'metal', 'dj', 'latin', 'country']
by a short english description.

the dataset is called MusicCaps from https://www.kaggle.com/datasets/googleai/musiccaps it includes an aspect list and a caption from a musician


Summary:
Its a multilabel classiication problem.

The model uses Count Vectorizer to extract all the captions into a matrix, where each row represents a caption and each column represents a unique word in the corpus. The value in each cell is the number of occurrences of that word in that caption. The model also uses logistic regression to detect the presence or absence of genres, based on the frequency of words associated with each genre. The model uses a threshold of 50% probability to determine whether a genre is present, and the probability calculation is done using the limited-memory Broyden-Fletcher-Goldfarb-Shannon algorithm. 


Results:
The model was trained on a dataset of captions and their corresponding genres, with 12 genres in total. The model achieved an overall accuracy score of 0.707 and the individual scores for each genre varied between 0.54 and 0.96. The genres with the highest scores were electric, classical, and latin, while the genres with the lowest scores were dj and metal. The frequency of labels in the dataset was also provided, with electric being the most frequent and traditional being the least frequent.
