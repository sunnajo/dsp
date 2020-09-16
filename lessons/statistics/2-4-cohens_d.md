[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

*Compute Cohen’s effect size to quantify the difference between the groups. How does it compare to the difference in pregnancy length?*  
	
	firsts.totalwgt_lb.mean(), others.totalwgt_lb.mean()  
(7.201094430437772, 7.325855614973262)    

	CohenEffectSize(firsts.totalwgt_lb, others.totalwgt_lb)  
-0.088672927072602    

The pregnancy length for first babies appears to be longer than that for other babies, whereas the birthweight of first babies seems to be lower than that for other babies.
