Welcome!
In this section, we will explore several methods to see if certain characteristics or features can be used to predict arrival delay minutes. The main question we will be trying to answer throughout this project is: what are the main characteristics which have the most impact on how long a flight arrives late?

The main question we are trying to answer in this module is: "What causes flight delays?". To get a better measure of the important characteristics, we look at the correlation of these variables with the arrival delay, AKA, "ArrDelayMinutes", in other words: how is the arrival delay minutes dependent on this variable?

First, let's begin with some important definitions:

•	Correlation: a measure of the extent of interdependence between variables.

•	Causation: the relationship between cause and effect between two variables.

It is important to know the difference between these two and that correlation does not imply causation. Determining correlation is much simpler than determining causation as causation may require independent experimentation.

Pearson Correlation

The Pearson Correlation measures the linear dependence between two variables X and Y.

The resulting coefficient is a value between -1 and 1 inclusive, where:

•	1: Total positive linear correlation.

•	0: No linear correlation, the two variables most likely do not affect each other.

•	-1: Total negative linear correlation.

Pearson Correlation is the default method of the function cor(), but other methods can be specified by setting method. Like before we can calculate the Pearson Correlation of the "integer" or "numeric" variables.

P-value:

What is this P-value? The P-value is the probability value that the correlation between these two variables is statistically significant. Normally, we choose a significance level of 0.05, which means that we are 95% confident that the correlation between the variables is significant.

By convention, when the

•	p-value is << 0.001: we say there is strong evidence that the correlation is significant.

•	the p-value is << 0.05: there is moderate evidence that the correlation is significant.

•	the p-value is << 0.1: there is weak evidence that the correlation is significant.

•	the p-value is >> 0.1: there is no evidence that the correlation is significant.

ANOVA: Analysis of Variance

The Analysis of Variance (ANOVA) is a statistical method used to test whether there are significant differences between the means of two or more groups. ANOVA returns two parameters:

•	F-test score: ANOVA assumes the means of all groups are the same, calculates how much the actual means deviate from the assumption, and reports it as the F-test score. A larger score means there is a larger difference between the means.

•	P-value: The p-value tells you how statistically significant the calculated score value is.

If our ArrDelay variable is strongly correlated with the variable we are analyzing, expect ANOVA to return a sizeable F-test score and a small p-value.

