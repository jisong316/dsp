[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

>> 
```{python}
import scipy.stats

mu = 178
sigma = 7.7
dist = scipy.stats.norm(loc=mu, scale=sigma)
type(dist)

dist.mean(), dist.std()

dist.cdf(mu-sigma)

n = dist.cdf(177.8)    # 177.8 cm = 5'10"
m = dist.cdf(185.42)   # 185.42 cm = 6'1"
n, m, m-n
```
