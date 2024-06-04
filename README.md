## Title: Which Variables Are Great at Determining Bankruptcy

----

<br clear="both">

<div align="center">
  <img height="300" width="100%" src="https://github.com/GodfreyElia/Modeling-Crises/blob/main/File/Financial_Crisis.jpg" />
</div>

----

### 1. Background

Predicting corporate bankruptcy is both a science and an art which requires making assumptions that are guided by a deeper understanding of business and corporate economics. As we have seen previously, the models that we adopt to predict business failure play a pivotal role in the quality of our predictions. However, in this project, we extend the research and ask a different question: Do the explanatory variables affect the quality of our predictions? If so, which ones are good explanatory variables and how can we know them? In the next sections of this project, we shall endeavour to precisely answer this question.

### 2. Methodology

To tackle the question of which variables do a great job at determining bankruptcy, we will use two main tools: variable visualisation, and emperical tests.

     2.1. Visualisation.

<br clear="both">

<div align="Left">
  <img height="60%" width="75%" src="https://github.com/GodfreyElia/Best-Bankruptcy-Predictors/blob/main/Stats/Variable-comps.png"  />
</div>
<br>

Fig. 1: Comparison of variables between bankrupt and non-bankrupt firms.

Fig 1 above shows stack differences between bankrupt and non-bankrupt firms. Except for the EBIT:Assets ratio (X3), the differences between bankrupt and live companies is well pronounced in the other variables. However, the most interesting question is whether or not the means are in line with our expectations. For this we get mixed results. For instance, we would expect the operating margin of live companies to be higher than that of companies that went bust, which is the case here. However, we would also expect the current ratio to be high for live companies than dead companies, which unfortunately is not the case.

In conclusion, we can decipher that learning machines only care about if there are differnces within a variable, places more emphasis on the size of the difference than the nature. Based on this and solely on the bar chart, I would argue that operating margin (AM), assets growth rate (AG), Current ratio (Current) and Assets to Sales Ratio (SAR) are the best predictors.


     2.2. Emperical tests

However and perhaps a more realible way of determining which variables are good predictors of bankruptcy is through running emperical tests and quering the models themselves on the importance of features.

<br clear="both">

<div align="Left">
  <img height="60%" width="75%" src="https://github.com/GodfreyElia/Best-Bankruptcy-Predictors/blob/main/Stats/Relative%20Influence.png"  />
</div>
<br>

Fig 2a. Relative Importance of Variables in Models

<br clear="both">

<div align="Left">
  <img height="60%" width="75%" src="https://github.com/GodfreyElia/Best-Bankruptcy-Predictors/blob/main/Stats/Average_importance.png"  />
</div>
<br>

Fig 2b. Average Influence of Variables in Models.

The above charts show the output that I obtained after inquiring of the models what variables they found influencial in predicting bankruptcy. It is quickly apparent that different models ranked the variables differently with age of company, operating margin, and Current ratio being top choices for the random forest, bagging, and boosting models respectively. Fig 2a, takes the averages for the 3 models which we can reliably use to rank the predictors.

    Based on this methodology, we can rank the top 5 predictors (in that order) as: Age of company, Current Ratio, EBIT-Assets Ratio, Sales-Assets Ratio, and the Operating margin.

### 3. Take Away

In this project, I have showed how we can use machine learning to understand which variables affect the likelihood of survival of companies. We have discovered that the age of a company has a large bearing on its chance of survival, corroborating with Fig 1 where we noticed bankrupt companies on average tend to be much younger than their non-bankrupt counterparts. This would be ideal in informing economic policy. Furthermore, other ratios such as the current ratio (measure of liquidity), Ebit- Assets ratio (measure of profitability) are equally very important. Thus it is in the best interest of management to critically manage these ratios.

### 4. Conclusion

In summary, in this project we find that  Age of company, Current Ratio, EBIT-Assets Ratio, Sales-Assets Ratio, and the Operating margin are the five top most important of company failure. Thus, it is left with management to ensure that they are managing effectively the factors that they can control.

----

### Thank you for reading my project.

Click [here](https://github.com/GodfreyElia) to read more projects
