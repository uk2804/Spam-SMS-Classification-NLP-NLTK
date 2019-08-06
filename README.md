# Spam SMS classification 

## Use-case: 

The use of mobile phones has skyrocketed in the last decade leading to a new area for junk promotions from disreptable marketers. 

People innocently give out their mobile phone numbers while utilizing day to day services and are then flooded with spam promotional messages.

In this repo, classifying SMS messages into two differnet classes (Spam or Ham) 

## Data Source:

The data set is collected from publicly available UCI Machine Learning repository [(Spam SMS classification - Dataset)](https://archive.ics.uci.edu/ml/datasets/sms+spam+collection).


### Feature Engineering (Text - Preprocessing):

* Remove all non-words
* Transform words into lower case
* Remove stop words
* Perform stemming
* Vectorization = Bag of Words (CountVectorization) & TF-IDF (Term Frequency-Inverse Document Frequency)

### Model: 

* Model Selection: Naive Bayes

* Model Evaluation: Accuracy 97%

### Why The Naive Bayes Model Works So Well

The Naive Bayes model works on the assumption that the features of the dataset are independent of each other — hence called Naive.

This works well for bag-of-words models a.k.a text documents since:

- words in a text document are independent of each other.

- the location of one word doesn’t depend on another word.

Thus satisfying the independence assumption of the Naive Bayes model. Hence, it is most commonly used for text classification, sentiment analysis, spam filtering & recommendation systems.
