# Titanic Classification

Collaborators:
[![](https://img.shields.io/badge/-Pradeep-0e76a8?style=plastic&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/pradeep-vip/)
[![](https://img.shields.io/badge/-Alexandra-0e76a8?style=plastic&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/ai-aksoyoglu/)

This project is based on the Kaggle competition [Titanic - Machine Learning from Disaster](https://www.kaggle.com/c/titanic/data).

## The Challenge

The sinking of the Titanic is one of the most infamous shipwrecks in history.

On April 15, 1912, during her maiden voyage, the widely considered “unsinkable” RMS Titanic sank after colliding with an iceberg. Unfortunately, there weren’t enough lifeboats for everyone onboard, resulting in the death of 1502 out of 2224 passengers and crew.

While there was some element of luck involved in surviving, it seems some groups of people were more likely to survive than others.

In this challenge, we are going to build a predictive model that answers the question: “what sorts of people were more likely to survive?” using passenger data (ie name, age, gender, socio-economic class, etc).

## Local Environment Setup

For this  challenge  we are  going to use python and sklearn ecosystem of tools to build a classification model. In order for us to get started we will need to install anaconda/miniconda on our machine. The reason for using anaconda/minconda is that it allows us to create a fully isolated environment of packages and language version without worrying about package versions. So to get started we are going to follow the below steps.

1. Install miniconda from the official source. The operation specific instructions and installation packages are listed below.

    A. Windows: [Installation Guide](https://docs.conda.io/projects/conda/en/latest/user-guide/install/windows.html)

    B. Linux: [Installation Guide](https://docs.conda.io/projects/conda/en/latest/user-guide/install/linux.html)

    C. Mac: [Installation Guide](https://docs.conda.io/projects/conda/en/latest/user-guide/install/macos.html)

2. Create a conda virtual environment using the ```environment.yml``` environment definition checked into the repository.
    > To create a virtual conda environment using the ```environment.yml``` file present in the root of this directory we need to execute the below command. For detailed instructions about how to manage your conda environment please visit [conda documentation](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#id2)
    ```bash
    conda env create -f environment.yml
    ```

## Project Objectives

Like any project we will start by defining the key outcomes from the each stage/milestone of the project. We can break down the project into 3 milestones.

### EDA

EDA refers to the exploratory data analysis, in this phase we will study the data available to us, review it's quality, perform univariate, bi-variate and multi-variate analysis on the data to study the relationships, variance and skewness in the data. The idea is to analyze the data to prepare for the next stage which is going to be model building.

### Model Building

Because this is an academic project to practice and learn - we will start with the simplest model - Logistic Regression and then expand into other kind of models like decision tress and random forests. Towards the end we will use the same data to build ensemble models using Bagging & Boosting techniques. We will publish the results of various models for comparions to able to make the decision for the next step which is deploying the model to make predictions. We will be selecting the best performing model for the next stage.

### Deployment

The final stage of the project would be to deploy the model and create a website for taking bookings for a fictional Titanic trip, while making the booking for the expedition people would be asked a set of questions - these answers would be then fed into the model to predict whether the passanger making the booking would survive in case the ship met with a disaster 😁.