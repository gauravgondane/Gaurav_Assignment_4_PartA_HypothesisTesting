# Hypothesis Testing for Weekly Operating Costs

This repository contains Python code to perform hypothesis testing to investigate restaurant owners' claims about increased weekly operating costs for Bombay Hospitality Ltd. franchises. The code follows a systematic approach to test whether the mean weekly operating cost has increased beyond the predicted value of $3,000.

---

## Background

Bombay Hospitality Ltd. operates a franchise model producing exotic Norwegian dinners in New England. The weekly operating cost (W) is modeled as:
\[ W = 1,000 + 5X \]
Where:
- \( X \) = Number of units produced in a week.

The predicted operating cost for \( X = 600 \) units is $3,000. Restaurant owners claim the actual operating costs are higher. This hypothesis is tested using the provided sample data.

---

## Objective

To verify if the mean weekly operating costs have increased beyond the predicted value of $3,000 using hypothesis testing.

---

## Hypothesis

- **Null Hypothesis (H₀)**: \( \mu = 3000 \)  
- **Alternative Hypothesis (H₁)**: \( \mu > 3000 \)  

Where:
- \( \mu \) = True mean of weekly operating costs.

---

## Steps Performed in the Code

### 1. **Calculate Standard Error**
The standard error is computed using the formula:
\[ \text{Standard Error} = \frac{\sigma}{\sqrt{n}} \]
Where:
- \( \sigma = 125 \) (standard deviation of the sample)
- \( n = 25 \) (sample size)

### 2. **Calculate Test Statistic**
The test statistic (t-score) is calculated as:
\[ t = \frac{\bar{x} - \mu}{\text{Standard Error}} \]
Where:
- \( \bar{x} = 3050 \) (sample mean)
- \( \mu = 3000 \) (hypothesized mean)

### 3. **Calculate p-value**
The p-value is computed using the t-distribution for \( n - 1 \) degrees of freedom.

### 4. **Compare Against Significance Level (\( \alpha = 0.05 \))**
- If \( p \)-value \( < \alpha \), reject \( H₀ \).
- If \( p \)-value \( \geq \alpha \), fail to reject \( H₀ \).

### 5. **Compute Z-Score and Z-Critical Value (Alternative Method)**
Using the z-distribution:
\[ z = \frac{\bar{x} - \mu}{\frac{\sigma}{\sqrt{n}}} \]

Compare \( z \)-score with \( z \)-critical value to determine the result.

---

## Results and Interpretation

The code outputs the following:

1. **Standard Error**: Measure of variability in the sample mean.
2. **Test Statistic (t-score)**: Value used to compute the p-value.
3. **p-value**: Probability of observing the sample mean if \( H₀ \) is true.
4. **Z-Score**: Alternative test statistic for comparison.
5. **Z-Critical Value**: Threshold value at a significance level (\( \alpha = 0.05 \)).
6. **Hypothesis Decision**: Based on p-value or z-score.

---
