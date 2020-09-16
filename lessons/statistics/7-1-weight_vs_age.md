[Think Stats Chapter 7 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2008.html#toc70) (weight vs. age)

>> REPLACE THIS TEXT WITH YOUR RESPONSE
*Using data from the NSFG, make a scatter plot of birth weight versus mother’s age. Plot percentiles of birth weight versus mother’s age. Compute Pearson’s and Spearman’s correlations. How would you characterize the relationship between these variables?*    

ages = live.agepreg  
weights = live.totalwgt_lb    

thinkplot.Scatter(ages, weights, alpha=0.05, s=10)  
thinkplot.Config(xlabel='Maternal age (years)',  
                 ylabel='Birthweight (lbs)',  
                 axis=[10, 45, 0, 15],  
                 legend=False)
