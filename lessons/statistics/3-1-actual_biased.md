[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

*Actual distribution for the number of children under 18 in the respondents' households:*  

	pmf = thinkstats2.Pmf(resp.numkdhh, label='actual')     

*Biased distribution for the number of children under 18 in the respondents' households:*  

	biased_pmf = BiasPmf(pmf, label='observed')
	thinkplot.PrePlot(2)
	thinkplot.Pmfs([pmf, biased_pmf])
	thinkplot.Config(xlabel='Number of children under 18', ylabel='PMF')

*Compute means of actual and observed/biased distributions:*  

	print('Actual mean:', pmf.Mean())
	print('Observed mean:', biased_pmf.Mean())
