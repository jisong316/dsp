[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

>>
```{python}
resp = nsfg.ReadFemResp()

actual_pmf = thinkstats2.Pmf(resp.numkdhh, label='actual')
thinkplot.Pmf(actual_pmf)
thinkplot.Config(xlabel='Number of children', ylabel='PMF')

biased_pmf = BiasPmf(pmf, label='biased')
thinkplot.PrePlot(2)
thinkplot.Pmfs([actual_pmf, biased_pmf])
thinkplot.Config(xlabel='Number of children', ylabel='PMF')

actual_pmf.Mean()

biased_pmf.Mean()
```
