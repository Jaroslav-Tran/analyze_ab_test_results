# analyze_ab_test_results
Udacity Data Analyst Nanodegree AB testing project

## SUMMARY
In this project I investigate an e-commerce company AB testing results dataset. The goal of the project is to determine whether the new version of the webpage is better than the old one. 

## INTRODUCTION:
This dataset collects information from over 290K users of the website divided into a control(old page) and treatment group (new page) with 5 associated variables (characteristics). It is focused on the question of whether or not the new page perform better than the old one. A number of characteristics about the user are included in each row:
1) user_id: Identification of a user
3) timestamp: a time frame when the website was used
4) group: whether the user was in the control or treatment group
5) landing_page: whether the user was exposed to the old landing page or a new landing page
6) converted: 0 or 1 depending on whether the user converted

## QUESTIONS INVESTIGATED:
I used data analysis proccess to explore a data set answer questions we were interested on:
<ul>
  <li> Q1: Does the new landing page lead to better conversion rate than the old landing page? </li>
  <li> Q2: Does the country of the user (where the transaction was made-USA,UK,CA) affect the conversion rate? </li>
</ul>

## PROCESS OUTLINE:
The AB testing was conducted from multiple angles:
<ol>
  <li> -Determine conversion probabilities for treatment and control group and observe the difference </li>
  <li> -Setup a null and alternative hypothesis </li>
  <li> -Simulate differences between treatment and control group under null hypothesis (p_diffs) </li>
  <li> -Observe the p value - whether proportion of the p_diffs are greater than the actual difference observed in point #1 </li>
  <li> -Reject/Accept null hypothesis </li>
  <li> -Using Regression approach to arrive at the same conclusion in the points 1-5 </li>
 </ol>
 
## KEY TAKEAWAYS
None of the variables have significant p-values. We will fail to reject the null and conclude that there is not sufficient evidence that would suggest that there is an interaction between country and page received that will predict whether a user converts or not.

Overall conclusion is that there is not a sufficient proof suggesting that the new page leads to a better conversion rate than the old page.

You can access the interactive version on my binder <a href ="https://mybinder.org/v2/gh/Jaroslav-Tran/investigate-doc-appointments/master"> here.</a>

