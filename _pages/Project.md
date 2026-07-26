---
layout: archive
title: "Project Experience"
permalink: /Project/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

A SQL-Based Hybrid Database-Driven Framework for Customer Satisfaction Prediction with Machine Learning and Natural Language Processing -Enhanced Sentiment Analysis
------
* Using SQL, reverse engineering and reengineering were conducted on 8 core tables of the e-commerce database. An ER diagram was designed and the data of orders, payments, logistics and comments were integrated to build a unified analysis view. Missing value processing, abnormal order elimination and feature derivation based on business logic (such as freight efficiency ratio and product volume) were completed to construct a high-quality modeling dataset.
* A prediction pipeline was built and three models, Ridge Regression, RF and XGBoost, were compared. Feature importance analysis and screening were carried out through SHAP values and mutual information method, and the Random Forest model performed the best, accurately quantifying the nonlinear impact mechanism of logistics timeliness and payment amount on user ratings
* A complete NLP process was implemented, including Portuguese text cleaning (noise removal, stem extraction), stop word filtering and TF-IDF vectorization. MultinomialNB, Logistic Regression and RF were compared, and Logistic Regression was finally selected for deployment because it maintained a high accuracy rate (89.28%) while having excellent model interpretability
* Combining the RFM model and EDA analysis, the risks of low user retention rate, uneven regional development and excessive reliance on credit card payments on the platform were revealed. Data-driven operation strategies such as "delayed compensation for high-value orders", "control of freight ratio threshold" and "awakening of dormant users" were proposed to guide business to optimize user experience

Horse Racing Prediction Based on PPCA and GLM
------
* We cleaned and reconstructed the original 53-dimensional features, implementing a track-specific partitioning strategy (HV/AVT/ST) to eliminate venue heterogeneity. We designed a dynamic normalization algorithm based on in-track race data, ensuring the input data for the model is independently and identically distributed while preserving horses' relative competitive states, thereby preventing data leakage risks

* To address the cold-start challenge caused by complete absence of historical features for new horses, we employed a probabilistic generative framework using PPCA (Probabilistic Principal Component Analysis), leveraging the EM algorithm to infer high-dimensional latent variables from known information (e.g., jockey, starting position), enabling unbiased dimensionality reduction. Given the evident nested structure of horse racing data, we constructed a GLMM (Generalized Linear Mixed Model) to separate systematic biases arising from weather or track conditions on specific race days from the horses’ intrinsic performance levels, resolving the violation of residual independence assumptions in traditional regression models and providing robust decision support for predicting race winners
