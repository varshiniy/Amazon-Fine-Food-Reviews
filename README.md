# Amazon-Fine-Food-Reviews

#### Performed Exploratory Data Analysis, Data Cleaning, Data Visualization and Text Featurization(BOW, tfidf, Word2Vec).Build ML models like KNN, Naive Bayes<br>
### Objective:
Given a text review, determine the sentiment of the review whether its positive or negative.
<br>Data Source: https://www.kaggle.com/snap/amazon-fine-food-reviews <br>
<br>About Dataset<br>
The Amazon Fine Food Reviews dataset consists of reviews of fine foods from Amazon.<br>

Number of reviews: 568,454<br>
Number of users: 256,059<br>
Number of products: 74,258<br>
Timespan: Oct 1999 - Oct 2012<br>
Number of Attributes/Columns in data: 10 

Attribute Information:
1. Id
2. ProductId - unique identifier for the product
3. UserId - unqiue identifier for the user
4. ProfileName
5. HelpfulnessNumerator - number of users who found the review helpful
6. HelpfulnessDenominator - number of users who indicated whether they found the review helpful or not
7. Score - rating between 1 and 5
8. Time - timestamp for the review
9. Summary - brief summary of the review
10. Text - text of the review

### 1. Amazon Food Reviews EDA, NLP, Text Preprocessing and Visualization using TSNE
 1. Defined Problem Statement
 2. Performed Exploratory Data Analysis(EDA) on Amazon Fine Food Reviews Dataset plotted  Pairplots, Histograms, etc.
 3. Performed Data Cleaning & Data Preprocessing by removing unneccesary and duplicates rows and for text reviews removed html tags,           punctuations, Stopwords and Stemmed the words using Porter Stemmer
 4. Documented the concepts clearly
 5. Plotted TSNE plots for Different Featurization of Data viz. BOW(uni-gram), tfidf, Avg-Word2Vec and tf-idf-Word2Vec

### 2. KNN
 1. Applied K-Nearest Neighbour on Different Featurization of Data viz. BOW(uni-gram), tfidf, Avg-Word2Vec and tf-idf-Word2Vec
 2. Used both brute & kd-tree implementation of KNN
 3. Evaluated the test data on various performance metrics like accuracy also plotted Confusion matrix
 #### Conclusions:
 1. KNN is a very slow Algorithm takes very long time to train.
 2. Best Accuracy is achieved by TF-IDF Featurization which is of 91.9% 
 3. Both kd-tree and brute algorithms of KNN gives comparatively similar results.
 4. Overall KNN was not that good for this dataset.
 
 ### 3. Naive Bayes
 1. Applied Naive Bayes using  Multinomial NB on Different Featurization of Data viz. BOW(uni-gram), tfidf.
 2. Evaluated the test data on various performance metrics like accuracy, f1-score, precision, recall,etc. also plotted Confusion matrix
 3. Printed top 10 Important Features for both Positive and Negative reviews
#### Conclusions:
1. Naive Bayes is much faster algorithm than KNN
2. Best Score is achieved by TF-IDF which is of 95.8%
