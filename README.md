## Title: Which Variables Are Great at Determining Bankruptcy

----

<br clear="both">

<div align="center">
  <img height="300" width="100%" src="https://github.com/GodfreyElia/Modeling-Crises/blob/main/File/Financial_Crisis.jpg" />
</div>

----

### 1. Background

Predicting corporate bankruptcy is both a science and an art which requires making assumptions that are guided by a deeper understanding of business and corporate economics. As we have seen previously, the models that we adopt to predict business failure play a pivotal role in the quality of our predictions. However, in this project, we extend the research and ask a different question: Do the explanatory variables affect the quality of our predictions? If so, which ones are good explanatory variables and how can we know them? In the next sections of this project, we shall endeavour to precisely answer this question.

### 3. Methodology

To tackle the question of which variables do a great job at determining bankruptcy, we will use two main tools: variable visualisation, and emperical tests.

    #### 3.1. Visualisation.

<br clear="both">

<div align="Left">
  <img height="60%" width="75%" src="https://github.com/GodfreyElia/Best-Bankruptcy-Predictors/blob/main/Stats/Variable-comps.png"  />
</div>
<br>

Fig. 1: Comparison of variables between bankrupt and non-bankrupt firms.

Fig 1 above shows stack differences between bankrupt and non-bankrupt firms. Except for the EBIT:Assets ratio (X3), the differences between bankrupt and live companies is well pronounced in the other variables. However, the most interesting question is whether or not the means are in line with our expectations. For this we get mixed results. For instance, we would expect the operating margin of live companies to be higher than that of companies that went bust, which is the case here. However, we would also expect the current ratio to be high for live companies than dead companies, which unfortunately is not the case.

In conclusion, we can decipher that learning machines only care about if there are differnces within a variable, places more emphasis on the size of the difference than the nature. Based on this and solely on the bar chart, I would argue that operating margin (AM), assets growth rate (AG), Current ratio (Current) and Assets to Sales Ratio (SAR) are the best predictors.


    #### 3.2. Emperical tests

However and perhaps a more realible way of determining which variables are good predictors of bankruptcy is by running emperical tests and quering the models on the importance of features.
