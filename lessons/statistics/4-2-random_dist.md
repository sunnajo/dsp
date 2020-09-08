[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

sample = np.random.random(1000)
sample_pmf = thinkstats2.Pmf(sample, label='pmf')
thinkplot.Hist(sample_pmf)
thinkplot.Config(xlabel='Number', ylabel='PMF')

sample_cdf = thinkstats2.Cdf(sample, label='cdf')
thinkplot.Cdf(sample_cdf)
thinkplot.Config(xlabel='Number', ylabel='CDF', loc='upper left')

The distribution is uniform.
