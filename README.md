# Personalized_Medicine_NLP
Classification of genetic variations based on clinical evidence (text)
<br>Data source: https://www.kaggle.com/c/msk-redefining-cancer-treatment/data

# Project Aim:
### Create an algorithm to classify genetic mutations based on clinical evidence (text description) of genetic mutations
Multiclass classification of clinical evidence (text) into 9 classes. However, the criterion by which each class is defined is not provided. In addition to text, `Gene` and `Variation` information of each mutation is also provided, which could be used in combination with text description to classify genetic mutations. 

# Approach:
### Text transformation models:
  CountVectorizer
  TfidfVectorizer
  Truncated singular value decomposition (SVD)
  Word2Vec (self-trained and pre-trained
  Doc2Vec
### Machine learning models:
  LogisticRegression
  RandomForestClassifier
  XGBClassifier
### Deep learning models
  Recurrent neural network (RNN)
  Long short-term memory (LSTM)
  Gated Recurrent Units (GRU)
  Conv1d

<br>This project has 9 sections with code and detailed explanation in 9 jupyter notebooks.

* [Part I: Exploratory data analysis](#PartI_link)
* [Part II: CountVectorizer + Machine Learning models](#PartII_link)
* [Part III: TfidfVectorizer + Machine Learning models](#PartIII_link)
* [Part IV: Latent Semantic Analysis (LSA)](#PartIV_link)
* [Part V: Latent Semantic Analysis (LSA) + `Gene` and `Variation` information](#PartV_link)
* [Part VI: Word2Vec + Machine Learning models](#PartVI_link)
* [Part VII: Doc2Vec + Machine Learning models](#PartVII_link)
* [Part VIII: Deep Learning models with pre-trained Word2Vec](#PartVIII_link)
* [Part IX: Deep Learning models with self-trained Word2Vec](#PartIX_link)

<a id='PartI_link'></a>
## Part I: Exploratory data analysis
### Short overview of the dataset:
  Number of documents in training dataset: 3321
  Number of documents in testing dataset: 5668
  
  After removing documents with NA in `Text` field:
  Number of documents in training dataset: 3316
  Number of documents in testing dataset: 5667

* The training dataset is imbalanced and the number of images in each dataset and in each class is shown as below.
<img src= 'https://github.com/xiey1/Personalized_Medicine_NLP/blob/master/images/class_description.png' width=300px>
