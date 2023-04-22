# genre-classification

Music Genre Classification with Captions

This project aims to classify music genres based on their captions using machine learning. The model uses Count Vectorizer to extract features and logistic regression to detect the presence or absence of each genre label.


### Dataset: <br>
The dataset consists of captions and their corresponding genres, with 12 genres in total: electric, pop, rock, dance, folk, classical, traditional, jazz, metal, dj, latin, and country.

the dataset is called MusicCaps and its from https://www.kaggle.com/datasets/googleai/musiccaps it includes an aspect list and a caption from a musician

### Results: <br>
The model achieved an overall accuracy score of: **0.70** , with individual scores for each genre varying between 0.54 and 0.96. The genres with the highest scores were electric, classical, and latin, while the genres with the lowest scores were dj and metal. The score for each label is provided below:

Score for each label: 

Label       | Precision | Recall | F1-Score | Support
------------|-----------|--------|----------|--------
electric    | 0.98      | 0.95   | 0.96     | 175
pop         | 0.94      | 0.77   | 0.85     | 104
rock        | 0.88      | 0.89   | 0.89     | 84
dance       | 0.78      | 0.67   | 0.72     | 73
folk        | 0.88      | 0.86   | 0.87     | 43
classical   | 1.00      | 0.88   | 0.94     | 41
traditional | 0.96      | 0.60   | 0.74     | 40
jazz        | 1.00      | 0.73   | 0.84     | 33
metal       | 0.88      | 0.58   | 0.70     | 24
dj          | 0.77      | 0.42   | 0.54     | 24
latin       | 0.92      | 0.96   | 0.94     | 23
country     | 1.00      | 0.86   | 0.93     | 22


### Conclusion <br>
The model was able to successfully classify music genres based on their captions, with an overall accuracy of 0.70. However, there is room for improvement in the individual scores for each genre. Further experimentation with different feature extraction methods and machine learning algorithms could potentially improve the model's performance.
