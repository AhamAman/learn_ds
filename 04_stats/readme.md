# Data Types

## Foundations

- [ ] Qualitative vs Quantitative
- [ ] Structured vs Unstructured Data

## Categorical Data

- [ ] Nominal
- [ ] Ordinal

## Numerical Data

- [ ] Discrete
- [ ] Continuous

## Measurement Scales

- [ ] Nominal Scale
- [ ] Ordinal Scale
- [ ] Interval Scale
- [ ] Ratio Scale

## Data Science Applications

- [ ] Choosing the right chart
- [ ] Choosing the right statistic
- [ ] Choosing the right ML feature encoding
- [ ] Identifying data types in datasets

## Can Explain

- [ ] Why average salary makes sense
- [ ] Why average blood group doesn't
- [ ] Why ratings are ordinal
- [ ] Difference between interval and ratio scales

# Sampling Techniques Mastery Checklist

---

# Phase 0: Foundations

## Core Concepts

- [ ] What is a Population?
- [ ] What is a Sample?
- [ ] Population vs Sample
- [ ] Census vs Sampling
- [ ] Sampling Frame
- [ ] Sampling Unit
- [ ] Representativeness

## First Principles

- [ ] Why Sampling Exists
- [ ] Cost vs Accuracy Tradeoff
- [ ] Sample as Population Approximation
- [ ] Sources of Error

---

# Phase 1: Probability Sampling

## Introduction

- [ ] What is Probability Sampling?
- [ ] Why Randomness Matters
- [ ] Equal vs Unequal Selection Probability

---

## Simple Random Sampling (SRS)

### Concepts

- [ ] Simple Random Sampling
- [ ] Sampling With Replacement
- [ ] Sampling Without Replacement

### Understand

- [ ] Equal Selection Probability
- [ ] Advantages
- [ ] Limitations

### Exercises

- [ ] Draw random samples from a dataset
- [ ] Compare multiple random samples

---

## Systematic Sampling

### Concepts

- [ ] Sampling Interval (k)
- [ ] Random Starting Point

### Understand

- [ ] How systematic selection works
- [ ] Hidden pattern risks

### Exercises

- [ ] Build systematic samples
- [ ] Compare with SRS

---

## Stratified Sampling

### Concepts

- [ ] Stratum
- [ ] Stratification Variables

### Types

- [ ] Proportionate Stratified Sampling
- [ ] Disproportionate Stratified Sampling

### Understand

- [ ] Why stratification improves representation
- [ ] Variance reduction

### Exercises

- [ ] Gender-based stratification
- [ ] Region-based stratification

---

## Cluster Sampling

### Concepts

- [ ] Cluster Definition
- [ ] Natural Grouping

### Types

- [ ] One-Stage Cluster Sampling
- [ ] Two-Stage Cluster Sampling

### Understand

- [ ] Cost savings
- [ ] Geographic sampling

### Exercises

- [ ] School survey example
- [ ] City survey example

---

## Multistage Sampling

### Concepts

- [ ] Multiple Sampling Levels
- [ ] Hierarchical Sampling

### Examples

- [ ] Country → State → City → Household

### Understand

- [ ] Real-world survey design

---

# Phase 2: Non-Probability Sampling

## Introduction

- [ ] What is Non-Probability Sampling?
- [ ] Advantages
- [ ] Limitations

---

## Convenience Sampling

### Concepts

- [ ] Easy-access sampling

### Understand

- [ ] Bias risks
- [ ] Common business usage

---

## Judgment (Purposive) Sampling

### Concepts

- [ ] Expert selection
- [ ] Researcher-driven sampling

### Understand

- [ ] Subjectivity

---

## Quota Sampling

### Concepts

- [ ] Category quotas
- [ ] Controlled representation

### Understand

- [ ] Difference from stratified sampling

---

## Snowball Sampling

### Concepts

- [ ] Referral-based sampling

### Use Cases

- [ ] Rare populations
- [ ] Hard-to-reach populations

---

# Phase 3: Sampling Error & Bias

## Sampling Error

- [ ] Definition
- [ ] Sources
- [ ] Sampling Variability

## Sampling Bias

### Types

- [ ] Selection Bias
- [ ] Undercoverage Bias
- [ ] Nonresponse Bias
- [ ] Survivorship Bias
- [ ] Volunteer Bias

### Understand

- [ ] Error vs Bias
- [ ] Why bias is more dangerous

---

# Phase 4: Sample Size Determination

## Concepts

- [ ] Sample Size
- [ ] Margin of Error
- [ ] Confidence Level
- [ ] Population Size

## Understand

- [ ] Sample size tradeoffs
- [ ] Diminishing returns

---

# Phase 5: Sampling Distributions

## Concepts

- [ ] Sampling Distribution
- [ ] Sample Mean Distribution
- [ ] Standard Error

## Understand

- [ ] Why samples differ
- [ ] Foundation for inference

### Exercises

- [ ] Simulate repeated sampling

---

# Phase 6: Central Limit Theorem Connection

## Concepts

- [ ] Central Limit Theorem (CLT)
- [ ] Sample Means
- [ ] Convergence to Normality

## Understand

- [ ] Why CLT matters
- [ ] Why inference works

---

# Phase 7: Survey Design Fundamentals

## Concepts

- [ ] Questionnaire Design
- [ ] Response Bias
- [ ] Measurement Error

## Understand

- [ ] Data quality
- [ ] Survey reliability

---

# Phase 8: Data Science Applications

## Real-World Usage

- [ ] A/B Testing
- [ ] Customer Analytics
- [ ] Market Research
- [ ] Election Polling
- [ ] Recommendation Systems
- [ ] Model Training Data Selection

---

# Phase 9: Python for Sampling

## NumPy

- [ ] random.choice()
- [ ] random.seed()

## Pandas

- [ ] DataFrame.sample()

## Simulations

- [ ] Random sampling experiments
- [ ] Bias demonstrations
- [ ] CLT simulations

---

# Phase 10: Real Projects

## Beginner

- [ ] Student Survey Analysis
- [ ] Product Feedback Analysis

## Intermediate

- [ ] Customer Satisfaction Study
- [ ] Market Research Dataset

## Advanced

- [ ] Election Poll Simulation
- [ ] Sampling Bias Detection System

---

# Final Mastery

Can Explain:

- [ ] Population vs Sample
- [ ] Census vs Sampling
- [ ] Probability vs Non-Probability Sampling
- [ ] Simple Random Sampling
- [ ] Systematic Sampling
- [ ] Stratified Sampling
- [ ] Cluster Sampling
- [ ] Multistage Sampling
- [ ] Sampling Error
- [ ] Sampling Bias
- [ ] Standard Error
- [ ] Sample Size Determination
- [ ] Sampling Distribution
- [ ] CLT Connection

Can Apply:

- [ ] Choose the correct sampling technique
- [ ] Detect biased samples
- [ ] Design representative surveys
- [ ] Estimate population characteristics from samples
- [ ] Evaluate survey quality
- [ ] Build sampling workflows in Python

# Descriptive Statistics Mastery Checklist

---

# Phase 0: Foundations

## Core Concepts

- [ ] What is Statistics?
- [ ] Descriptive vs Inferential Statistics
- [ ] Population
- [ ] Sample
- [ ] Variable
- [ ] Observation
- [ ] Dataset

## Data Types Review

- [ ] Categorical Data
- [ ] Numerical Data
- [ ] Discrete Data
- [ ] Continuous Data
- [ ] Nominal Data
- [ ] Ordinal Data
- [ ] Interval Data
- [ ] Ratio Data

---

# Phase 1: Data Summarization

## Understand

- [ ] Why summarize data?
- [ ] Raw data vs summarized data
- [ ] Distribution overview

## Tabular Summaries

- [ ] Frequency Table
- [ ] Relative Frequency
- [ ] Percentage Distribution
- [ ] Cumulative Frequency

### Exercises

- [ ] Create frequency tables
- [ ] Build category distributions

---

# Phase 2: Measures of Central Tendency

## Mean

- [ ] Arithmetic Mean
- [ ] Weighted Mean

### Understand

- [ ] Interpretation
- [ ] Effect of outliers
- [ ] When mean is useful

### Exercises

- [ ] Calculate averages
- [ ] Compare means across groups

---

## Median

- [ ] Median Calculation
- [ ] Odd-sized datasets
- [ ] Even-sized datasets

### Understand

- [ ] Robustness to outliers
- [ ] Skewed distributions

### Exercises

- [ ] Compare mean vs median

---

## Mode

- [ ] Single Mode
- [ ] Multiple Modes
- [ ] No Mode

### Understand

- [ ] Categorical data applications

### Exercises

- [ ] Identify modal categories

---

## Choosing the Right Measure

- [ ] Mean vs Median
- [ ] Median vs Mode
- [ ] Mean vs Mode
- [ ] When each is appropriate

---

# Phase 3: Measures of Dispersion (Spread)

## Range

- [ ] Minimum
- [ ] Maximum
- [ ] Range

### Understand

- [ ] Sensitivity to outliers

---

## Variance

- [ ] Population Variance
- [ ] Sample Variance

### Understand

- [ ] Average squared deviation
- [ ] Why squaring is used

### Exercises

- [ ] Manual variance calculation

---

## Standard Deviation

- [ ] Population Standard Deviation
- [ ] Sample Standard Deviation

### Understand

- [ ] Variability interpretation
- [ ] Relationship to variance

### Exercises

- [ ] Compare low vs high variability datasets

---

## Interquartile Range (IQR)

- [ ] Quartiles
- [ ] Q1
- [ ] Q2
- [ ] Q3

### Understand

- [ ] Resistant measure of spread
- [ ] Outlier detection

### Exercises

- [ ] Compute IQR manually

---

## Coefficient of Variation

- [ ] Relative variability

### Understand

- [ ] Comparing different scales

---

# Phase 4: Percentiles & Quantiles

## Learn

- [ ] Percentiles
- [ ] Deciles
- [ ] Quartiles
- [ ] Quantiles

### Understand

- [ ] Ranking observations
- [ ] Position within dataset

### Exercises

- [ ] Calculate percentile ranks

---

# Phase 5: Shape of Distribution

## Symmetry

- [ ] Symmetric Distribution
- [ ] Left-Skewed Distribution
- [ ] Right-Skewed Distribution

### Understand

- [ ] Impact on mean and median

---

## Skewness

- [ ] Positive Skewness
- [ ] Negative Skewness

### Exercises

- [ ] Identify skewed datasets

---

## Kurtosis

- [ ] Leptokurtic
- [ ] Mesokurtic
- [ ] Platykurtic

### Understand

- [ ] Tail behavior
- [ ] Extreme values

---

# Phase 6: Outlier Analysis

## Concepts

- [ ] What is an outlier?
- [ ] Sources of outliers

## Detection Methods

- [ ] IQR Method
- [ ] Z-Score Method

### Exercises

- [ ] Detect outliers in datasets

---

# Phase 7: Visualization for Descriptive Statistics

## Histograms

- [ ] Distribution Visualization
- [ ] Bin Selection

### Understand

- [ ] Shape
- [ ] Spread
- [ ] Center

---

## Box Plots

- [ ] Median
- [ ] Quartiles
- [ ] IQR
- [ ] Outliers

### Exercises

- [ ] Interpret box plots

---

## Bar Charts

- [ ] Categorical Frequencies

---

## Density Plots

- [ ] Distribution Estimation

---

## Scatter Plots

- [ ] Relationship Exploration

---

# Phase 8: Five Number Summary

## Learn

- [ ] Minimum
- [ ] Q1
- [ ] Median
- [ ] Q3
- [ ] Maximum

### Understand

- [ ] Distribution overview

### Exercises

- [ ] Build five-number summaries

---

# Phase 9: Standardization

## Learn

- [ ] Standard Score
- [ ] Z-Score

### Widget


::contentReference[oaicite:0]{index=0}


### Understand

- [ ] Relative position
- [ ] Comparing different scales

### Exercises

- [ ] Standardize datasets

---

# Phase 10: Grouped Data Statistics

## Learn

- [ ] Grouped Frequency Tables
- [ ] Class Intervals

### Measures

- [ ] Grouped Mean
- [ ] Grouped Median
- [ ] Grouped Mode

---

# Phase 11: Descriptive Statistics with Python

## NumPy

- [ ] mean()
- [ ] median()
- [ ] std()
- [ ] var()
- [ ] percentile()

---

## Pandas

- [ ] describe()
- [ ] value_counts()
- [ ] quantile()

---

## SciPy

- [ ] skew()
- [ ] kurtosis()

---

# Phase 12: Comparing Distributions

## Learn

- [ ] Compare Centers
- [ ] Compare Spread
- [ ] Compare Shape

### Exercises

- [ ] Analyze multiple datasets

---

# Phase 13: Real-World Applications

## Business Analytics

- [ ] Sales Analysis
- [ ] Customer Analysis
- [ ] Revenue Analysis

## Data Science

- [ ] Exploratory Data Analysis (EDA)
- [ ] Feature Understanding
- [ ] Data Quality Assessment

## Finance

- [ ] Risk Analysis
- [ ] Return Analysis

---

# Phase 14: Common Mistakes

## Understand

- [ ] Mean with highly skewed data
- [ ] Ignoring outliers
- [ ] Confusing variance and standard deviation
- [ ] Correlation assumptions from summary stats
- [ ] Using wrong statistics for categorical data

---

# Phase 15: Real Projects

## Beginner

- [ ] Student Marks Analysis
- [ ] Employee Salary Analysis

## Intermediate

- [ ] Customer Analytics Report
- [ ] Product Sales Report

## Advanced

- [ ] Full Exploratory Data Analysis Report
- [ ] Business KPI Dashboard

---

# Final Mastery

Can Explain:

- [ ] Mean
- [ ] Median
- [ ] Mode
- [ ] Range
- [ ] Variance
- [ ] Standard Deviation
- [ ] IQR
- [ ] Percentiles
- [ ] Quartiles
- [ ] Skewness
- [ ] Kurtosis
- [ ] Outliers
- [ ] Five Number Summary
- [ ] Z-Score

Can Apply:

- [ ] Summarize datasets
- [ ] Compare distributions
- [ ] Detect outliers
- [ ] Choose appropriate summary statistics
- [ ] Perform EDA on real-world data
- [ ] Build descriptive statistical reports

# Descriptive Statistics Mastery Checklist

---

# Phase 0: Foundations

## Core Concepts

- [ ] What is Statistics?
- [ ] Descriptive vs Inferential Statistics
- [ ] Population
- [ ] Sample
- [ ] Variable
- [ ] Observation
- [ ] Dataset

## Data Types Review

- [ ] Categorical Data
- [ ] Numerical Data
- [ ] Discrete Data
- [ ] Continuous Data
- [ ] Nominal Data
- [ ] Ordinal Data
- [ ] Interval Data
- [ ] Ratio Data

---

# Phase 1: Data Summarization

## Understand

- [ ] Why summarize data?
- [ ] Raw data vs summarized data
- [ ] Distribution overview

## Tabular Summaries

- [ ] Frequency Table
- [ ] Relative Frequency
- [ ] Percentage Distribution
- [ ] Cumulative Frequency

### Exercises

- [ ] Create frequency tables
- [ ] Build category distributions

---

# Phase 2: Measures of Central Tendency

## Mean

- [ ] Arithmetic Mean
- [ ] Weighted Mean

### Understand

- [ ] Interpretation
- [ ] Effect of outliers
- [ ] When mean is useful

### Exercises

- [ ] Calculate averages
- [ ] Compare means across groups

---

## Median

- [ ] Median Calculation
- [ ] Odd-sized datasets
- [ ] Even-sized datasets

### Understand

- [ ] Robustness to outliers
- [ ] Skewed distributions

### Exercises

- [ ] Compare mean vs median

---

## Mode

- [ ] Single Mode
- [ ] Multiple Modes
- [ ] No Mode

### Understand

- [ ] Categorical data applications

### Exercises

- [ ] Identify modal categories

---

## Choosing the Right Measure

- [ ] Mean vs Median
- [ ] Median vs Mode
- [ ] Mean vs Mode
- [ ] When each is appropriate

---

# Phase 3: Measures of Dispersion (Spread)

## Range

- [ ] Minimum
- [ ] Maximum
- [ ] Range

### Understand

- [ ] Sensitivity to outliers

---

## Variance

- [ ] Population Variance
- [ ] Sample Variance

### Understand

- [ ] Average squared deviation
- [ ] Why squaring is used

### Exercises

- [ ] Manual variance calculation

---

## Standard Deviation

- [ ] Population Standard Deviation
- [ ] Sample Standard Deviation

### Understand

- [ ] Variability interpretation
- [ ] Relationship to variance

### Exercises

- [ ] Compare low vs high variability datasets

---

## Interquartile Range (IQR)

- [ ] Quartiles
- [ ] Q1
- [ ] Q2
- [ ] Q3

### Understand

- [ ] Resistant measure of spread
- [ ] Outlier detection

### Exercises

- [ ] Compute IQR manually

---

## Coefficient of Variation

- [ ] Relative variability

### Understand

- [ ] Comparing different scales

---

# Phase 4: Percentiles & Quantiles

## Learn

- [ ] Percentiles
- [ ] Deciles
- [ ] Quartiles
- [ ] Quantiles

### Understand

- [ ] Ranking observations
- [ ] Position within dataset

### Exercises

- [ ] Calculate percentile ranks

---

# Phase 5: Shape of Distribution

## Symmetry

- [ ] Symmetric Distribution
- [ ] Left-Skewed Distribution
- [ ] Right-Skewed Distribution

### Understand

- [ ] Impact on mean and median

---

## Skewness

- [ ] Positive Skewness
- [ ] Negative Skewness

### Exercises

- [ ] Identify skewed datasets

---

## Kurtosis

- [ ] Leptokurtic
- [ ] Mesokurtic
- [ ] Platykurtic

### Understand

- [ ] Tail behavior
- [ ] Extreme values

---

# Phase 6: Outlier Analysis

## Concepts

- [ ] What is an outlier?
- [ ] Sources of outliers

## Detection Methods

- [ ] IQR Method
- [ ] Z-Score Method

### Exercises

- [ ] Detect outliers in datasets

---

# Phase 7: Visualization for Descriptive Statistics

## Histograms

- [ ] Distribution Visualization
- [ ] Bin Selection

### Understand

- [ ] Shape
- [ ] Spread
- [ ] Center

---

## Box Plots

- [ ] Median
- [ ] Quartiles
- [ ] IQR
- [ ] Outliers

### Exercises

- [ ] Interpret box plots

---

## Bar Charts

- [ ] Categorical Frequencies

---

## Density Plots

- [ ] Distribution Estimation

---

## Scatter Plots

- [ ] Relationship Exploration

---

# Phase 8: Five Number Summary

## Learn

- [ ] Minimum
- [ ] Q1
- [ ] Median
- [ ] Q3
- [ ] Maximum

### Understand

- [ ] Distribution overview

### Exercises

- [ ] Build five-number summaries

---

# Phase 9: Standardization

## Learn

- [ ] Standard Score
- [ ] Z-Score

### Widget


::contentReference[oaicite:0]{index=0}


### Understand

- [ ] Relative position
- [ ] Comparing different scales

### Exercises

- [ ] Standardize datasets

---

# Phase 10: Grouped Data Statistics

## Learn

- [ ] Grouped Frequency Tables
- [ ] Class Intervals

### Measures

- [ ] Grouped Mean
- [ ] Grouped Median
- [ ] Grouped Mode

---

# Phase 11: Descriptive Statistics with Python

## NumPy

- [ ] mean()
- [ ] median()
- [ ] std()
- [ ] var()
- [ ] percentile()

---

## Pandas

- [ ] describe()
- [ ] value_counts()
- [ ] quantile()

---

## SciPy

- [ ] skew()
- [ ] kurtosis()

---

# Phase 12: Comparing Distributions

## Learn

- [ ] Compare Centers
- [ ] Compare Spread
- [ ] Compare Shape

### Exercises

- [ ] Analyze multiple datasets

---

# Phase 13: Real-World Applications

## Business Analytics

- [ ] Sales Analysis
- [ ] Customer Analysis
- [ ] Revenue Analysis

## Data Science

- [ ] Exploratory Data Analysis (EDA)
- [ ] Feature Understanding
- [ ] Data Quality Assessment

## Finance

- [ ] Risk Analysis
- [ ] Return Analysis

---

# Phase 14: Common Mistakes

## Understand

- [ ] Mean with highly skewed data
- [ ] Ignoring outliers
- [ ] Confusing variance and standard deviation
- [ ] Correlation assumptions from summary stats
- [ ] Using wrong statistics for categorical data

---

# Phase 15: Real Projects

## Beginner

- [ ] Student Marks Analysis
- [ ] Employee Salary Analysis

## Intermediate

- [ ] Customer Analytics Report
- [ ] Product Sales Report

## Advanced

- [ ] Full Exploratory Data Analysis Report
- [ ] Business KPI Dashboard

---

# Final Mastery

Can Explain:

- [ ] Mean
- [ ] Median
- [ ] Mode
- [ ] Range
- [ ] Variance
- [ ] Standard Deviation
- [ ] IQR
- [ ] Percentiles
- [ ] Quartiles
- [ ] Skewness
- [ ] Kurtosis
- [ ] Outliers
- [ ] Five Number Summary
- [ ] Z-Score

Can Apply:

- [ ] Summarize datasets
- [ ] Compare distributions
- [ ] Detect outliers
- [ ] Choose appropriate summary statistics
- [ ] Perform EDA on real-world data
- [ ] Build descriptive statistical reports


# Central Limit Theorem (CLT) Mastery Checklist

---

# Phase 0: Prerequisites

## Statistics Foundations

- [ ] Population
- [ ] Sample
- [ ] Mean
- [ ] Variance
- [ ] Standard Deviation

## Sampling

- [ ] Random Sampling
- [ ] Sampling Error
- [ ] Sampling Bias

## Probability Distributions

- [ ] Normal Distribution
- [ ] Random Variables
- [ ] Probability Distribution

---

# Phase 1: Why CLT Exists

## The Problem

- [ ] Different samples produce different results
- [ ] Sample means vary
- [ ] Need a predictable pattern

## First Principles

- [ ] Population Distribution
- [ ] Sample Distribution
- [ ] Sample Mean

## Understand

- [ ] Why samples differ
- [ ] Why uncertainty exists

---

# Phase 2: Sampling Distribution

## Core Concepts

- [ ] What is a Sampling Distribution?
- [ ] Distribution of Sample Means
- [ ] Distribution of Sample Proportions

## Understand

- [ ] One sample vs many samples
- [ ] Repeated sampling process

### Exercises

- [ ] Draw multiple samples
- [ ] Compare sample means

---

# Phase 3: Central Limit Theorem Fundamentals

## Learn

- [ ] Definition of CLT
- [ ] Conditions for CLT
- [ ] Importance of CLT

## Core Statement

### Understand

- [ ] As sample size increases
- [ ] Sample mean distribution approaches normality
- [ ] Regardless of original population shape

### Key Idea

- [ ] Population can be non-normal
- [ ] Sampling distribution becomes approximately normal

---

# Phase 4: Visual Understanding

## Population Shapes

- [ ] Uniform Population
- [ ] Skewed Population
- [ ] Bimodal Population
- [ ] Exponential Population

## Observe

- [ ] Sample size = 5
- [ ] Sample size = 10
- [ ] Sample size = 30
- [ ] Sample size = 50
- [ ] Sample size = 100

### Exercises

- [ ] Simulate CLT visually

---

# Phase 5: CLT Components

## Population Mean

- [ ] Population Mean (μ)

### Understand

- [ ] Sampling distribution center

---

## Population Standard Deviation

- [ ] Population Standard Deviation (σ)

### Understand

- [ ] Population variability

---

## Sample Size

- [ ] Small Samples
- [ ] Large Samples

### Understand

- [ ] Effect on variability

---

# Phase 6: Standard Error

## Learn

- [ ] Standard Error (SE)

### Formula

:contentReference[oaicite:0]{index=0}

### Understand

- [ ] Standard deviation of sample means
- [ ] Precision of estimates

### Exercises

- [ ] Calculate SE for various sample sizes

---

# Phase 7: Effects of Sample Size

## Learn

- [ ] Increasing sample size
- [ ] Shrinking standard error

## Understand

- [ ] Why larger samples are more stable
- [ ] Why estimates improve

### Exercises

- [ ] Compare n=10 vs n=100 vs n=1000

---

# Phase 8: CLT Conditions

## Required Conditions

- [ ] Random Sampling
- [ ] Independence

## Sample Size Rules

- [ ] n ≥ 30 Rule
- [ ] Large Sample Assumption

## Understand

- [ ] When CLT may fail

---

# Phase 9: CLT for Means

## Learn

- [ ] Sample Mean Distribution

### Properties

- [ ] Mean of Sampling Distribution
- [ ] Standard Error

### Understand

- [ ] Why sample means are normal

---

# Phase 10: CLT for Proportions

## Learn

- [ ] Sample Proportion
- [ ] Proportion Distribution

## Conditions

- [ ] Success-Failure Rule

### Exercises

- [ ] Survey examples
- [ ] Polling examples

---

# Phase 11: CLT Simulations

## Python

### NumPy

- [ ] Generate random populations
- [ ] Draw repeated samples

### Visualization

- [ ] Histograms of sample means

### Exercises

- [ ] Uniform → Normal
- [ ] Exponential → Normal
- [ ] Skewed → Normal

---

# Phase 12: CLT and Normal Distribution

## Relationship

- [ ] Population Distribution
- [ ] Sampling Distribution

## Understand

- [ ] Why normal distribution dominates statistics

### Exercises

- [ ] Compare distributions

---

# Phase 13: CLT and Z-Scores

## Learn

- [ ] Standardization

### Formula

:contentReference[oaicite:1]{index=1}

### Understand

- [ ] Position of sample mean

### Exercises

- [ ] Calculate z-scores for sample means

---

# Phase 14: CLT and Confidence Intervals

## Learn

- [ ] Confidence Intervals

## Understand

- [ ] Why confidence intervals work

### Connection

- [ ] CLT → Normality
- [ ] Normality → Confidence Intervals

---

# Phase 15: CLT and Hypothesis Testing

## Learn

- [ ] Null Hypothesis
- [ ] Alternative Hypothesis

## Understand

- [ ] Why test statistics follow known distributions

### Connection

- [ ] CLT → Test Statistics
- [ ] Test Statistics → P-values

---

# Phase 16: Practical Applications

## Surveys

- [ ] Election Polling
- [ ] Customer Satisfaction Surveys

## Business

- [ ] Sales Estimation
- [ ] Revenue Forecasting

## Data Science

- [ ] Model Evaluation
- [ ] Experiment Analysis

## Machine Learning

- [ ] Sampling Training Data
- [ ] Performance Metrics

---

# Phase 17: Common Misconceptions

## Understand

- [ ] CLT does NOT make data normal
- [ ] CLT applies to sample means
- [ ] n=30 is not a magic number
- [ ] CLT requires proper sampling

### Exercises

- [ ] Identify incorrect CLT claims

---

# Phase 18: Advanced Topics

## Learn

- [ ] Law of Large Numbers (LLN)
- [ ] CLT vs LLN
- [ ] Multivariate CLT

## Understand

- [ ] Statistical foundations

---

# Phase 19: Real Projects

## Beginner

- [ ] Dice Roll Simulation
- [ ] Coin Toss Simulation

## Intermediate

- [ ] Survey Analysis
- [ ] Polling Simulation

## Advanced

- [ ] Confidence Interval Calculator
- [ ] Sampling Distribution Simulator

---

# Final Mastery

Can Explain:

- [ ] Population vs Sample
- [ ] Sampling Distribution
- [ ] Central Limit Theorem
- [ ] Standard Error
- [ ] Effect of Sample Size
- [ ] CLT Conditions
- [ ] CLT for Means
- [ ] CLT for Proportions
- [ ] CLT vs Normal Distribution
- [ ] CLT vs Law of Large Numbers
- [ ] Why Confidence Intervals Work
- [ ] Why Hypothesis Tests Work

Can Apply:

- [ ] Simulate CLT
- [ ] Calculate Standard Error
- [ ] Interpret Sampling Distributions
- [ ] Build Confidence Intervals
- [ ] Perform Statistical Inference
- [ ] Explain CLT in interviews

# Statistical Testing (Hypothesis Testing) Mastery Checklist

---

# Phase 0: Prerequisites

## Statistics Foundations

- [ ] Population
- [ ] Sample
- [ ] Mean
- [ ] Median
- [ ] Variance
- [ ] Standard Deviation

## Probability Foundations

- [ ] Probability
- [ ] Random Variables
- [ ] Normal Distribution
- [ ] Z-Score

## Sampling Foundations

- [ ] Sampling Distribution
- [ ] Central Limit Theorem (CLT)
- [ ] Standard Error

---

# Phase 1: Why Statistical Testing Exists

## The Problem

- [ ] Samples vary naturally
- [ ] Observed differences may occur by chance
- [ ] Need a method to evaluate evidence

## First Principles

- [ ] Signal vs Noise
- [ ] Random Variation
- [ ] Statistical Evidence

## Understand

- [ ] Why intuition is insufficient
- [ ] Why we need formal testing

---

# Phase 2: Hypothesis Fundamentals

## Learn

- [ ] Null Hypothesis (H₀)
- [ ] Alternative Hypothesis (H₁)

## Understand

- [ ] Assume H₀ is true initially
- [ ] Gather evidence against H₀
- [ ] Fail to Reject vs Reject

### Exercises

- [ ] Define hypotheses for business problems
- [ ] Translate questions into hypotheses

---

# Phase 3: Test Statistics

## Learn

- [ ] Test Statistic
- [ ] Standardization

## Common Statistics

- [ ] Z Statistic
- [ ] T Statistic
- [ ] Chi-Square Statistic
- [ ] F Statistic

## Understand

- [ ] Measuring evidence against H₀

---

# Phase 4: Significance Level (α)

## Learn

- [ ] Significance Level

## Common Values

- [ ] 0.10
- [ ] 0.05
- [ ] 0.01

## Understand

- [ ] Decision threshold
- [ ] Risk tolerance

---

# Phase 5: P-Value

## Learn

- [ ] P-Value Definition

## Understand

- [ ] Probability under H₀
- [ ] Evidence strength

## Interpretation

- [ ] Small p-value
- [ ] Large p-value

## Common Mistakes

- [ ] p-value is NOT probability H₀ is true
- [ ] p-value is NOT effect size

### Exercises

- [ ] Interpret p-values correctly

---

# Phase 6: Type I and Type II Errors

## Learn

### Type I Error

- [ ] False Positive

### Type II Error

- [ ] False Negative

## Understand

- [ ] Consequences of each error

## Tradeoffs

- [ ] α vs β
- [ ] Sensitivity vs Specificity

### Exercises

- [ ] Medical testing examples
- [ ] Fraud detection examples

---

# Phase 7: Statistical Power

## Learn

- [ ] Statistical Power

## Understand

- [ ] Probability of detecting real effects
- [ ] Factors affecting power

### Influencing Factors

- [ ] Sample Size
- [ ] Effect Size
- [ ] Variability
- [ ] Significance Level

---

# Phase 8: One-Tailed vs Two-Tailed Tests

## Learn

### One-Tailed Tests

- [ ] Left-Tailed
- [ ] Right-Tailed

### Two-Tailed Tests

- [ ] Bidirectional testing

## Understand

- [ ] When each is appropriate

### Exercises

- [ ] Select proper test direction

---

# Phase 9: Z-Test

## Learn

- [ ] One-Sample Z-Test
- [ ] Two-Sample Z-Test

## Conditions

- [ ] Known Population Variance
- [ ] Large Sample Size

## Applications

- [ ] Population Mean Testing

### Exercises

- [ ] Business KPI testing

---

# Phase 10: T-Test

## Learn

### One-Sample T-Test

- [ ] Sample vs Population

### Independent T-Test

- [ ] Two Independent Groups

### Paired T-Test

- [ ] Before vs After Comparisons

## Understand

- [ ] Unknown Population Variance

### Exercises

- [ ] A/B comparison
- [ ] Training effectiveness study

---

# Phase 11: Chi-Square Tests

## Learn

### Goodness-of-Fit Test

- [ ] Expected vs Observed

### Test of Independence

- [ ] Relationship between categories

## Understand

- [ ] Categorical Data Analysis

### Exercises

- [ ] Gender vs Purchase Analysis

---

# Phase 12: ANOVA

## Learn

- [ ] One-Way ANOVA
- [ ] Multiple Group Comparisons

## Understand

- [ ] Why not multiple T-tests?

### Exercises

- [ ] Compare marketing campaigns
- [ ] Compare multiple products

---

# Phase 13: Correlation Testing

## Learn

- [ ] Correlation Significance

## Methods

- [ ] Pearson Correlation
- [ ] Spearman Correlation

## Understand

- [ ] Statistical significance of relationships

---

# Phase 14: Assumptions of Statistical Tests

## Learn

- [ ] Independence
- [ ] Normality
- [ ] Equal Variance

## Diagnostics

- [ ] Assumption Checking

### Exercises

- [ ] Validate assumptions before testing

---

# Phase 15: Non-Parametric Tests

## Why They Exist

- [ ] Violated assumptions

## Learn

### Mann-Whitney U Test

- [ ] Alternative to Independent T-Test

### Wilcoxon Signed-Rank Test

- [ ] Alternative to Paired T-Test

### Kruskal-Wallis Test

- [ ] Alternative to ANOVA

### Chi-Square

- [ ] Categorical Analysis

---

# Phase 16: Confidence Intervals & Testing

## Learn

- [ ] Confidence Interval Interpretation

## Understand

- [ ] Relationship with hypothesis testing

### Exercises

- [ ] Compare CI and p-value approaches

---

# Phase 17: Effect Size

## Learn

- [ ] Statistical Significance
- [ ] Practical Significance

## Metrics

- [ ] Cohen's d
- [ ] Odds Ratio
- [ ] Relative Risk

## Understand

- [ ] Why significance alone is insufficient

---

# Phase 18: Multiple Testing Problems

## Learn

- [ ] Multiple Comparisons

## Understand

- [ ] False Discovery Rate
- [ ] Family-Wise Error Rate

## Corrections

- [ ] Bonferroni Correction

---

# Phase 19: A/B Testing

## Foundations

- [ ] Control Group
- [ ] Treatment Group

## Learn

- [ ] Conversion Rate Testing
- [ ] Experiment Design

## Understand

- [ ] Business applications

### Exercises

- [ ] Website optimization experiments

---

# Phase 20: Statistical Testing in Python

## SciPy

- [ ] ttest_ind()
- [ ] ttest_rel()
- [ ] chisquare()
- [ ] chi2_contingency()

## Statsmodels

- [ ] ANOVA
- [ ] Confidence Intervals

## Visualization

- [ ] Distribution checking
- [ ] Result interpretation

---

# Phase 21: Common Mistakes

## Understand

- [ ] Confusing significance with importance
- [ ] Ignoring assumptions
- [ ] P-hacking
- [ ] Multiple testing issues
- [ ] Misinterpreting p-values
- [ ] Underpowered studies

---

# Phase 22: Real Projects

## Beginner

- [ ] Product Rating Analysis
- [ ] Employee Satisfaction Study

## Intermediate

- [ ] Marketing Campaign Comparison
- [ ] Website A/B Test

## Advanced

- [ ] Customer Retention Experiment
- [ ] Clinical Trial Simulation

## Expert

- [ ] End-to-End Experimentation Platform

---

# Phase 23: Statistical Decision Framework

## Can Select Correct Test

### Numerical Data

- [ ] One Group → T-Test
- [ ] Two Groups → T-Test
- [ ] Multiple Groups → ANOVA

### Categorical Data

- [ ] Chi-Square Tests

### Non-Normal Data

- [ ] Non-Parametric Alternatives

---

# Final Mastery

Can Explain:

- [ ] Null Hypothesis
- [ ] Alternative Hypothesis
- [ ] P-Value
- [ ] Significance Level
- [ ] Type I Error
- [ ] Type II Error
- [ ] Statistical Power
- [ ] Confidence Intervals
- [ ] Effect Size
- [ ] Z-Test
- [ ] T-Test
- [ ] Chi-Square Test
- [ ] ANOVA
- [ ] Non-Parametric Tests
- [ ] A/B Testing

Can Apply:

- [ ] Choose correct statistical test
- [ ] Check assumptions
- [ ] Interpret p-values correctly
- [ ] Interpret confidence intervals
- [ ] Measure effect size
- [ ] Analyze experiments
- [ ] Perform A/B tests
- [ ] Communicate statistical findings

