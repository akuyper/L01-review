---
title: "L01 Review"
author: "Data Science III (STAT 301-3)"
output: 
  html_document:
    toc: true
    toc_float: true
    highlight: "tango"
---

## Overview

The goal of this lab is to review concepts and techniques from the previous quarter (STAT 301-2).

# Datasets

We will be using the `wildfires.csv` dataset contained in the **data** subdirectory. Read `wildfires_codebook.html` to familiarize yourself with the dataset.

## Exercises

Please complete the following exercises. Be sure that your solutions are clearly indicated and that your document is neatly formatted.

#### Load Packages

```{r, message = FALSE}
# Loading package(s)

```

### Exercise 1

The total area burned by a wildfire is of great concern to government planners. This is captured by the continuous variable `burned` in the `wildfires` dataset. The goal of this exercise is to build a model for predicting the total area burned by a wildfire (`burned`).

Use 10-fold cross validation with 2 repeats. Compare two models:

-   an elastic net, tuning `penalty()` and `mixture()`
-   a boosted tree, tuning `learn_rate()` and `mtry()`

Use the RMSE metric to tune models and assess model performance on the test set.

### Exercise 2

Using your own words, briefly define each of the following terms and explain why they are important:

-   V-fold cross-validation

-   Repeated cross-validation

-   Model tuning

-   Data splitting

-   Bias-variance tradeoff (in the context of mechanistic vs. empirically-driven models)

-   Overfitting

-   Feature engineering

-   ROC curve


### Exercise 3

A wildlife protection area is located in the park from which this data was collected. The variable `wlf` in the dataset denotes whether or not fires reached that protection area.

The goal of this exercise is to build a model for predicting whether or not a fire will reach the protection area (`wlf`).

Use 10-fold cross validation with 2 repeats. Compare two models:

-   an elastic net, tuning `penalty()` and `mixture()`
-   a boosted tree, tuning `learn_rate()` and `mtry()`

Use the ROC AUC metric to tune models and assess model performance on the test set. <br><br>
