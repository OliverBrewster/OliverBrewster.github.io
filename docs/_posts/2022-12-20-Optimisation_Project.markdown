---
layout: post
title:  "Algorithms for Regression and Binary Classification"
date:   2022-12-20 09:32:26 +0000
categories: Engineering Projects
---
<!-- # RoboChess Project -->

### Project Summary:
This was a university project undertaken to understand and implement many foundational algorithms that form the basis for machine learning. It involved a toy problem, with a function to generate 'messy' 2D data points about two nodes with Gaussian noise added. 

The initial (and simpler) problem was a linear regression task used to generate parameters for a linear transformation of (x1, x2) to an output parameter y. This was solved analytically by optimising the mean squared error of the parameter space (θ1, θ2). This was subsequently solved more computationally efficiently using gradient descent.

The second problem was to classify each data point by the node which it was generated from. The following algorithms were used to solve the classification problem:
- Gradient descent with logistic regression
- Stochastic gradient descent with logistic regression
- Support Vector Machine (SVM) with linear programming

The results between algorithms agreed to within a very small margin, with logistic regression using stochastic gradient descent being the most computationally efficient algorithm under my implementation. This exercise was useful for understanding the process of tuning hyper-parameters and understanding the risk of overfitting when the tuning parameter space was too large.

The following shows how classification error changes for different batch sizes with stochastic gradient descent and a visual proof of the algorithm's success!

<div style="display: grid; grid-template-columns: 0.7fr 0.3fr;">
  <img src="/assets/B1/ClassifErrorAll.jpg" alt="Classification error SGD" style="max-width: 100;">
  <img src="/assets/B1/DecisionLine.jpg" alt="Decision line produced" style="max-width: 100%;">
</div>