<p>
  <h1 align="center"><b>Web Phishing Detection :female_detective:</h1>
</p>

<p>
  <h2 align="center"> Category: Machine Learning</h2>
</p>

![HookPhish](https://user-images.githubusercontent.com/64459672/199978511-1fb870b3-542d-4928-bba6-f2aa0f4937ee.gif)

## Objective

A phishing website is a common social engineering method that mimics trustful uniform resource locators (URLs) and webpages. The objective of this project is to train machine learning models on the dataset given to predict phishing websites. Both phishing and benign URLs of websites are gathered to form a dataset and from them required URL and website content-based features are extracted. The performance level of each model is measured and compared.

## Data Collection and Analysis

The given [data](https://github.com/IBM-EPBL/IBM-Project-14297-1659548839/blob/main/final%20deliverables/data/dataset_website.csv) contains both phishing and benign URLs of websites with various website content-based features. 

The above mentioned dataset is uploaded to the 'final deliverables/data' folder of this repository.

From data distribution graph and correlation matrix, we can conclude that the 16 of the given features do not have much impact on the result. So they are removed from further processing. The final set of features that are used to build the model are shown in the figure below.

![final_features](https://user-images.githubusercontent.com/64459672/199578614-f8cb7f81-9da0-43a8-b6eb-5381970a9768.png)


## Models & Training

Before stating the ML model training, the data is split into 80-20 i.e., 8844 training samples & 2211 testing samples. From the dataset, it is clear that this is a supervised machine learning task. There are two major types of supervised machine learning problems, called classification and regression.

This data set comes under classification problem, as the input URL is classified as phishing (1) or legitimate (0). The supervised machine learning models (classification) considered to train the dataset in this project are:

- Decision Tree
- Random Forest
- XGBoost
- Support Vector Machines

All these models are trained on the dataset and evaluation of the model is done with the test dataset. The elaborate details of the models & its training are mentioned in [Phishing_Website_Detection.ipynb](https://github.com/IBM-EPBL/IBM-Project-14297-1659548839/blob/main/final%20deliverables/preprocessing%20%26%20model%20building/Phishing_Website_Detection.ipynb).

## End Results

From the obtained results of the above models, XGBoost Classifier has highest model performance of 92.3%. So the model is saved to the file [XGBoostClassifier.pickle.dat](https://github.com/IBM-EPBL/IBM-Project-14297-1659548839/blob/main/final%20deliverables/preprocessing%20%26%20model%20building/XGBoostClassifier.pickle.dat).

## Demo Video:

[HookPhish](https://www.youtube.com/watch?v=0_jsiAmkz64)

## Team Members

- [@Shekinah](https://github.com/sheki018) (Team Lead)
- [@Akshaya](https://github.com/Akxshaya)
- [@Amala](https://github.com/Amala-29)
- [@Annie](https://github.com/ANNIEMARLENENIKITA)

Team ID: PNT2022TMID27489
