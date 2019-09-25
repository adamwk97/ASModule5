Module 5 - Random Variables & Probability Distributions
================

A - "Consider a population consisting of the following values, which represents the number of ice cream purchases during the academic year for each of the five housemates - (8, 14, 16, 10, 11)"

A. Compute the mean of this population.

``` r
icvalues = c(8,14,16,10,11)
icmean = mean(icvalues)

icsd = sd(icvalues)
```

The mean of this population is 11.8.

B. Select a random sample of size 2 out of the five members.

C. Compute the mean and standard deviation of your sample.

``` r
icsample = sample(icvalues, 2)
icsample
```

    ## [1] 14 16

``` r
icsamplemean = mean(icsample)
icsamplemean
```

    ## [1] 15

``` r
icsamplesd = sd(icsample)
icsamplesd
```

    ## [1] 1.414214

The mean of this sample is 15 and the standard deviation is 1.4142136.

D. Compare the Mean and Standard deviation of your sample to the entire population of this set (8,14, 16, 10, 11).

The mean and standard deviation of the sample is 15 and 1.4142136 respectively, while the mean of the original population is 11.8 and the standard deviation is 3.1937439.
