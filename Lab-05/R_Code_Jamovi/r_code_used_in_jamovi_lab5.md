r_code_used_in_jamovi_lab5
================
Siddhartha Chilukuri
2025-07-15

# R-code for calculating the mean and SD of a discrete random variable

``` r
# Defining the values of the random variable (x) and their probabilities (P(x)) 
x <- c(0, 1, 2, 3, 4, 5, 6) 
p_x <- c(0.20, 0.15, 0.10, 0.25, 0.05, 0.10, 0.15) 
# Calculating the mean (expected value) using the formula: mu = sum(x * P(x)) 
mean_x <- sum(x*p_x) 
# Calculating the standard deviation using the formula: SD = sqrt(sum((x - mu)^2 * P(x))) 
sd_x <- sqrt(sum(((x - mean_x)^2) * p_x)) 
# Printing the calculated values in the Results panel 
# function cat() acts similar to function print(). See Appendix for more information. 

cat("Mean (mu):", mean_x, "\n") 
```

    ## Mean (mu): 2.7

``` r
cat("Standard Deviation (sigma):", sd_x, "\n") 
```

    ## Standard Deviation (sigma): 2.051828

# R-Code Block for simulating the random binomial experiment

``` r
# Setting a seed for the reproductivity of output 
set.seed(1442) 
# Binomial simulation inputs 
n_obs <- 10000    # simulation number 
size <-5        # n  
prob <- 0.65    # p
# Next, we simulate the binomial data for 10,000 iterations using the rbinom() function. 
# rbinom() stands for " random binomial distribution," which generates a binomial simulation. 
binom_sim <- rbinom(n = n_obs, size = size, prob = prob) 
print(head(binom_sim, 100))    # prints first 100 simulations 
```

    ##   [1] 5 3 3 4 3 2 3 3 3 4 4 4 1 4 5 1 3 5 3 3 3 3 4 4 3 4 2 3 2 3 4 4 3 4 2 1 3
    ##  [38] 4 4 2 1 5 4 5 3 4 2 3 5 4 4 2 3 3 3 4 4 3 3 4 5 4 4 5 5 4 5 5 4 5 2 3 1 4
    ##  [75] 2 4 3 4 0 5 3 4 4 3 1 4 4 3 3 3 5 3 4 2 0 4 4 3 4 4

``` r
# Simulation summary table 
summary_table <- table(binom_sim) 
print(summary_table)
```

    ## binom_sim
    ##    0    1    2    3    4    5 
    ##   48  482 1774 3287 3195 1214
