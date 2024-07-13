### Predicting Euro 2024 winner

**Domenico Tanzarella**

#### Executive summary

The goal of this project is to identify and train a model that can predict the outcome of Euro 2024 cup based on historical data

#### Rationale

Machine Learning is at the peak of the hype cycle, but still hard to understand for most people.
Conversely, Soccer is an extremely popular, followed and well understood sport.

Leveraging people interest in this popular sport and the hype of Machine Learning, my goal is to drive more learning into technologies like ML and AI by providing a fun example of ML application in a popular field.

#### Research Question

Can we build a machine learning model to predict the winner of the UEFA Euro 2024 tournament based on historical team and player data? 
Or in general build a predictive model for figuring out UEFA Euro cup winners based on historical data?

#### Data Sources

There are many source of data for players and teams, such as:

  - Kaggle: Dataset "European Football Database" [Kaggle](https://www.kaggle.com/datasets/piterfm/football-soccer-uefa-euro-1960-2024/code) 
  - Kaggle: Dataset Euro 2024 players dataset [Kaggle](https://www.kaggle.com/datasets/damirdizdarevic/uefa-euro-2024-players)
  - Fifa National Team ranking (as at June 10th 2024) [FIFA](https://inside.fifa.com/fifa-world-ranking/men?dateId=id14415)
    
The above listed Datasets will be used for the project

#### Methodology

To frame the task, we will refer back to a standard process in industry for data projects called CRISP-DM. This process provides a framework for working through a data problem. 

This is a classification problem so I expect to:

    - Collect data from above listed data sources

    - Perform Data exploration, data cleaning and aggregation as needed

    - Train KNN, Logistic Regression, Decision Trees and SVM, also train with Neural Networks

    - Once the best model has been found, apply it to the Euro 2024 roster and predict both individual games and final winner.

#### Results
The model with the best accuracy and f1-score will be deployed for the Euro 2024 predictions.

In my case Logistic Regression was the best performing mode, and according to it Spain will win Euro2024, which is a result that matches common sense despite Spain not being ranked the highest in the FIFA ranming system.
  
#### Outline of project

The Notebook can be found here:

[PredictingUEFA24winner.ipynb](https://github.com/DomenicoTanzarella/predictingEuro24winner/blob/main/PredictingUEFA24winner.ipynb)

It is divided in the following sections that can be easily accessed via the Colab Navigation bar on the left frame.

  - Exploratory Data Analysis
  - Feature Engineering
    - Average goal scored
    - Average goal conceded
    - Average game wins
    - Visualizations:
      -  Goal Scored vs Goal Conceded
      -  Percentage wins vs Goal Scored
      -  Heatmap
    - Players data Exploration and feature engineering
    - Final dataset creation
  - Train the Model
  - Predict results (prep work)
    - Group Games Showtime
    - Predictions for the round of 16
    - Predictions for the round of 8
    - Predictions for the semifinals
    - Predictions for the final

    ...and the winner of Euro2024 is...

  Please note that Individual csv files used for the project are in the git repository: in the notebook they are imported from a Google Drive folder, but they can easily be loaded from a computer

##### Contact and Further Information
Domenico Tanzarella
