r_code_used_in_jamovi_lab7
================
Siddhartha Chilukuri
2025-10-10

# R-code block for simulating the Repeated Sampling Confidance Level

``` r
#------------------------------------------------------------------------------------------------------------------
# Loading necessary libraries for data manipulation and plotting
#------------------------------------------------------------------------------------------------------------------
library(ggplot2) # A powerful library for creating elegant data visualizations
```

    ## Warning: package 'ggplot2' was built under R version 4.4.3

``` r
library(dplyr)   # A library for data manipulation and transformation
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
library(purrr)   # A library for functional programming (used here for mapping functions)
```

    ## Warning: package 'purrr' was built under R version 4.4.3

``` r
#------------------------------------------------------------------------------------------------------------------
# Setting up the Simulation Parameters
#------------------------------------------------------------------------------------------------------------------
# The true population mean (the value we want our CIs to capture)
true_mean <- 10

# The number of simulated samples
n_samples <- 100                  # <---- Change this

# The sample size for each individual sample
sample_size <- 30


#------------------------------------------------------------------------------------------------------------------
# Generating the 100 samples with 30 observations each of random normal data
#------------------------------------------------------------------------------------------------------------------
# Generating a tibble (a modern data frame) with random data
# We create 100 samples, each with 30 observations drawn from a normal distribution
# with a mean of 10 and a standard deviation of 0.5.
df <- tibble(sample_id = 1:n_samples,
             x = purrr::map(1:n_samples, ~rnorm(sample_size, mean = true_mean, sd = 0.5)))


#------------------------------------------------------------------------------------------------------------------
# Calculating the Confidence Intervals for all 100 samples generated
#------------------------------------------------------------------------------------------------------------------
# Calculating the sample mean and confidence interval for each of the 100 samples
confidence_data <- df %>% mutate(mean_x = purrr::map_dbl(x, ~mean(.x)), 
                                 sd_x = purrr::map_dbl(x, ~sd(.x)),
                                 se_x = sd_x / sqrt(sample_size),
                                 ci_lower = mean_x - qt(0.975, df = sample_size - 1) * se_x,
                                 ci_upper = mean_x + qt(0.975, df = sample_size - 1) * se_x,
                                 covers_true_mean = (ci_lower <= true_mean) & (ci_upper >= true_mean))%>% 
                          select(sample_id, mean_x, ci_lower, ci_upper, covers_true_mean)


#------------------------------------------------------------------------------------------------------------------
# Creating the Plot Title & Subtitle Calculations
#------------------------------------------------------------------------------------------------------------------
# Counting how many CIs successfully covered the true mean
coverage_count <- sum(confidence_data$covers_true_mean)

# Calculating the percentage of successful CIs
coverage_percent <- round((coverage_count / n_samples) * 100)

# Creating the main title for the plot
main_title <- "Confidence-interval coverage across simulations"

# Creating the subtitle dynamically, showing the coverage count and percentage
subtitle_text <- paste0(coverage_count," out of ",n_samples," (", coverage_percent, "%) CIs contain μ=", true_mean)


#------------------------------------------------------------------------------------------------------------------
# Plotting with ggplot2
#------------------------------------------------------------------------------------------------------------------
# Initializing the plot with the data and aesthetic mappings
ggplot(confidence_data, aes(x = mean_x, y = as.factor(sample_id))) +
       # Adding a vertical line at the true mean to serve as a reference
       geom_vline(xintercept = true_mean, color = "#050505", linetype = "solid", size = 0.8) +
       # Plotting the confidence intervals as horizontal error bars
       # The color is determined by whether the CI covers the true mean
       geom_errorbarh(aes(xmin = ci_lower, xmax = ci_upper, color = covers_true_mean), height = 0.2) +
       # Plotting the sample means as points
       geom_point(aes(color = covers_true_mean)) +
       # Adding the black line at the bottom to represent the overall range
       # This line shows the total span of all the calculated CIs
       geom_segment(aes(x = min(ci_lower), xend = max(ci_upper), 
                        y = 0, yend = 0), color = "#050505",size = 0.5,
                        lineend = "round") +
       # Manually set the colors for the confidence intervals (green for success, red for failure)
       scale_color_manual(values = c("TRUE" = "#3BAD3E", "FALSE" = "#DB0736")) +
       # Adding labels for the title, subtitle, and axes
       labs(title = main_title,
            subtitle = subtitle_text,
            x = "Estimate / 95% CI for mean",
            y = "Sample Number") +
       # Applying a clean, minimal theme to the plot
       theme(plot.title = element_text(size = 13, face = "bold"),
             plot.subtitle = element_text(size = 11),
             # Removing all background grid lines for a cleaner look
             panel.background = element_blank(),
             panel.grid.major = element_blank(),
             panel.grid.minor = element_blank(),
             # Hiding the legend as the colors are explained in the plot itself
             legend.position = "none")
```

    ## Warning: Using `size` aesthetic for lines was deprecated in ggplot2 3.4.0.
    ## ℹ Please use `linewidth` instead.
    ## This warning is displayed once every 8 hours.
    ## Call `lifecycle::last_lifecycle_warnings()` to see where this warning was
    ## generated.

    ## Warning in geom_segment(aes(x = min(ci_lower), xend = max(ci_upper), y = 0, : All aesthetics have length 1, but the data has 100 rows.
    ## ℹ Please consider using `annotate()` or provide this layer with data containing
    ##   a single row.

![](r_code_used_in_jamovi_lab7_files/figure-gfm/unnamed-chunk-1-1.png)<!-- -->
