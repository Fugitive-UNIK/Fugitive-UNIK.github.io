---
layout: archive
title: "Research Experience"
permalink: /research/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

A Theoretical Understanding of Vision Transformers from a Foundation Model Perspective
------
__Abstract__: Since the introduction of Vision Transformer (ViT), it has demonstrated excellent performance in various vision tasks. due to the complex multi-layer interaction mechanism during the training process, its theoretical analysis remains highly challenging. Existing theoretical studies primarily focus on establishing convergence bounds to justify the effectiveness of attention mechanisms. Based on binary classification, we conduct a theoretical investigation of shallow single-head and multi-head ViT. The results show that, for single-head ViT, the sample complexity required to achieve zero generalization error is positively correlated with the inverse proportion of the square of label-relevant tokens, the noise level in tokens, and the initialization error. For multi-head ViT, increasing the number of attention heads reduces the required sample complexity for achieving zero generalization error, particularly in scenarios with sparse informative tokens or high noise levels, and choosing the number of heads consistent with the target task leads to better performance. However, this benefit comes at the cost of the model complexity potentially increasing exponentially as the proportion of relevant labels decreases. In multi-head ViT, the number of iterations is not significantly related to the number of heads, regardless of whether the proportion of relevant labels is high or low. Moreover, appropriately removing irrelevant labels and noisy labels can to some extent improve the model performance. 
__Bullet Point__ <br>
* Conducted a theoretical analysis of shallow single-head and multi-head Vision Transformers (ViTs) based on 
binary classification models. For single-head ViT, revealed that the sample complexity required to achieve zero 
generalization error is inversely proportional to the proportion of the square of relevant labels, and positively 
correlated with label noise level and initialization error. For multi-head ViT, increasing the number of attention 
heads reduces the sample complexity needed for zero generalization error, particularly in scenarios with sparse 
label information or high noise levels, and selecting the number of heads that matches the target task leads to better 
performance. Moreover, appropriately removing irrelevant and noisy labels can enhance model performance to a 
certain extent.
* In simulation experiments, validated the four conclusions for single-head ViT. Additionally, when the proportion 
of relevant labels decreases, the sample complexity for multi-head ViT grows exponentially.

A Comparison Between Gray Models of The Conformable and Caputo Types Using Shock Data
------
__Background__: The gray system's capacity to evaluate with fewer data, inadequate knowledge, and system uncertainty has drawn much attention. As the complexity of the objects being examined increases, the study of fractional order calculus has led to the development of the fractional order gray system, which is widely utilized by academics due to its benefits in managing small sample data and flexible mining. This paper focuses on the gray models of Conformable and Caputo fractional-order calculus and reveals their performance characteristics in various data scenarios by building comparative analyses of periodic gradient oscillatory data. This is because different fractional-order gray models have different applications. <br>
__Bullet Point__ <br>
*  By introducing the fractional accumulation operator defined by Conformable, the coefficient simplification form is derived. Then, the time response is derived based on the constant change method and the CoFGM(r,1) model is established. The example analysis shows that the model can more successfully integrate the information of the current data points and their neighborhoods, has good localization and dynamic responsiveness, which allows the model to quickly identify the data mutations in the iterative process, and has higher accuracy in data fitting and trend prediction for actual changes.
* Through the fractional accumulation operator defined by Caputo, the relationship between the order and the priority of new information is revealed. Then, based on the Laplace transform, the time response function is derived to establish the CaFGM(r,1) model. The model's ability to incorporate global historical data, accurately depict the possible impact of initial data on the trend of change, and exhibit a distinctive long memory—all of which contribute to the model's smoother data fitting and trend prediction curves and its ability to fully capture the overall development trend—is confirmed by the example analysis.
* We systematically analyze the performance of the three types of models, GM(1,1), CoFGM(r,1), and CaFGM(r,1), by building a multi-scale gradient oscillation test dataset (short-term 100%, medium-term 50%, and long-term 25%). The experiments demonstrate that the GM(1,1) model is constrained by equal-weighted accumulation, whichresults in a significant error accumulation effect because of the lack of sensitivity in shock scenarios; the CaFGM(r,1) model satisfies new information prioritization, but its operators' long memory has a lag in response to mutations, so it only retains its advantage in long-term non-stationary data; and the CoFGM(r,1) model only retains its advantage in long-term non-stationary data because the Conformable fractional order gives the data distinct weights, resulting in the synergistic optimization of computational efficiency and local sensitivity, which allows it to function optimally across a variety of algorithms.
*  This study shows the special benefits of the Conformable fractional-order gray model. It offers recommendations for the selection of fractional-order gray models in the cases of locally modified and oscillating data.

A Functional Data Classification Model Utilizing Functional Mahalanobis Distance and Regenerative Kernel Methods
------
__Abstract__: The classification of functional data is an important research direction in modern data mining. In this paper, we propose a similarity measurement method for functional data based on functional Mahalanobis distance and regenerative kernel theory, considering the scenario where the predictor variable is a random function and the response variable is a categorical scalar. This method is then applied to functional kernel principal component analysis. During the classification phase, classic algorithms such as support vector machines and random forests can be combined to accomplish the task of classifying functional data. In empirical analysis, compared to the regenerative kernel based on Euclidean distance and the Euclidean distance regenerative kernel based on B-spline basis functions, the proposed method achieves better classification results. Furthermore, this similarity measurement can also be utilized in other machine learning algorithms based on regenerative kernel theory, thereby developing corresponding analysis methods for functional data. <br>
__Bullet Point__ <br>
* Developed a similarity measurement method for functional data based on functional Mahalanobis distance and regenerative kernel theory and applied it to functional kernel principal component analysis.
*  Discussed the application of this similarity measurement in other machine learning algorithms based on regenerative kernel theory and the development of corresponding analysis methods for functional data.
*  Combined Random Forest to classify functional data and compared its results with Euclidean distance-based reproducing kernel classification and B-spline Euclidean distance-based reproducing kernel classification, achieving an accuracy of 90% with a variance of 0.0009.

A Multivariate Statistical Process Control Model Based on CRITIC Entropy Method and EWMA
------
__Abstract__: Statistical process control is a technique to monitor product or service quality timely that ensure stability. It promotes quality assurance, resource optimization, and is crucial to informed decision-making. Given the diversification of quality indicators, this paper introduces a multivariate EWMA control chart model based on the CRITIC and entropy weighting method. This model allows lack of knowledge of variable distributions and considers variable correlations, which demonstrates strong sensitivity to slight drifts in mean and volatility, even with a non-diagonal covariance matrix. Simulation experiments confirm its ability to identify process changes and their types by manipulating the mean vector and covariance matrix in five controlled experiments. <br>
__Bullet Point__ <br>
* Proposed a new multivariate control chart construction method that applied the CRITIC weighting method for firststage dimensionality reduction and entropy method for second-stage reduction, transforming it into univariate process control and eventually plotting an Exponentially Weighted Moving Average (EWMA) control chart, demonstrating improved sensitivity to small variations in both mean and volatility while accounting for correlations between different indicators.
* Conducted five simulation experiments by manipulating the mean vector and covariance matrix to confirm the model’s ability to identify process changes and their types
