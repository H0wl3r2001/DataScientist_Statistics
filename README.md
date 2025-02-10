# DataScientist_Statistics

## Introduction

Statistics is a fundamental pillar of data science, providing tools to describe, analyze, and infer insights from data. This repository covers key statistical concepts essential for data science, including descriptive statistics, inferential statistics fundamentals, confidence intervals, and hypothesis testing.

## Table of Contents

1. [Descriptive Statistics](#descriptive-statistics)
2. [Inferential Statistics Fundamentals](#inferential-statistics-fundamentals)
3. [Confidence Intervals](#confidence-intervals)
4. [Hypothesis Testing](#hypothesis-testing)

---

## Descriptive Statistics

Descriptive statistics summarize and organize characteristics of a dataset.

### Measures of Central Tendency

- **Mean** (Arithmetic Average):
  $$
  \bar{x} = \frac{\sum_{i=1}^{n} x_i}{n}
  $$
- **Median**: The middle value when data is ordered.
- **Mode**: The most frequently occurring value in the dataset.

### Measures of Dispersion

- **Variance**:

    $$
    \sigma^2 = \frac{\sum_{i=1}^{n} (x_i - \bar{x})^2}{n}
    $$

- **Standard Deviation**:

    $$
    \sigma = \sqrt{\sigma^2}
    $$

- **Range**: The difference between the maximum and minimum values.
- **Interquartile Range (IQR)**: Difference between Q3 and Q1 (75th and 25th percentiles).

---

## Inferential Statistics Fundamentals

Inferential statistics allow us to make predictions and inferences about a population from a sample.

### Sampling Techniques

- **Simple Random Sampling**: Every individual has an equal chance of selection.
- **Stratified Sampling**: The population is divided into subgroups, and random samples are taken from each.
- **Cluster Sampling**: The population is divided into clusters, and entire clusters are randomly selected.

### Probability Distributions

As previously seen in the probability project-section, let's revise some of the formulas for the most relevant probability distributions:

- **Normal Distribution** (Gaussian):

  $$
  f(x) = \frac{1}{\sigma \sqrt{2\pi}} e^{-\frac{(x-\mu)^2}{2\sigma^2}}
  $$

- **Binomial Distribution**:

  $$
  P(X = k) = \binom{n}{k} p^k (1-p)^{n-k}
  $$

- **Poisson Distribution**:

  $$
  P(X = k) = \frac{e^{-\lambda} \lambda^k}{k!}
  $$

---

## Confidence Intervals

A confidence interval estimates a range within which a population parameter is expected to lie.

- **Formula for a confidence interval (for mean, when population variance is unknown):**

  $$
  \bar{x} \pm t^* \frac{s}{\sqrt{n}}
  $$

  where:
  - $t^*$ is the critical value from the t-distribution
  - $s$ is the sample standard deviation
  - $n$ is the sample size

- **Z-score vs. t-score**:
  - Use a **Z-score** when population standard deviation is known.
  - Use a **t-score** when population standard deviation is unknown and sample size is small ($n < 30$).

---

## Hypothesis Testing

Hypothesis testing evaluates claims about a population using sample data.

### Steps in Hypothesis Testing

1. Define the **null hypothesis (H₀)** and **alternative hypothesis (H₁)**.
2. Choose a significance level ($\alpha$, commonly 0.05).
3. Select the appropriate test (Z-test, t-test, chi-square test, etc.).
4. Calculate the test statistic.
5. Compare with the critical value or compute the p-value.
6. Reject or fail to reject H₀ based on the comparison.

### Common Statistical Tests

- **Z-test** (for large samples, known variance):
  
  $$
  Z = \frac{\bar{x} - \mu}{\sigma / \sqrt{n}}
  $$

- **t-test** (for small samples, unknown variance):
  
  $$
  t = \frac{\bar{x} - \mu}{s / \sqrt{n}}
  $$

- **Chi-square test** (for categorical data):
  
  $$
  \chi^2 = \sum \frac{(O - E)^2}{E}
  $$
  

---

## Conclusion

Understanding these statistical concepts is crucial for analyzing data effectively in data science. This repository will provide deeper theoretical explanations along with practical examples to help you navigate or revise these techniques.

### Contributions

Feel free to contribute by adding examples, code implementations, or additional topics!

### License

This project is licensed under the MIT License.
