---
layout: post
title: Resampling Methods
---

- [2014-10-06-bootstrap]({{ site.url }}/assets/papers/2014-10-06-bootstrap.pdf)
    - A very layman's guide to resampling, written for business students
- Resampling is a modern approach to calculating variances/confidence intervals of specific statistics and significance tests

## Bootstrap

- Which bootstrap when [http://www.stat.cmu.edu/~cshalizi/uADA/13/lectures/which-bootstrap-when.pdf](http://www.stat.cmu.edu/~cshalizi/uADA/13/lectures/which-bootstrap-when.pdf)

- Bootstrap is superior to Jackknife [ref](http://stats.stackexchange.com/questions/21023/bootstrap-vs-jackknife)
- Bootstrap standard error: the standard deviation of the bootstrap distribution
- Bootstrap estimate of bias: the mean of the bootstrap distribution minus the statistic of original data.
- bootstrap t confidence interval: only if bootstrap distribution is unbiased and normal. Std deviation of Bootstrap distribution. Gives confidence interval.
- Using 1000 or more resamples introduces little additional variation (business book) The resampling process introduces little variation.
- Bootstrap bias-corrected accelerated (BCa) and bootstrap tilting: improve accuracy faster with more data. "Should always use instead of simply taking standard deviation of bootstrap distribution." It tries to counteract the bias and skewness of the data.

## Permutation Test

- Resampling in a manner consistent with the null hypothesis. Resample so that the hypothesis isn't true.
- Advantage over t-test: doesn't assume normal distribution over x1 - x2
- Assumption: two populations have identical distributions when the null hypothesis is true

## Statistics/Parameters

- mean
- variance
- trimmed mean (25% trimmed mean is the mean of the middle 50% of the observations)


