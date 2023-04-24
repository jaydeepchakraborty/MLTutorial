Overview

Clarify Requirements
How the ML system fits into the overal product backend
Data Related Activites
Model Related Activities
Scaling
Details

Clarify Requirements
What is the goal? Any secondary goal?
e.g. for CTR - maximizing the number of clicks is the primary goal. A secondary goal might be the quality of the ads/content
Ask questions about the scale of the system - how many users, how much content?
How the ML system fits into the overall product backend
Think/draw a very simple diagram with input/output line between system backend and ML system
Data Related Activites
Data Explore - whats the dataset looks like?
Understand different features and their relationship with the target
        - Is the data balanced? If not do you need oversampling/undersampling?
        - Is there a missing value (not an issue for tree-based models)
        - Is there an unexpected value for one/more data columns? How do you know if its a typo etc. and decide to ignore?
Feature Importance - partial dependency plot, SHAP values, dataschool video (reference)
(ML Pipeline: Data Ingestion) Think of Data ingestion services/storage
(ML Pipeline: Data Preparation) Feature Engineering - encoding categorical features, embedding generation etc.
(ML Pipeline - Data Segregation) Data split - train set, validation set, test set
Model Related Activities
(ML Pipeline - Model Train and Evaluation) Build a simple model (XGBoost or NN)
        - How to select a model? Assuming its a Neural Network
            1. NLP/Sequence Model
                - start: LSTM with 2 hidden layers
                - see if 3 layers help,
                - improve: check if Attention based model can help
            2. Image Models - (Don't care right now)
            3. Other
                - start: Fully connected NN with 2 hidden layers
                - Improve: problem specific
(ML Pipeline - Model Train and Evaluation) What are the different hyperparameters (HPO) in the model that you chose and why?
(ML Pipeline - Model Train and Evaluation) Once the simple model is built, do a bias-variance tradeoff, it will give you an idea of overfitting vs underfitting and based on whether overfit or underfit, you need different approaches to make you model better.
Draw the ML pipeline (reference #3)
Model Debug (reference #1)
Model Deployment (reference#3)
(ML Pipeline: Performance Monitoring) Metrics
AUC, F1, MSE, Accuracy, NDCG for ranking problems etc.
When to use which metrics?
Scaling



https://leetcode.com/discuss/interview-question/system-design/566057/Machine-Learning-System-Design-%3A-A-framework-for-the-interview-day