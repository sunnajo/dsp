[Think Stats Chapter 8 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2009.html#toc77) (scoring)

*Suppose you draw a sample with size n=10 from an exponential distribution with λ=2. Simulate this experiment 1000 times and plot the sampling distribution of the estimate L. Compute the standard error of the estimate and the 90% confidence interval.  Repeat the experiment with a few different values of n and make a plot of standard error versus n.*   

	def SimulateSample(lam=2, n=10, iters=1000):

    	estimates = []
    	for _ in range(iters):
        	xs = np.random.exponential(1.0/lam, n)
        	lamhat = 1.0 / np.mean(xs)
        	estimates.append(lamhat)
    
    	# compute standard error
    	stderr = RMSE(estimates, lam)
    	print('standard error:', stderr)
    
    	# compute confidence interval
    	cdf = thinkstats2.Cdf(estimates)
    	ci = cdf.Percentile(5), cdf.Percentile(95)
    	print('confidence interval:', ci)
    
    	# plot the CDF
    	thinkplot.Cdf(cdf)
    	thinkplot.Config(xlabel='estimate',
                     	ylabel='CDF',
                     	title='Sampling distribution')
    	return stderr

	SimulateSample()
