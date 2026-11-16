# ML Projects

## Project overview
This project investigates customer churn using a Netflix customer dataset and aims to develop a machine learning model to predict which customers are likely to cancel their subscription.

The goal is to explore how customer data can help identify customers at risk of churning and support more informed retention strategies and business decisions.

## Project status
Setup in progress.

## Project structure
1. Define business problem and objectives
2. Select and understand dataset
3. Exploratory data analysis
4. Data preparation and feature engineering
5. Model development
    - Establish a baseline model
    - Train and compare candidate models
    - Tune model parameters
6. Model evaluation
    - Evaluate predictive performance
    - Analyse prediction errors
    - Assess business implication
7. Deployment
    - Build and test a prediction API
    - Develop a monitoring approach
Business application and recommendations


## Business problem & Goal

Business context:
The service Netflix provides is a subscription with which customers can stream films & tv shows.
These can be produced by Netflix itself or Netflix bought the distribution rights.
Netflix's main corporate mission is 'to entertain the world'.
Historically, their focus was purely on maximizing active customers.
Given the rapidly increasing competition in the streaming market, their focus has extened to maximizing leisure time for each customer. They have the following goals.

Subgoal A: Maximize active customers
- Get rid of shared subscriptions
- Social media engagement
Subgoal B: Get customers on the most relevant (or most expensive) tier
- Introducing ad-supported tier
Subgoal C: Offer the most relevant films/shows to each customer
- Recommendation engine

Problem statement: 
- Reacquiring a new or churned customer is typically much more expensive than retaining a cutomomer.
- Netflix needs to understand which customers are at risk of cancelling their subscriptions and what factors may contribute to their decision.
When a customer churns it's already too late.

Opportunity:
- Identifying customers at risk of churning before they cancel could create opportunities to investigate and implement targeted retention strategies
- A machine learning model could help Netflix:
    - Identify customers with an elevated probability of churning.
    - Understand which customer characteristics are associated with churn.
    - Provide insights that could inform targeted retention initiatives.

Objectives:
- Develop a classification model to predict whether a customer will churn within the next 30 days
- Identify customer characteristics and behaviours associated with churn
- Evaluate how churn predictions could support customer retention decisions

Limitations/assumptions:
Key assumptions and limitations
- The dataset is representative of the customer population being studied.
- The available features contain information that could help predict churn.
- The dataset contains sufficient information to establish a meaningful 30-day prediction horizon.

## Dataset
- Source: Kaggle
- Dataset: https://www.kaggle.com/datasets/abdulwadood11220/netflix-customer-churn-dataset
- Number of observations: 5000
- Number of features: 14
- Target variable: churned, 50/50 distributed
- Data limitations: Syntetic data


## Decision log
Decision: Use classification
- Reason: Customer either churns or not
Decision: Only keep features ...
- Reason: ...
Decision: Keep feature last login days, but when monitoring, keep an eye out for data leakage
- Reason: strong churn indicator and no clear proof of data leakage