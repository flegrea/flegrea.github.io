---
title: "A Strategy for Predicting the Performance of Supervised and Unsupervised Tabular Data Classifiers"
pubvenue: Data Science and Engineering
authors: T. Zoppi, A. Ceccarelli, A. Bondavalli
link: https://doi.org/10.1007/s41019-024-00264-9
arxiv: 
date: September 2024
dataset: "Feature RAnkers to Predict classification PerformancE of binary classifiers"
tags: ids
---
Machine Learning algorithms that perform classification are increasingly been adopted in Information and Communication Technology (ICT) systems and infrastructures due to their capability to profile their expected behavior and detect anomalies due to ongoing errors or intrusions. Deploying a classifier for a given system requires conducting comparison and sensitivity analyses that are time-consuming, require domain expertise, and may even not achieve satisfactory classification performance, resulting in a waste of money and time for practitioners and stakeholders. This paper predicts the expected performance of classifiers without needing to select, craft, exercise, or compare them, requiring minimal expertise and machinery. Should classification performance be predicted worse than expectations, the users could focus on improving data quality and monitoring systems instead of wasting time in exercising classifiers, saving key time and money. The prediction strategy uses scores of feature rankers, which are processed by regressors to predict metrics such as Matthews Correlation Coefficient (MCC) and Area Under ROC-Curve (AUC) for quantifying classification performance. We validate our prediction strategy through a massive experimental analysis using up to 12 feature rankers that process features from 23 public datasets, creating additional variants in the process and exercising supervised and unsupervised classifiers. Our findings show that it is possible to predict the value of performance metrics for supervised or unsupervised classifiers with a mean average error (MAE) of residuals lower than 0.1 for many classification tasks. The predictors are publicly available in a Python library whose usage is straightforward and does not require domain-specific skill or expertise.
