# Titanic Classification

Collaborators:
[![](https://img.shields.io/badge/-Pradeep-0e76a8?style=plastic&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/pradeep-vip/)
[![](https://img.shields.io/badge/-Alexandra-0e76a8?style=plastic&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/ai-aksoyoglu/)

This project is based on the Kaggle competition [Titanic - Machine Learning from Disaster](https://www.kaggle.com/c/titanic/data).



## Context

The sinking of the Titanic is one of the most infamous shipwrecks in history.

On April 15, 1912, during her maiden voyage, the widely considered “unsinkable” RMS Titanic sank after colliding with an iceberg. Unfortunately, there weren’t enough lifeboats for everyone on board, resulting in the death of 1502 out of 2224 passengers and crew.

While there was some element of luck involved in surviving, it seems some groups of people were more likely to survive than others.

In this challenge, we are going to build a predictive model that answers the question:  “which passengers were more likely to survive?” based on passenger data such as name, age, gender, socio-economic class, etc.



## Local Environment Setup

To build a classification model for this  challenge we used Scikit-learn (aka sklearn), which is a machine learning library in Python. 

To create a fully isolated environment for the packages and language version used, we install anaconda/miniconda on our local machine. If you want to code along, please follow these steps:

1. Install miniconda from the official source. The operation specific instructions and installation packages are listed below.

    A. Windows: [Installation Guide](https://docs.conda.io/projects/conda/en/latest/user-guide/install/windows.html)

    B. Linux: [Installation Guide](https://docs.conda.io/projects/conda/en/latest/user-guide/install/linux.html)

    C. Mac: [Installation Guide](https://docs.conda.io/projects/conda/en/latest/user-guide/install/macos.html)

2. Create a conda virtual environment using the ```environment.yml``` environment definition checked into the repository.
    > To create a virtual conda environment using the ```environment.yml``` file present in the root of this directory we need to execute the below command. For detailed instructions about how to manage your conda environment please visit [conda documentation](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#id2)
    ```bash
    $ conda env create -f environment.yml
    ```
    
3. To activate this environment:

    ```bash
    $ conda activate titanic-classification
    ```

4. To deactivate an active environment:

    ```bash
    $ conda deactivate
    ```

    

## Project Goal

The goal is to predict if a Titanic passenger (from a test data set) survives the trip. To do so, we first build a predictive model based on the training data set. This is supervised machine learning and we will use a classification model to begin with.

We have split the project into three sub-parts:

1. **EDA (Exploratory Data Analysis)**

EDA is the phase in which we study the data available, review it's quality, perform univariate, bi-variate and multi-variate analysis on the data to study the relationships, variance and skewness in the data. The idea is to analyze the data to prepare for the next stage which is going to be model building.

2. **Model Building**

Because this is an academic project to practice and learn - we will start with the simplest model - Logistic Regression and then expand into other kind of models like decision tress and random forests. Towards the end we will use the same data to build ensemble models using Bagging & Boosting techniques. We will publish the results of various models for comparisons to able to make the decision for the next step which is deploying the model to make predictions. We will be selecting the best performing model for the next stage.

3. **Deployment**

The final stage of the project would be to deploy the model and create a website for taking bookings for a fictional Titanic trip, while making the booking for the expedition people would be asked a set of questions - these answers would be then fed into the model to predict whether the passanger making the booking would survive in case the ship met with a disaster 😁.