# Fake-news

## Capstone Project for Flatiron School of Data Science 

## Dataset Information
The dataset used can ce found here: https://www.uvic.ca/engineering/ece/isot/datasets/fake-news/index.php

### Dataset Info
"ISOT Fake News Dataset The ISOT Fake News dataset is a compilation of several thousands fake news and truthful articles, obtained from different legitimate news sites and sites flagged as unreliable by Politifact.com. The dataset for this analysis can be found here

The dataset contains two types of articles fake and real News. This dataset was collected from realworld sources; the truthful articles were obtained by crawling articles from Reuters.com (News website). As for the fake news articles, they were collected from different sources. The fake news articles were collected from unreliable websites that were flagged by Politifact (a fact-checking organization in the USA) and Wikipedia. The dataset contains different types of articles on different topics, however, the majority of articles focus on political and World news topics. The dataset consists of two CSV files. The first file named “True.csv” contains more than 12,600 articles from reuter.com. The second file named “Fake.csv” contains more than 12,600 articles from different fake news outlet resources. Each article contains the following information: article title, text, type and the date the article was published on. We focused mostly on collecting articles from 2016 to 2017. The data collected were cleaned and processed, however, the punctuations and mistakes that existed in the fake news were kept in the text. The following table gives a breakdown of the categories and number of articles per category.

Thre are 21417 articles in the Real_news dataset: 10145 articles are from World_News category"

Ahmed H, Traore I, Saad S. “Detecting opinion spams and fake news using text classification”, Journal of Security and Privacy, Volume 1, Issue 1, Wiley, January/February 2018.
Ahmed H, Traore I, Saad S. (2017) “Detection of Online Fake News Using N-Gram Analysis and Machine Learning Techniques. In: Traore I., Woungang I., Awad A. (eds) Intelligent, Secure, and Dependable Systems in Distributed and Cloud Environments. ISDDC 2017. Lecture Notes in Computer Science, vol 10618. Springer, Cham (pp. 127- 138).


 ### Requirements

There are some general library requirements for the project and some which are specific to individual methods. The general requirements are as follows.  
* `numpy`
* `scikit-learn`
* `scipy`
* `nltk`

The library requirements specific to some methods are:
* `keras` with `TensorFlow` 
* `xgboost` 
* `LogisticRegression`
* `RandomForestClassifier`
* `KNeighborsClassifier`
* `Support Vector Machine`
* `AdaBoost
* `Gradient Boosting`


**Note**: It is recommended to use Anaconda distribution of Python.


### Analysis and Preprocessing 

1. Run `Scarpping_the_guardian.ipynb`  This will scrape The Guardian news paper website for all the articles for 2019. In order to do that you need an Api key. You can find more info on the process here:  https://open-platform.theguardian.com/documentation/.
I only selected the Word News and Political News to create the aproximate 3000 articles for the test datase.

2. Run `dataset_analysis.ipynb` , this will download the 2 datasets used for training models. Use WordCloud to examine the words in the texts of the articles.

3. Run `models.ipynb` to: Tokenize data, 
                         Instantiate models,
                         Chose the best performing model,
                         Create a Pipeline,
                         Test the best performing model on the scrapped dataset from The Guardian.
                         
   Models used: * `xgboost` 
                * `LogisticRegression`
                * `RandomForestClassifier`
                * `KNeighborsClassifier`
                * `Support Vector Machine`
                * `AdaBoost
                * `Gradient Boosting`
                
4. Run `Keras model.ipynb` to create, train and test a deep learning Keras model.

5. `Fake.csv.zip`, and `True.csv.zip` are the 2 datasets downloaded from University of Victoria.

6. `the_guardian_file.csv` is the dataset obtained when we scrapped The Guardian website.
                

