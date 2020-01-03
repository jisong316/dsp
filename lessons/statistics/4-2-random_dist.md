[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

>> 
```{Python}
t = np.random.random(1000)

pmf = thinkstats2.Pmf(t)
thinkplot.Pmf(pmf, linewidth=0.2)
thinkplot.Config(xlabel='Random', ylabel='PMF')

cdf = thinkstats2.Cdf(t)
thinkplot.Cdf(cdf)
thinkplot.Config(xlabel='Random', ylabel='CDF')

# The distribution of CDF is almost uniform.

```
