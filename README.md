Module 5 - Random Variables & Probability Distributions
================

A - "Consider a population consisting of the following values, which represents the number of ice cream purchases during the academic year for each of the five housemates - (8, 14, 16, 10, 11)"

A. Compute the mean of this population.

``` r
icvalues = c(8,14,16,10,11)
icmean = mean(icvalues)
icsd = sd(icvalues)
icsd = round(icsd,4)
```

The mean of this population is 11.8.

B. Select a random sample of size 2 out of the five members.

C. Compute the mean and standard deviation of your sample.

``` r
icsample = sample(icvalues, 2)
icsample
```

    ## [1] 11 14

``` r
icsamplemean = mean(icsample)
icsamplemean
```

    ## [1] 12.5

``` r
icsamplesd = sd(icsample)
icsamplesd = round(icsamplesd,4)
icsamplesd
```

    ## [1] 2.1213

The mean of this sample is 12.5 and the standard deviation is 2.1213.

D. Compare the Mean and Standard deviation of your sample to the entire population of this set (8,14, 16, 10, 11).

The mean and standard deviation of the sample is 12.5 and 2.1213 respectively, while the mean of the original population is 11.8 and the standard deviation is 3.1937.

B. Suppose that the sample size n = 100 and the population proportion p = 0.95.

1.  Does the sample proportion p have approximately a normal distribution? Explain.

``` r
a =5
s = 2
n = 100
error = qnorm(0.950)*s/sqrt(n)
left = a - error
right = a + error
left
```

    ## [1] 4.671029

``` r
right
```

    ## [1] 5.328971

Yes, the sample proportion p has an approximate normal distribution because the sample size and sample proportion are large enough in number. If a large enough proportion of the sample size is included, it is more likely the mean and standard deviation will be close to 0 and 1 respectively. If the error falls within a close range of a, then it it considered normal. In this case, error between 4.5 and 5.5 would be sufficiently called normal.

1.  What is the smallest value of n for which the sampling distribution of p is approximately normal?

``` r
a =5
s = 2
n = 43
error = qnorm(0.950)*s/sqrt(n)
left = a - error
right = a + error
left
```

    ## [1] 4.498324

``` r
right
```

    ## [1] 5.501676

``` r
a =5
s = 2
n = 44
error = qnorm(0.950)*s/sqrt(n)
left = a - error
right = a + error
left
```

    ## [1] 4.504058

``` r
right
```

    ## [1] 5.495942

The smallest number that n can be with a population proportion of .95 and be normally distributed is 44.
