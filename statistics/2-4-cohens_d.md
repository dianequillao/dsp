[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

# Exercise 2.4 Using the variable totalwgt_lb, investigate whether first babies
# are lighter or heavier than others. Compute Cohen’s d to quantify the
# difference between the groups. How does it compare to the difference in pregnancy length?

def CohenEffectSize(group1, group2):
    diff = group1.mean() - group2.mean()

    var1 = group1.var()
    var2 = group2.var()
    n1, n2 = len(group1), len(group2)

    pooled_var = (n1 * var1 + n2 * var2) / (n1 + n2)
    d = diff / np.sqrt(pooled_var)
    return d
    
    
CohenEffectSize(firsts.totalwgt_lb, others.totalwgt_lb) 

#The effect size is small. A first baby doesn't necessarily mean it will be heavier or lighter than others.
