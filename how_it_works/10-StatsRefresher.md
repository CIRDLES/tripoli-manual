---
title: A Statistics Refresher
subject: How It Works
subtitle: 
short_title: 
authors:
  - name: Noah McLean
    affiliation:
      - University of Kansas
    orcid: 0000-0003-0388-1862
    email: noahmc@ku.edu
date: May 15, 2024
license: CC-BY-4.0
keywords: 
exports:
  - format: docx
  - format: pdf
    template: eartharxiv
    article_type: Report
numbering:
  code: false
  headings: false
---

# The arithmetic mean
The arithmetic mean $\bar{x}$ for $n$ measurements indexed $i = 1\ldots n$ is
$$ \bar{x} = \dfrac{1}{n}\sum_{i=1}^n x_i \label{eq:ArithmeticMean}$$


# The variance
The variance $\sigma^2$ is a measure of how scattered about the mean the data points are.
$$ \sigma^2 = \dfrac{1}{n-1}\sum_{i=1}^n \big( x_i - \bar{x}\big)^2 \label{eq:Variance} $$
where $\bar{x}$ is the mean defined in equation [](#eq:ArithmeticMean). The variance is tricky, since it has the same units as your measurements, squared.


# The standard deviation
The standard deviation also measures how your data points scatter around the mean, but this time in units that you actually understand.
$$ \sigma = \sqrt{\sigma^2} $$ 
where $\sigma^2$ is the variance defined in equation [](#eq:Variance). 

# The standard error
The standard error tells you how well you know the mean.  It gets smaller as $n$ gets bigger, reflecting your improved knowledge of the mean as you make more measurements.
$$ \sigma_{\bar{x}} = \dfrac{\sigma}{\sqrt{n}} $$

