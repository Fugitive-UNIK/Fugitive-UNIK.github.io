---
layout: archive
title: "Project Experiences / 项目经历"
permalink: /Project/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

A SQL-Based Hybrid Database-Driven Framework for Customer Satisfaction Prediction with Machine Learning and Natural Language Processing -Enhanced Sentiment Analysis
------
* Using SQL, reverse engineering and reengineering were conducted on 8 core tables of the e-commerce database. An ER diagram was designed and the data of orders, payments, logistics and comments were integrated to build a unified analysis view. Missing value processing, abnormal order elimination and feature derivation based on business logic (such as freight efficiency ratio and product volume) were completed to construct a high-quality modeling dataset
* A prediction pipeline was built and three models, Ridge Regression, RF and XGBoost, were compared. Feature importance analysis and screening were carried out through SHAP values and mutual information method, and the Random Forest model performed the best, accurately quantifying the nonlinear impact mechanism of logistics timeliness and payment amount on user ratings
* A complete NLP process was implemented, including Portuguese text cleaning (noise removal, stem extraction), stop word filtering and TF-IDF vectorization. MultinomialNB, Logistic Regression and RF were compared, and Logistic Regression was finally selected for deployment because it maintained a high accuracy rate (89.28%) while having excellent model interpretability
* Combining the RFM model and EDA analysis, the risks of low user retention rate, uneven regional development and excessive reliance on credit card payments on the platform were revealed. Data-driven operation strategies such as "delayed compensation for high-value orders", "control of freight ratio threshold" and "awakening of dormant users" were proposed to guide business to optimize user experience

电商用户满意度预测与运营策略分析
------
* 使用SQL对电子商务数据库的8个核心表进行了逆向工程和重构，设计了实体关系图（ER图），并将订单、支付、物流和评论数据整合，构建统一的分析视图。完成了缺失值处理、异常订单剔除以及基于业务逻辑的特征衍生（如货运效率比和产品销量），从而构建出高质量的建模数据集  
* 构建了预测流水线，并对岭回归（Ridge Regression）、随机森林（RF）和XGBoost三种模型进行了比较。通过SHAP值和互信息方法对特征重要性进行分析与筛选，结果表明随机森林模型表现最优，能够准确量化物流时效性和付款金额对用户评分的非线性影响机制。 
* 实现了完整的自然语言处理流程，包括葡萄牙语文本清洗（去除噪声、提取词干）、停用词过滤以及TF-IDF向量化处理。对多项式朴素贝叶斯、逻辑回归和随机森林进行了比较，最终选择逻辑回归进行部署，因为它在保持高准确率（89.28%）的同时，模型可解释性也十分出色。 
* 结合RFM模型与数据探索分析，揭示了平台用户留存率低、区域发展不均衡以及过度依赖信用卡支付等风险。提出了“高价值订单延迟补偿”“控制货运比例阈值”“唤醒沉睡用户”等数据驱动的运营策略，以指导业务优化用户体验

Horse Racing Prediction Based on PPCA and GLMM
------
* We cleaned and reconstructed the original 53-dimensional features, implementing a track-specific partitioning strategy (HV/AVT/ST) to eliminate venue heterogeneity. We designed a dynamic normalization algorithm based on in-track race data, ensuring the input data for the model is independently and identically distributed while preserving horses' relative competitive states, thereby preventing data leakage risks
* To address the cold-start challenge caused by complete absence of historical features for new horses, we employed a probabilistic generative framework using PPCA (Probabilistic Principal Component Analysis), leveraging the EM algorithm to infer high-dimensional latent variables from known information (e.g., jockey, starting position), enabling unbiased dimensionality reduction. Given the evident nested structure of horse racing data, we constructed a GLMM (Generalized Linear Mixed Model) to separate systematic biases arising from weather or track conditions on specific race days from the horses’ intrinsic performance levels, resolving the violation of residual independence assumptions in traditional regression models and providing robust decision support for predicting race winners

赛马预测：基于PPCA与GLM的冷启动与嵌套结构建模
------
* 对原始53维特征的清洗与重构，实施赛道特异性分区策略（HV/AVT/ST）以消除场地异质性；设计基于同场赛事的动态归一化算法，在保留马匹相对竞技状态的同时，确保模型输入数据的独立同分布特性，阻断数据泄露风险
* 针对新马历史特征全缺失的冷启动难题，利用PPCA（概率主成分分析）的概率生成框架，通过EM算法基于已知信息（如骑师、档位）推断高维潜变量，实现无偏降维；根据赛马数据具有明显的嵌套结构，通过构建GLMM模型，分离由特定比赛日天气或场地带来的系统性偏差与马匹自身的竞技状态，解决传统回归模型中残差独立性假设被违反的问题，为赛马冠军预测提供稳健的决策依据
