# Reaction Times

## MCC
[Matthews Correlation Coefficient](https://en.wikipedia.org/wiki/Matthews_correlation_coefficient) is a measure of accuracy when true (correct) and false (incorrect) responses are given to positive (response) and negative (non-response) stimuli.

## SSRT
SSRT, or stop-signal reaction time, is the time it takes for the stop-signal to elicit an inhibited response. This is impossible to measure directly but can be approximated. For analysis on approximation methods, see [this paper](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2696813/).


## Distributions
Reaction time distributions are best parameterized by [Exponential-Gauss](https://en.wikipedia.org/wiki/Exponentially_modified_Gaussian_distribution), [Exponential-Wald (link is not exact)](https://en.wikipedia.org/wiki/Inverse_Gaussian_distribution), or [Gamma](Gamma Distribution) distributions, as shown in [this paper](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3062635/). All three perform equally well. We use the Gamma because it's the easiest to implement since most stats packages have gamma functions.