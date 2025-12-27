R_Code_Used_in_Jamovi_Lab4
================
Siddhartha Chilukuri
2025-06-27

## R code to simulate a dice roll 1000 times

``` r
# R code to simulate a dice roll 1000 times


# Loading the dplyr library for data manipulation 
library(dplyr) 
```

    ## Warning: package 'dplyr' was built under R version 4.4.3

    ## 
    ## Attaching package: 'dplyr'

    ## The following objects are masked from 'package:stats':
    ## 
    ##     filter, lag

    ## The following objects are masked from 'package:base':
    ## 
    ##     intersect, setdiff, setequal, union

``` r
# Setting a seed to make the results reproducible 
set.seed(1442) 
# Simulating a fair six-sided die roll for 1000 rolls 
dice_roll <- function(n) {sample(1:6, size = n, replace = TRUE)} 
sim_1000 <- data.frame(Roll = dice_roll(1000)) 
print(head(sim_1000, 20))   # prints first 20 rows. 
```

    ##    Roll
    ## 1     3
    ## 2     4
    ## 3     4
    ## 4     6
    ## 5     2
    ## 6     1
    ## 7     2
    ## 8     6
    ## 9     1
    ## 10    1
    ## 11    4
    ## 12    4
    ## 13    6
    ## 14    3
    ## 15    6
    ## 16    3
    ## 17    3
    ## 18    1
    ## 19    1
    ## 20    6

``` r
# Simulation summary table 
summary_1000 <- table(sim_1000) 
print(summary_1000) 
```

    ## Roll
    ##   1   2   3   4   5   6 
    ## 178 163 174 164 149 172

## R-code to simulate picking a card from a deck

``` r
# R-code to simulate picking a card from a deck

# Loading the dplyr library for data manipulation 
library(dplyr) 
# Setting a seed to make the results reproducible 
set.seed(1442) 
# Defining a vector of card values 
card_values <- c("A", "2", "3", "4", "5", "6", "7", "8", "9", "10", "J", "Q", "K") 
# Simulating a fair pick from a single suit for 1000 trials 
card_draw <- function(n) {sample(card_values, size = n, replace = TRUE)} 
sim_1000 <- data.frame(Card_Draw = card_draw(1000)) 
print(head(sim_1000, 20))   # prints first 20 rows. 
```

    ##    Card_Draw
    ## 1          3
    ## 2          Q
    ## 3          Q
    ## 4          8
    ## 5          2
    ## 6          A
    ## 7         10
    ## 8          9
    ## 9          9
    ## 10         8
    ## 11         8
    ## 12         8
    ## 13         Q
    ## 14         Q
    ## 15         6
    ## 16         3
    ## 17         3
    ## 18         3
    ## 19         7
    ## 20         8

``` r
# Simulation summary table 
summary_1000 <- table(sim_1000) 
print(summary_1000)
```

    ## Card_Draw
    ## 10  2  3  4  5  6  7  8  9  A  J  K  Q 
    ## 73 74 72 62 78 87 78 78 78 86 84 64 86
