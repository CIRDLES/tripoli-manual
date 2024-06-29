---
title: Basic Statistics for Mass Spectrometry
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

Software for all major mass spectrometer manufacturers provides some out-of-the-box statistics to summarize measured data.  Mass spectrometry 

# The arithmetic mean and its uncertainty

## The arithmetic mean
The {term}`arithmetic mean <arithmetic mean>` $\bar{x}$ for $n$ measurements indexed $i = 1\ldots n$ is
$$ \bar{x} = \dfrac{1}{n}\sum_{i=1}^n x_i \label{eq:ArithmeticMean}$$

## The variance
The variance $\sigma^2$ measures the scatter of the data points around the mean value.
$$ \sigma^2 = \dfrac{1}{n-1}\sum_{i=1}^n \big( x_i - \bar{x}\big)^2 \label{eq:Variance} $$
where $\bar{x}$ is the mean defined in equation [](#eq:ArithmeticMean) and $n$ is the number of data points. The variance is tricky because it has the same units as your measurements, squared.

## The standard deviation
The {term}`standard deviation <standard deviation>` also measures how your data points scatter around the mean, but this time in units that you actually understand.
$$ \sigma = \sqrt{\sigma^2} \label{eq:StdDeviation}$$ 
where $\sigma^2$ is the variance defined in equation [](#eq:Variance). 

## The standard error
The {term}`standard error` tells you how well you know the mean.  It gets smaller as $n$ gets bigger, reflecting your improved knowledge of the mean as you make more measurements.
$$ \sigma_{\bar{x}} = \dfrac{\sigma}{\sqrt{n}} \label{eq:StdError} $$

## Standard deviation vs. standard error
Both the standard deviation and the standard error are used to represent uncertainties in measurements.  So which should you use?  

Use the **standard deviation** when you're looking to describe the scatter among your measured data points.  The standard deviation doesn't change as you measure more data and increase $n$.  For instance, you might use the standard deviation to measure the reproducibility of your reference material measurements.  You could use the standard deviation of your past reference material measurements to predict the range of values where your next reference material measurement is likely to be.

Use the **standard error** when you're describing the uncertainty in a mean value.  According to equation [](#eq:StdError), the standard error gets smaller as $n$ increases, reflecting your increased confidence in the mean as you take more measurements.  If you've just measured 100 isotope ratios, then the standard error best reflects your uncertainty in the mean of those 100 ratios.  If you want to improve the uncertainty in the mean by a factor of two, then equation [](#eq:StdError) says that you need to collect four times as much data with the same standard deviation.  

## Relative uncertainties
A relative uncertainty an absolute uncertainty (a standard deviation or a standard error) divided by the mean value.  Relative uncertainties are often expressed in percent (e.g., $100\,\sigma/\bar{x}$), but could also be expressed for instance in per mille or ppm.

# Confidence Intervals

You can calculate a mean, standard deviation, and standard error for any dataset with more than one measurement.  These three statistics are just the numbers that are calculated by the formulas given above.  However, we usually want to make some more quantitative estimates about our data.  For instance, a 95% <wiki:confidence_interval> for the mean would be expected to contain the true value of the mean about 95% of the time.  This idea helps you make the leap from an uncertainty (just a number) to a mental picture of what range of values might reasonably be attributed to the parameter (e.g., isotope ratio) you're measuring.

Isotope ratio data are often presented as a mean value and a ±2σ confidence interval, interpreted as a 95% confidence interval.  To construct a 95% confidence interval in this way, the $\sigma$ that you want is the {term}`standard error`, since it tells you about the uncertainty in the mean value.  For instance, if you measure 100 isotope ratios with a mean of 1.234 and a standard deviation of 0.0120, then the standard error of the ratios is 
$$ \sigma_{\bar{x}} \  = \  \dfrac{\sigma}{\sqrt{n}} \  = \  \dfrac{0.0120}{\sqrt{100}} \  = \  0.0012, $$ 
and a 95% confidence interval for the mean ratio would be 
$$ \bar{x} \pm 2\sigma_{\bar{x}} \  = \  1.234 \pm 0.0024. $$

To make a 95\% confidence interval in this way, though, requires that you make a number of assumptions that are not always met by mass spectrometer data.  For datasets that do not meet these assumptions, you can calculate a ±2σ confidence interval (these are just numbers that come from formulas), but it will not be a 95\% confidence interval.

## Assumptions

The following assumptions are baked into the way we report and think about 

## Visualization

:::{figure} #ratio-plots
:label: fig-ratio-lots
:width:
:align: center
:::