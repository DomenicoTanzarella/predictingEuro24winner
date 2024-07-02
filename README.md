# predictingEuro24winner [WIP]

## OVERVIEW

The data is related to past performances of Eupean soccer national teams. 

The dataset comes Kaggle ![alt text](https://www.kaggle.com/datasets/piterfm/football-soccer-uefa-euro-1960-2024/code) 
To frame the task, we will refer back to a standard process in industry for data projects called CRISP-DM. This process provides a framework for working through a data problem. A brief overview of CRISP-DM is here.

The notebook is here: [PredictingUEFA24winner.ipynb](https://github.com/DomenicoTanzarella/predictingEuro24winner/blob/main/PredictingUEFA24winner.ipynb)

### Business Understanding

This data represents ...


### Data Understanding

The main featurs are the ones related to the national teams performances over time:

#### Features of interest:


#### Ranking:


#### Players:


## Data Preparation

After our initial exploration and fine tuning of the business understanding, it is time to construct our final dataset prior to modeling. Here, we want to make sure to handle any integrity issues and cleaning, the engineering of new features, any transformations that we believe should happen and general preparation for modeling with sklearn.

In this case we have a series of datasets, so lots of work went into making it consistent for the project.

Below is the pie chart 


### Modeling

The dataset we are analyzing is a typical example of classification problem.

We decide to use the following features for our predictions. 



We perform the following operations to further massage the data:

- We encode non numerical features with OneHotEncoding
- We use StandardScaler to normalize the data (which is very inportant especially for Support Vecto Machine models)
- We split the data in train (80%) and test (25%)

After this we compare for different classifier and we decide to go with the LogisticRegression()

### Finding

The accuracy for all four tests is poor, with Logistic regression being the best and SVM runner up.

