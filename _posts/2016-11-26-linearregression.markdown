---
layout: post
title:  "Linear Regression"
date:   2016-11-28 18:05:12 -0400
categories: Javascript
bigimg: /img/linearregression.png
---
Linear Regression is a web [app][linear-regression] inspired by my time working through Andrew Ng's machine learning Coursera [class](https://www.coursera.org/learn/machine-learning). I wanted to help visualize some of the fundamental mathematical concepts that are the building blocks for machine learning and neural networks in a simplified way. The goal is to help users understand what is happening under the hood when hyperparameters, like learning rate and iterations, are set for a model.


This web app is a static HTML and Javascript site that solves and visualizes how linear regression is used to approximate a best fit curve for data on a 2D plot. The user can vary the learning rate (alpha) and observe how the cost converges or diverges based on overshooting, and how the rate of cost reduction varies with learning rate as the cost is plotted against the number of iterations. The numerical representation for the approximation function ( **ϴ** ) and cost ( **[X]\*[ϴ<sup>T</sup>] - [Y]** ) is visible at each iterative step and a sequence of plots can be played to show a continuous visualization of this process. This experience was also an exercise in the struggles of mathematical operations such as matrix multiplication being performed in the single threaded, untyped language that is Javascript.


Check out the [Linear Regression Web App][linear-regression] and give it a try! If you have any feedback feel free to send it my way.

[linear-regression]: http://chrissebesta.com/plain-regression

<!--
 go deeper in to an explanation of linear regression, and how it really relates to machine learning
 give more motivation behing why linear regression matters
 and why its hard to understand, and why this helps solve that
 Talk about learning rate specifically and how this visualized that
 Dynamic learning rates(?)
 -->
