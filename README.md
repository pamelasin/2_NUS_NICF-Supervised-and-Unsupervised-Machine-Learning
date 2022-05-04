# NUS - NICF Supervised and Unsupervised Machine Learning

## **Description**
- Machine learning model that predicts which Tweets are about real disasters and which one’s are not
- https://www.kaggle.com/c/nlp-getting-started/overview
- Create new features such as url_count, word_count, char_per_word, stopwaords_count, polarity, subjectivity, punc_count from Tweets
- Univariate, bivariate analysis, correlation heatmap
- Pipelines:
    - Pipeline 1: logreg + countvect
    - Pipeline 2: logreg + tfidf
    - Pipeline 3: SGD + tfidf
    - Pipeline 4: SVM + tfidf
- GridsearchCV for each pipeline 
    - Remove stop words | None
    - Lemmatizer | Stemmer | None
    - 1-gram | 1-gram and 2-gram
- Assuming stratification, a dumb model predicting the majority class has a 57% accuracy. 
- Pipeline 3 has best F1 score = 0.81
- Best model and parameters:
    - TFIDF
    - ngram_range = (1, 2)
    - Don't remove stop words
    - SGD
    - alpha = 0.0001
    - loss = 'hinge'
    - penalty = 'elasticnet
- Score of 0.79252 on Kaggle
- Files include dataset and Python code. 


## **Python code excerpts**
[![Capture.png](https://i.postimg.cc/T29b4Gv7/Capture.png)](https://postimg.cc/vD4D4JBf)

[![Capture.png](https://i.postimg.cc/4ybjzyKT/Capture.png)](https://postimg.cc/PvJ6Htz6)

[![Capture.png](https://i.postimg.cc/YSWn60Vy/Capture.png)](https://postimg.cc/94cYVmcG)

[![Capture.png](https://i.postimg.cc/HnsqH5WP/Capture.png)](https://postimg.cc/BLkYBjKx)

[![Capture.png](https://i.postimg.cc/P5m23JTL/Capture.png)](https://postimg.cc/Mnp7XWcx)

[![Capture.png](https://i.postimg.cc/Cxzm07Gq/Capture.png)](https://postimg.cc/PCnmzmFX)

[![Capture.png](https://i.postimg.cc/RCpgD2fB/Capture.png)](https://postimg.cc/K4L7KqJq)

[![Capture.png](https://i.postimg.cc/w3KLd5gh/Capture.png)](https://postimg.cc/N2456HyM)

[![Capture.png](https://i.postimg.cc/wxDhhPV2/Capture.png)](https://postimg.cc/qgMhr1W6)

[![Capture.png](https://i.postimg.cc/fyMk7Hzq/Capture.png)](https://postimg.cc/0MH8P0J7)
