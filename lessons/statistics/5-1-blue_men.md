[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

*Percentage of people between 5'10" and 6'1":*  

Compute the percentage of people who are 5'10" or shorter using the CDF and the percentage of people who are 6'1" or shorter using the CDF, and find the difference between the two values.

	h1 = dist.cdf(177.8) 
	h2 = dist.cdf(185.4)  
	h2-h1
