# Misuses of the Kolmogorov–Smirnov Test

Based on a [paper](https://digitalcommons.lib.uconn.edu/cgi/viewcontent.cgi?article=1900&context=srhonors_theses) by Anthony Zeimbekakis.

## Abstract

The Kolmogorov–Smirnov (KS) test is one of the most popular goodness-of-fit tests for com-
paring a sample with a hypothesized parametric distribution. Nevertheless, it has often
been misused. The standard one-sample KS test applies to independent, continuous data
with a hypothesized distribution that is completely specified. It is not uncommon, however,
to see in the literature that it was applied to dependent, discrete, or rounded data, with
hypothesized distributions containing estimated parameters. For example, it has been “dis-
covered” multiple times that the test is too conservative when the parameters are estimated.

## Implementation

This repository contains an implementation of two algorithms mentioned in the paper, which can be used to derive the p-value of the Kolmogorov–Smirnov test, when the distribution parameters from $H_0$ are estimated.

The test is implemented for data coming from the following distributions:

- Gamma
- Weibull

## Usage

All code is in the [notebook](ks_test_misuse.ipynb) file. The notebook contains implementations of the parametric and nonparametric methods along with a simulation study to compare the two methods and against the naive approach.
