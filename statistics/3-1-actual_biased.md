[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)



resp = nsfg.ReadFemResp()

#Use the NSFG respondent variable numkdhh to construct the actual distribution for the number of children under 18 in the respondents' households.
pmf = thinkstats2.Pmf(resp.numkdhh, label='numkdhh')

#actual distribution
thinkplot.Pmf(pmf)
thinkplot.Config(xlabel='Number of children', ylabel='PMF')

#Now compute the biased distribution we would see if we surveyed the children and asked them how many children under 18 (including themselves) are in their household.
def BiasPmf(pmf, label):
    new_pmf = pmf.Copy(label=label)

    for x, p in pmf.Items():
        new_pmf.Mult(x, x)
        
    new_pmf.Normalize()
    return new_pmf
    
biased = BiasPmf(pmf, label='biased')

#biased distribution
thinkplot.PrePlot(2)
thinkplot.Pmfs([pmf, biased])
thinkplot.Config(xlabel='Number of children', ylabel='PMF')

