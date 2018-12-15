---
layout: page
title: Motivation
permalink: /Motivation/
---

<p align="center">
  <img src="{{site.url}}{{site.baseurl}}/assets/Google.jpg" width="250" />
  <img src="{{site.url}}{{site.baseurl}}/assets/RStudio.png" width="250" />
</p>

Project is motivated by a kaggle problem  [Google Analytics Customer Revenue Prediction](https://www.kaggle.com/c/ga-customer-revenue-prediction), where google provide huge amount fo raw data from website. You need to find useful information and predict for revenues. 

After viewing the raw data form, we find it's interesting to do a statistical analysis, since the columns contain huge amount of information which makes we able to find other useful relations (not just revenue). Also, nested and nested data with huge amount of raw features are very hard for human to intepret and make decision. Therefore a lot room for statistics.

There're three goals for this project
1.  Find good way to represent the original nested and nested data and clean it to make statistics possible. This is not a typical work you will do in a statistical class since data you use there is typically quite regular and in good shape.
2.  Exploring interesting features which can show the data vividly, help people to understand what the data is exprssing, also help to bulid various of statistical models. And then compare those models
3.  Study the effect of externel data and combine all the knowledge to understand the transaction behavior, which will help us to get the final reasonable model. 

The general question we want to answer is that how to make data powerful? We want to know how to represent the data and how to choose statistical models. But along the project, the questions becomes more practical as "how to represent data if the exact tidy version of it will invovle much unecessary information?" "how to deal with the missing data when the missingness is terrible?" "how to choose model and do statistics in highly ill-conditioned data? can we do sequential modeling?" 

And even encounter some new questions other data itself and models, like "How to ensemble different models and also the externel data?" "how to reduce the features if typical dimension reduction failed because of data being not quite numerical and different entries has even different dimension?"

Only related work is from kaggle website, where we can communicate with each other to deeper our understanding of the question.


