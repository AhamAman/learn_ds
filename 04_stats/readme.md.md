# Statistics Foundations Mastery Checklists

> A complete, phase-by-phase learning roadmap covering Data Types, Sampling, Descriptive Statistics, Central Limit Theorem, and Hypothesis Testing — from first principles to real-world application.

---

## Table of Contents

1. [Data Types](#1-data-types)
2. [Sampling Techniques](#2-sampling-techniques)
3. [Descriptive Statistics](#3-descriptive-statistics)
4. [Central Limit Theorem (CLT)](#4-central-limit-theorem-clt)
5. [Statistical Testing (Hypothesis Testing)](#5-statistical-testing-hypothesis-testing)

---

# 1. Data Types

---

## Foundations

- [ ] Qualitative vs Quantitative data
- [ ] Structured vs Unstructured data

---

## Categorical Data

- [ ] Nominal (no order — e.g. blood group, color)
- [ ] Ordinal (ordered — e.g. ratings, satisfaction)

---

## Numerical Data

- [ ] Discrete (countable — e.g. number of students)
- [ ] Continuous (measurable — e.g. height, temperature)

---

## Measurement Scales

- [ ] Nominal Scale — labels only, no order
- [ ] Ordinal Scale — ordered, differences not meaningful
- [ ] Interval Scale — ordered, equal differences, no true zero
- [ ] Ratio Scale — ordered, equal differences, true zero exists

---

## Data Science Applications

- [ ] Choosing the right chart for a data type
- [ ] Choosing the right statistic for a data type
- [ ] Choosing the right ML feature encoding
- [ ] Identifying data types in real datasets

---

## Can Explain

- [ ] Why average salary makes sense (ratio scale)
- [ ] Why average blood group doesn't (nominal scale)
- [ ] Why ratings are ordinal and not interval
- [ ] Difference between interval and ratio scales
- [ ] Why you can't divide ordinal values meaningfully

---

# 2. Sampling Techniques

---

## Phase 0: Foundations

### Core Concepts

- [ ] What is a Population?
- [ ] What is a Sample?
- [ ] Population vs Sample
- [ ] Census vs Sampling
- [ ] Sampling Frame
- [ ] Sampling Unit
- [ ] Representativeness

### First Principles

- [ ] Why Sampling Exists
- [ ] Cost vs Accuracy Tradeoff
- [ ] Sample as Population Approximation
- [ ] Sources of Error

---

## Phase 1: Probability Sampling

### Introduction

- [ ] What is Probability Sampling?
- [ ] Why Randomness Matters
- [ ] Equal vs Unequal Selection Probability

---

### Simple Random Sampling (SRS)

**Concepts**
- [ ] Simple Random Sampling definition
- [ ] Sampling With Replacement
- [ ] Sampling Without Replacement

**Understand**
- [ ] Equal selection probability for all units
- [ ] Advantages: unbiased, simple
- [ ] Limitations: impractical for large populations

**Exercises**
- [ ] Draw random samples from a dataset
- [ ] Compare multiple random samples

---

### Systematic Sampling

**Concepts**
- [ ] Sampling Interval (k = N/n)
- [ ] Random Starting Point

**Understand**
- [ ] How systematic selection works
- [ ] Hidden pattern risks (periodicity bias)

**Exercises**
- [ ] Build systematic samples
- [ ] Compare with SRS

---

### Stratified Sampling

**Concepts**
- [ ] Stratum definition
- [ ] Stratification Variables

**Types**
- [ ] Proportionate Stratified Sampling
- [ ] Disproportionate Stratified Sampling

**Understand**
- [ ] Why stratification improves representation
- [ ] Variance reduction vs SRS

**Exercises**
- [ ] Gender-based stratification
- [ ] Region-based stratification

---

### Cluster Sampling

**Concepts**
- [ ] Cluster definition
- [ ] Natural grouping (schools, cities, blocks)

**Types**
- [ ] One-Stage Cluster Sampling
- [ ] Two-Stage Cluster Sampling

**Understand**
- [ ] Cost savings over SRS
- [ ] Geographic and logistical sampling

**Exercises**
- [ ] School survey example
- [ ] City survey example

---

### Multistage Sampling

**Concepts**
- [ ] Multiple Sampling Levels
- [ ] Hierarchical Sampling

**Example**
- [ ] Country → State → City → Household

**Understand**
- [ ] Real-world large-scale survey design

---

## Phase 2: Non-Probability Sampling

### Introduction

- [ ] What is Non-Probability Sampling?
- [ ] Advantages: quick, cheap, practical
- [ ] Limitations: results not generalizable

---

### Convenience Sampling

- [ ] Easy-access sampling
- [ ] Bias risks
- [ ] Common in early-stage research

---

### Judgment (Purposive) Sampling

- [ ] Expert selection of units
- [ ] Researcher-driven sampling
- [ ] Subjectivity concerns

---

### Quota Sampling

- [ ] Category quotas defined upfront
- [ ] Controlled representation
- [ ] Difference from Stratified Sampling (no randomness)

---

### Snowball Sampling

- [ ] Referral-based sampling
- [ ] Use cases: rare populations, hard-to-reach groups

---

### Voluntary Response Sampling (Added)

- [ ] Participants self-select
- [ ] Strong volunteer bias risk
- [ ] Common in online surveys, polls

---

## Phase 3: Sampling Error & Bias

### Sampling Error

- [ ] Definition: difference between sample and population
- [ ] Sources of sampling error
- [ ] Sampling Variability

### Sampling Bias

**Types**
- [ ] Selection Bias
- [ ] Undercoverage Bias
- [ ] Nonresponse Bias
- [ ] Survivorship Bias
- [ ] Volunteer Bias
- [ ] Recall Bias (Added)
- [ ] Observer Bias (Added)

**Understand**
- [ ] Error vs Bias (error is random, bias is systematic)
- [ ] Why bias is more dangerous than random error

---

## Phase 4: Sample Size Determination

### Concepts

- [ ] Sample Size (n)
- [ ] Margin of Error
- [ ] Confidence Level
- [ ] Population Size effect on required n

### Understand

- [ ] Sample size tradeoffs (cost vs precision)
- [ ] Diminishing returns beyond a certain n
- [ ] Power analysis for sample size (Added)

---

## Phase 5: Sampling Distributions

### Concepts

- [ ] Sampling Distribution definition
- [ ] Distribution of Sample Means
- [ ] Standard Error

### Understand

- [ ] Why samples differ from each other
- [ ] Foundation for statistical inference

**Exercises**
- [ ] Simulate repeated sampling
- [ ] Plot sampling distributions

---

## Phase 6: Central Limit Theorem Connection

### Concepts

- [ ] Central Limit Theorem (CLT)
- [ ] Sample Means converge to normality
- [ ] Convergence speed depends on population shape

### Understand

- [ ] Why CLT makes inference possible
- [ ] Why n ≥ 30 is a common rule of thumb

---

## Phase 7: Survey Design Fundamentals

### Concepts

- [ ] Questionnaire Design principles
- [ ] Response Bias
- [ ] Measurement Error
- [ ] Leading Questions (Added)
- [ ] Double-Barreled Questions (Added)

### Understand

- [ ] How question wording affects data quality
- [ ] Survey reliability and validity

---

## Phase 8: Data Science Applications

- [ ] A/B Testing sample design
- [ ] Customer Analytics sampling
- [ ] Market Research
- [ ] Election Polling
- [ ] Recommendation Systems
- [ ] Model Training Data Selection
- [ ] Handling imbalanced classes via sampling (Added)

---

## Phase 9: Python for Sampling

### NumPy

- [ ] random.choice()
- [ ] random.seed()

### Pandas

- [ ] DataFrame.sample()
- [ ] Stratified sampling with groupby (Added)

### Simulations

- [ ] Random sampling experiments
- [ ] Bias demonstrations
- [ ] CLT simulations

---

## Phase 10: Real Projects

### Beginner
- [ ] Student Survey Analysis
- [ ] Product Feedback Analysis

### Intermediate
- [ ] Customer Satisfaction Study
- [ ] Market Research Dataset

### Advanced
- [ ] Election Poll Simulation
- [ ] Sampling Bias Detection System

---

## Final Mastery

**Can Explain:** Population vs Sample, Census vs Sampling, Probability vs Non-Probability Sampling, SRS, Systematic, Stratified, Cluster, Multistage Sampling, Sampling Error, Sampling Bias, Standard Error, Sample Size Determination, Sampling Distribution, CLT Connection

**Can Apply:** Choose correct sampling technique, detect biased samples, design representative surveys, estimate population characteristics, evaluate survey quality, build sampling workflows in Python

---

# 3. Descriptive Statistics

---

## Phase 0: Foundations

### Core Concepts

- [ ] What is Statistics?
- [ ] Descriptive vs Inferential Statistics
- [ ] Population / Sample / Variable / Observation / Dataset

### Data Types Review

- [ ] Categorical / Numerical / Discrete / Continuous
- [ ] Nominal / Ordinal / Interval / Ratio

---

## Phase 1: Data Summarization

### Understand

- [ ] Why summarize data?
- [ ] Raw data vs summarized data
- [ ] Distribution overview

### Tabular Summaries

- [ ] Frequency Table
- [ ] Relative Frequency
- [ ] Percentage Distribution
- [ ] Cumulative Frequency
- [ ] Cross-tabulation / Contingency Table (Added)

**Exercises**
- [ ] Create frequency tables
- [ ] Build category distributions

---

## Phase 2: Measures of Central Tendency

### Mean

- [ ] Arithmetic Mean
- [ ] Weighted Mean
- [ ] Trimmed Mean (Added — robust to outliers)
- [ ] Geometric Mean (Added — for rates, growth)
- [ ] Harmonic Mean (Added — for ratios, speeds)

**Understand**
- [ ] Interpretation in context
- [ ] Effect of outliers on mean
- [ ] When mean is appropriate

---

### Median

- [ ] Median for odd-sized datasets
- [ ] Median for even-sized datasets

**Understand**
- [ ] Robustness to outliers
- [ ] Better for skewed distributions

---

### Mode

- [ ] Single Mode / Multiple Modes / No Mode
- [ ] Bimodal distributions (Added)

**Understand**
- [ ] Best measure for categorical data

---

### Choosing the Right Measure

| Data Type | Best Measure |
|---|---|
| Symmetric numerical | Mean |
| Skewed numerical | Median |
| Categorical | Mode |
| Contains outliers | Median |

---

## Phase 3: Measures of Dispersion (Spread)

### Range

- [ ] Minimum / Maximum / Range
- [ ] Sensitivity to outliers

---

### Variance

- [ ] Population Variance (σ²)
- [ ] Sample Variance (s²)
- [ ] Why squaring is used (penalizes large deviations)
- [ ] Bessel's correction — why divide by n−1 (Added)

**Exercises**
- [ ] Manual variance calculation

---

### Standard Deviation

- [ ] Population Standard Deviation (σ)
- [ ] Sample Standard Deviation (s)
- [ ] Relationship to variance

**Exercises**
- [ ] Compare low vs high variability datasets

---

### Interquartile Range (IQR)

- [ ] Q1 / Q2 (Median) / Q3
- [ ] IQR = Q3 − Q1
- [ ] Resistant measure of spread
- [ ] Outlier detection: below Q1−1.5×IQR or above Q3+1.5×IQR

---

### Coefficient of Variation (CV)

- [ ] CV = (σ / μ) × 100%
- [ ] Comparing variability across different scales

---

### Mean Absolute Deviation (Added)

- [ ] MAD: average absolute deviation from mean
- [ ] More interpretable than variance

---

## Phase 4: Percentiles & Quantiles

- [ ] Percentiles / Deciles / Quartiles / Quantiles
- [ ] Ranking observations and position within dataset

**Exercises**
- [ ] Calculate percentile ranks

---

## Phase 5: Shape of Distribution

### Symmetry

- [ ] Symmetric Distribution
- [ ] Left-Skewed (Negative Skew)
- [ ] Right-Skewed (Positive Skew)
- [ ] Impact on mean vs median relationship

---

### Skewness

- [ ] Positive Skewness (tail right)
- [ ] Negative Skewness (tail left)
- [ ] Rule: mean > median → right skew

**Exercises**
- [ ] Identify skewed datasets visually and numerically

---

### Kurtosis

- [ ] Leptokurtic (heavy tails, peaked)
- [ ] Mesokurtic (normal-like)
- [ ] Platykurtic (light tails, flat)
- [ ] Excess kurtosis = kurtosis − 3 (Added)

---

## Phase 6: Outlier Analysis

### Concepts

- [ ] What is an outlier?
- [ ] Sources: data entry error, genuine extreme value

### Detection Methods

- [ ] IQR Method (1.5 × IQR rule)
- [ ] Z-Score Method (|z| > 3)
- [ ] Modified Z-Score (Added — uses median, more robust)
- [ ] Isolation Forest for multivariate outliers (Added)

**Exercises**
- [ ] Detect outliers in real datasets

---

## Phase 7: Visualization for Descriptive Statistics

### Histograms

- [ ] Distribution visualization
- [ ] Bin selection (Sturges rule, Scott rule) (Added)
- [ ] Interpret shape, spread, center

---

### Box Plots

- [ ] Median / Quartiles / IQR / Whiskers / Outliers
- [ ] Side-by-side box plots for comparison (Added)

---

### Bar Charts

- [ ] Categorical frequencies

---

### Density Plots (KDE)

- [ ] Smooth distribution estimate
- [ ] Bandwidth selection (Added)

---

### Scatter Plots

- [ ] Relationship exploration

---

### Violin Plots (Added)

- [ ] Combines box plot + density plot

---

### QQ Plot (Added)

- [ ] Check normality assumption visually

---

## Phase 8: Five Number Summary

- [ ] Minimum / Q1 / Median / Q3 / Maximum
- [ ] Distribution overview at a glance

---

## Phase 9: Standardization

### Learn

- [ ] Standard Score (Z-Score)
- [ ] Z = (x − μ) / σ
- [ ] Relative position within distribution
- [ ] Comparing values across different scales

**Exercises**
- [ ] Standardize datasets
- [ ] Interpret Z-scores in context

---

## Phase 10: Grouped Data Statistics

- [ ] Grouped Frequency Tables / Class Intervals
- [ ] Grouped Mean / Grouped Median / Grouped Mode

---

## Phase 11: Covariance & Correlation (Added)

### Covariance

- [ ] Direction of relationship between two variables
- [ ] Scale-dependent (hard to interpret)

### Pearson Correlation

- [ ] Standardized covariance (−1 to +1)
- [ ] Linear relationship strength

### Spearman Correlation

- [ ] Rank-based, handles non-linear monotonic relationships

### Understand

- [ ] Correlation ≠ Causation
- [ ] Spurious correlations

---

## Phase 12: Descriptive Statistics with Python

### NumPy

- [ ] mean() / median() / std() / var() / percentile()

### Pandas

- [ ] describe() / value_counts() / quantile() / corr()

### SciPy

- [ ] skew() / kurtosis()

### Matplotlib / Seaborn (Added)

- [ ] histplot() / boxplot() / violinplot() / kdeplot()

---

## Phase 13: Comparing Distributions

- [ ] Compare Centers / Spread / Shape
- [ ] Overlapping histograms
- [ ] Side-by-side box plots

---

## Phase 14: Real-World Applications

### Business Analytics

- [ ] Sales Analysis / Customer Analysis / Revenue Analysis

### Data Science

- [ ] EDA / Feature Understanding / Data Quality Assessment

### Finance

- [ ] Risk Analysis / Return Analysis / Portfolio Variance

### Healthcare (Added)

- [ ] Patient outcomes / Clinical trial summaries

---

## Phase 15: Common Mistakes

- [ ] Using mean with highly skewed data
- [ ] Ignoring outliers without investigation
- [ ] Confusing variance and standard deviation
- [ ] Assuming correlation implies causation
- [ ] Using wrong statistics for categorical data
- [ ] Ignoring sample size when comparing groups (Added)

---

## Phase 16: Real Projects

### Beginner
- [ ] Student Marks Analysis
- [ ] Employee Salary Analysis

### Intermediate
- [ ] Customer Analytics Report
- [ ] Product Sales Report

### Advanced
- [ ] Full EDA Report
- [ ] Business KPI Dashboard

---

## Final Mastery

**Can Explain:** Mean, Median, Mode, Range, Variance, Standard Deviation, IQR, Percentiles, Quartiles, Skewness, Kurtosis, Outliers, Five Number Summary, Z-Score, Correlation

**Can Apply:** Summarize datasets, compare distributions, detect outliers, choose appropriate summary statistics, perform EDA, build descriptive statistical reports

---

# 4. Central Limit Theorem (CLT)

---

## Phase 0: Prerequisites

### Statistics Foundations

- [ ] Population / Sample / Mean / Variance / Standard Deviation

### Sampling

- [ ] Random Sampling / Sampling Error / Sampling Bias

### Probability Distributions

- [ ] Normal Distribution / Random Variables / Probability Distribution

---

## Phase 1: Why CLT Exists

### The Problem

- [ ] Different samples produce different results
- [ ] Sample means vary naturally
- [ ] Need a predictable pattern for inference

### First Principles

- [ ] Population Distribution
- [ ] Sample Distribution
- [ ] Sample Mean as a random variable

### Understand

- [ ] Why samples differ from each other
- [ ] Why uncertainty exists in statistics

---

## Phase 2: Sampling Distribution

### Core Concepts

- [ ] What is a Sampling Distribution?
- [ ] Distribution of Sample Means
- [ ] Distribution of Sample Proportions

### Understand

- [ ] One sample vs many samples concept
- [ ] Repeated sampling process

**Exercises**
- [ ] Draw multiple samples from a population
- [ ] Compare sample means

---

## Phase 3: Central Limit Theorem Fundamentals

### Core Statement

As sample size increases, the distribution of sample means approaches a normal distribution, regardless of the original population shape.

- [ ] Definition of CLT
- [ ] Conditions for CLT
- [ ] Importance of CLT

### Key Ideas

- [ ] Population can be any shape (uniform, skewed, bimodal)
- [ ] Sampling distribution becomes approximately normal
- [ ] This enables all of classical inference

---

## Phase 4: Visual Understanding

### Population Shapes

- [ ] Uniform Population
- [ ] Skewed Population
- [ ] Bimodal Population
- [ ] Exponential Population

### Observe CLT at Different Sample Sizes

- [ ] n = 5
- [ ] n = 10
- [ ] n = 30
- [ ] n = 50
- [ ] n = 100

**Exercises**
- [ ] Simulate CLT visually in Python

---

## Phase 5: CLT Components

### Population Mean (μ)

- [ ] Center of the sampling distribution

### Population Standard Deviation (σ)

- [ ] Drives variability of sample means

### Sample Size (n)

- [ ] Small samples → more spread in sampling distribution
- [ ] Large samples → tighter sampling distribution

---

## Phase 6: Standard Error

### Learn

- [ ] Standard Error (SE) = σ / √n
- [ ] Standard deviation of the sampling distribution of means

### Understand

- [ ] SE measures precision of the sample mean estimate
- [ ] Larger n → smaller SE → more precise

**Exercises**
- [ ] Calculate SE for various sample sizes
- [ ] Plot SE vs n curve

---

## Phase 7: Effects of Sample Size

- [ ] Increasing n → shrinking SE
- [ ] Why larger samples produce more stable estimates
- [ ] Why precision improves with more data

**Exercises**
- [ ] Compare n=10 vs n=100 vs n=1000

---

## Phase 8: CLT Conditions

### Required Conditions

- [ ] Random Sampling
- [ ] Independence of observations
- [ ] 10% condition (sample < 10% of population)

### Sample Size Rules

- [ ] n ≥ 30 rule of thumb
- [ ] Symmetric populations: smaller n sufficient
- [ ] Heavily skewed populations: larger n needed

### Understand

- [ ] n=30 is a guideline, not a law
- [ ] When CLT may fail (very small n, extreme skew)

---

## Phase 9: CLT for Means

### Properties

- [ ] Mean of sampling distribution = μ
- [ ] Standard Error = σ / √n
- [ ] Shape → Normal as n increases

**Understand**
- [ ] Why sample means are approximately normal for large n

---

## Phase 10: CLT for Proportions

### Learn

- [ ] Sample Proportion (p̂)
- [ ] Sampling distribution of proportions

### Conditions

- [ ] Success-Failure rule: np ≥ 10 and n(1−p) ≥ 10

**Exercises**
- [ ] Survey proportion examples
- [ ] Election polling examples

---

## Phase 11: CLT Simulations in Python

### NumPy

- [ ] Generate random populations of different shapes
- [ ] Draw repeated samples

### Visualization

- [ ] Histograms of sample means at different n

**Exercises**
- [ ] Uniform population → normal sampling distribution
- [ ] Exponential population → normal sampling distribution
- [ ] Heavily skewed → observe convergence rate

---

## Phase 12: CLT and Normal Distribution

- [ ] Why the normal distribution dominates classical statistics
- [ ] Population distribution vs sampling distribution — don't confuse them

---

## Phase 13: CLT and Z-Scores

### Learn

- [ ] Z = (x̄ − μ) / (σ / √n)
- [ ] Standardizing a sample mean

**Exercises**
- [ ] Calculate z-scores for sample means
- [ ] Find probability of observing a certain sample mean

---

## Phase 14: CLT and Confidence Intervals

### Learn

- [ ] Why confidence intervals are built on CLT
- [ ] CLT → Normality → Interval estimation

**Understand**
- [ ] Without CLT, we couldn't build CIs for arbitrary populations

---

## Phase 15: CLT and Hypothesis Testing

### Learn

- [ ] Why test statistics follow known distributions
- [ ] CLT → Test Statistics → P-values

**Connection**
- [ ] Every common statistical test relies on CLT

---

## Phase 16: Law of Large Numbers vs CLT (Added)

### Law of Large Numbers (LLN)

- [ ] Sample mean converges to population mean as n → ∞
- [ ] About the value of the mean

### CLT

- [ ] About the shape of the distribution of sample means
- [ ] LLN and CLT are complementary, not the same

---

## Phase 17: Practical Applications

### Surveys

- [ ] Election Polling
- [ ] Customer Satisfaction Surveys

### Business

- [ ] Sales Estimation / Revenue Forecasting

### Data Science

- [ ] Model Evaluation / Experiment Analysis

### Machine Learning

- [ ] Sampling Training Data
- [ ] Bootstrap methods (Added)

---

## Phase 18: Common Misconceptions

- [ ] CLT does NOT make the original data normal
- [ ] CLT applies to sample means, not individual observations
- [ ] n=30 is not a magic number — it depends on population shape
- [ ] CLT requires proper random sampling

**Exercises**
- [ ] Identify incorrect CLT claims

---

## Phase 19: Real Projects

### Beginner
- [ ] Dice Roll CLT Simulation
- [ ] Coin Toss CLT Simulation

### Intermediate
- [ ] Survey Analysis with CLT
- [ ] Polling Simulation

### Advanced
- [ ] Confidence Interval Calculator
- [ ] Sampling Distribution Simulator

---

## Final Mastery

**Can Explain:** Population vs Sample, Sampling Distribution, CLT, Standard Error, Effect of Sample Size, CLT Conditions, CLT for Means, CLT for Proportions, CLT vs Normal Distribution, CLT vs Law of Large Numbers, Why CIs Work, Why Hypothesis Tests Work

**Can Apply:** Simulate CLT, Calculate Standard Error, Interpret Sampling Distributions, Build Confidence Intervals, Perform Statistical Inference

---

# 5. Statistical Testing (Hypothesis Testing)

---

## Phase 0: Prerequisites

### Statistics Foundations

- [ ] Population / Sample / Mean / Median / Variance / Standard Deviation

### Probability Foundations

- [ ] Probability / Random Variables / Normal Distribution / Z-Score

### Sampling Foundations

- [ ] Sampling Distribution / CLT / Standard Error

---

## Phase 1: Why Statistical Testing Exists

### The Problem

- [ ] Samples vary naturally
- [ ] Observed differences may occur by chance
- [ ] Need a formal method to evaluate evidence

### First Principles

- [ ] Signal vs Noise
- [ ] Random Variation
- [ ] Statistical Evidence

### Understand

- [ ] Why intuition alone is insufficient
- [ ] Why we need formal decision frameworks

---

## Phase 2: Hypothesis Fundamentals

### Learn

- [ ] Null Hypothesis (H₀) — default assumption, no effect
- [ ] Alternative Hypothesis (H₁) — what we're testing for

### Understand

- [ ] We assume H₀ is true initially
- [ ] We gather evidence against H₀
- [ ] Fail to Reject H₀ ≠ Accept H₀ (Added)

**Exercises**
- [ ] Define hypotheses for business problems
- [ ] Translate research questions into H₀ and H₁

---

## Phase 3: Test Statistics

### Learn

- [ ] Test Statistic: standardized measure of evidence against H₀

### Common Statistics

- [ ] Z Statistic (known σ, large n)
- [ ] T Statistic (unknown σ, small n)
- [ ] Chi-Square Statistic (categorical data)
- [ ] F Statistic (comparing variances / ANOVA)

---

## Phase 4: Significance Level (α)

### Common Values

- [ ] α = 0.10 (lenient)
- [ ] α = 0.05 (standard)
- [ ] α = 0.01 (strict)

### Understand

- [ ] α is the decision threshold — maximum acceptable Type I error rate
- [ ] Chosen before seeing data (Added)

---

## Phase 5: P-Value

### Learn

- [ ] P-Value: probability of observing this result (or more extreme) assuming H₀ is true

### Interpretation

- [ ] Small p-value → strong evidence against H₀
- [ ] Large p-value → insufficient evidence against H₀

### Common Mistakes

- [ ] p-value is NOT the probability H₀ is true
- [ ] p-value is NOT the probability the result occurred by chance
- [ ] p-value is NOT effect size
- [ ] Statistical significance ≠ practical significance

**Exercises**
- [ ] Interpret p-values correctly in context

---

## Phase 6: Type I and Type II Errors

### Type I Error (α)

- [ ] False Positive — rejecting H₀ when it's true
- [ ] Consequence: acting on a false finding

### Type II Error (β)

- [ ] False Negative — failing to reject H₀ when it's false
- [ ] Consequence: missing a real effect

### Tradeoffs

- [ ] Reducing α increases β
- [ ] Sensitivity vs Specificity analogy

**Exercises**
- [ ] Medical testing examples (false positive = unnecessary treatment)
- [ ] Fraud detection examples

---

## Phase 7: Statistical Power

### Learn

- [ ] Statistical Power = 1 − β
- [ ] Probability of detecting a real effect when it exists

### Factors Affecting Power

- [ ] Sample Size (larger → higher power)
- [ ] Effect Size (larger → higher power)
- [ ] Variability (lower → higher power)
- [ ] Significance Level (higher α → higher power)

### Understand

- [ ] Underpowered studies miss real effects
- [ ] Power analysis before collecting data (Added)

---

## Phase 8: One-Tailed vs Two-Tailed Tests

### One-Tailed Tests

- [ ] Left-Tailed: testing if parameter < value
- [ ] Right-Tailed: testing if parameter > value

### Two-Tailed Tests

- [ ] Testing if parameter ≠ value (direction unknown)

### Understand

- [ ] One-tailed has more power but requires directional hypothesis
- [ ] Two-tailed is more conservative and more common

---

## Phase 9: Z-Test

### Learn

- [ ] One-Sample Z-Test (sample mean vs known population mean)
- [ ] Two-Sample Z-Test (comparing two means)

### Conditions

- [ ] Known Population Variance
- [ ] Large Sample Size (n ≥ 30)

**Exercises**
- [ ] Business KPI testing (is average order value = $50?)

---

## Phase 10: T-Test

### One-Sample T-Test

- [ ] Sample mean vs hypothesized value, unknown σ

### Independent Samples T-Test

- [ ] Two independent groups compared

### Paired T-Test

- [ ] Before vs after comparisons, matched pairs

### Welch's T-Test (Added)

- [ ] Independent T-Test that doesn't assume equal variances

**Exercises**
- [ ] A/B comparison (control vs treatment)
- [ ] Training effectiveness study (before vs after)

---

## Phase 11: Chi-Square Tests

### Goodness-of-Fit Test

- [ ] Do observed frequencies match expected?

### Test of Independence

- [ ] Are two categorical variables related?

### Conditions (Added)

- [ ] Expected frequency ≥ 5 in each cell

**Exercises**
- [ ] Gender vs Purchase Analysis
- [ ] Marketing channel vs conversion rate

---

## Phase 12: ANOVA

### One-Way ANOVA

- [ ] Compare means across 3+ groups
- [ ] F-statistic: between-group vs within-group variance

### Why Not Multiple T-Tests? (Added)

- [ ] Inflates Type I error (multiple comparison problem)

### Post-Hoc Tests (Added)

- [ ] Tukey HSD
- [ ] Bonferroni correction
- [ ] Which pairs differ significantly?

### Two-Way ANOVA (Added)

- [ ] Two categorical factors and their interaction

**Exercises**
- [ ] Compare 3 marketing campaigns
- [ ] Compare multiple product variants

---

## Phase 13: Correlation Testing

### Learn

- [ ] Testing if correlation is statistically significant

### Methods

- [ ] Pearson Correlation (linear relationships)
- [ ] Spearman Correlation (monotonic relationships, non-parametric)
- [ ] Kendall's Tau (Added — small samples, ties)

---

## Phase 14: Assumptions of Statistical Tests

### Common Assumptions

- [ ] Independence of observations
- [ ] Normality (of data or residuals)
- [ ] Equal Variance (homoscedasticity)

### Diagnostics

- [ ] Shapiro-Wilk test for normality (Added)
- [ ] Levene's test for equal variances (Added)
- [ ] QQ Plots

**Exercises**
- [ ] Validate assumptions before testing

---

## Phase 15: Non-Parametric Tests

### Why They Exist

- [ ] When parametric assumptions are violated
- [ ] Small samples / ordinal data / non-normal distributions

### Tests

| Parametric | Non-Parametric Alternative |
|---|---|
| Independent T-Test | Mann-Whitney U Test |
| Paired T-Test | Wilcoxon Signed-Rank Test |
| One-Way ANOVA | Kruskal-Wallis Test |
| Pearson Correlation | Spearman / Kendall |

---

## Phase 16: Confidence Intervals & Testing

### Learn

- [ ] Confidence Interval: range of plausible values for parameter
- [ ] Relationship: if CI doesn't include H₀ value → reject H₀

**Exercises**
- [ ] Compare CI and p-value approaches (equivalent results)

---

## Phase 17: Effect Size

### Learn

- [ ] Statistical significance tells you IF an effect exists
- [ ] Effect size tells you HOW LARGE it is

### Metrics

- [ ] Cohen's d (mean difference in SD units)
- [ ] Eta-squared η² (for ANOVA)
- [ ] Odds Ratio
- [ ] Relative Risk
- [ ] Cramér's V (Added — for chi-square tests)

### Understand

- [ ] Large samples can make tiny effects statistically significant
- [ ] Always report effect size alongside p-value

---

## Phase 18: Multiple Testing Problem

### Learn

- [ ] Running many tests inflates false positive rate
- [ ] False Discovery Rate (FDR)
- [ ] Family-Wise Error Rate (FWER)

### Corrections

- [ ] Bonferroni Correction (strict, conservative)
- [ ] Benjamini-Hochberg Procedure (Added — controls FDR)

---

## Phase 19: A/B Testing

### Foundations

- [ ] Control Group vs Treatment Group
- [ ] Randomization is essential

### Learn

- [ ] Conversion Rate Testing
- [ ] Experiment Design (pre-registration) (Added)
- [ ] Minimum Detectable Effect (Added)
- [ ] Sample Size Calculation for A/B (Added)

### Understand

- [ ] Peeking problem (stopping early based on results) (Added)
- [ ] Business applications: UI, pricing, marketing

**Exercises**
- [ ] Website optimization experiments

---

## Phase 20: Bayesian vs Frequentist (Added)

### Frequentist (What we've covered)

- [ ] H₀ and p-values
- [ ] Confidence intervals

### Bayesian Testing

- [ ] Prior beliefs updated with evidence
- [ ] Credible intervals
- [ ] Bayes Factor

### Understand

- [ ] When Bayesian approach is preferred
- [ ] Key philosophical differences

---

## Phase 21: Statistical Testing in Python

### SciPy

- [ ] ttest_1samp() / ttest_ind() / ttest_rel()
- [ ] chisquare() / chi2_contingency()
- [ ] mannwhitneyu() / wilcoxon() / kruskal()
- [ ] f_oneway() for ANOVA
- [ ] shapiro() for normality test

### Statsmodels

- [ ] OLS / ANOVA / Confidence Intervals

### Pingouin (Added — clean stats library)

- [ ] ttest() / anova() / pairwise_tests()
- [ ] Effect sizes computed automatically

### Visualization

- [ ] Distribution checking (histograms, QQ plots)
- [ ] Result interpretation plots

---

## Phase 22: Common Mistakes

- [ ] Confusing statistical significance with practical importance
- [ ] Ignoring test assumptions
- [ ] P-hacking (running tests until p < 0.05)
- [ ] Multiple testing without correction
- [ ] Misinterpreting p-values
- [ ] Underpowered studies
- [ ] HARKing: Hypothesizing After Results are Known (Added)
- [ ] Stopping an experiment early (peeking) (Added)

---

## Phase 23: Statistical Decision Framework

### Select the Correct Test

| Scenario | Test |
|---|---|
| One group mean vs value (known σ) | Z-Test |
| One group mean vs value (unknown σ) | One-Sample T-Test |
| Two independent groups, numerical | Independent T-Test / Welch's |
| Before vs after, same subjects | Paired T-Test |
| 3+ groups, numerical | One-Way ANOVA |
| Two categorical variables | Chi-Square Independence |
| One categorical vs expected | Chi-Square Goodness-of-Fit |
| Non-normal / ordinal | Non-Parametric alternatives |

---

## Phase 24: Real Projects

### Beginner
- [ ] Product Rating Analysis
- [ ] Employee Satisfaction Study

### Intermediate
- [ ] Marketing Campaign Comparison
- [ ] Website A/B Test

### Advanced
- [ ] Customer Retention Experiment
- [ ] Clinical Trial Simulation

### Expert
- [ ] End-to-End Experimentation Platform
- [ ] Automated Statistical Reporting System (Added)

---

## Final Mastery

**Can Explain:** Null Hypothesis, Alternative Hypothesis, P-Value, Significance Level, Type I & II Errors, Statistical Power, Confidence Intervals, Effect Size, Z-Test, T-Test, Chi-Square Test, ANOVA, Non-Parametric Tests, A/B Testing, Multiple Testing Problem

**Can Apply:** Choose correct statistical test, check assumptions, interpret p-values and CIs correctly, measure effect size, design and analyze experiments, perform A/B tests, communicate statistical findings to non-technical audiences
