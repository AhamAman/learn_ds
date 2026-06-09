# Machine Learning Mastery Checklists

> A complete, phase-by-phase learning roadmap covering core ML concepts, algorithms, and techniques.

---

## Table of Contents

1. [Machine Learning Introduction](#1-machine-learning-introduction)
2. [Linear Regression & Gradient Descent](#2-linear-regression--gradient-descent)
3. [Regularization](#3-regularization)
4. [Logistic Regression](#4-logistic-regression)
5. [Decision Trees](#5-decision-trees)
6. [Random Forest](#6-random-forest)
7. [K-Nearest Neighbors (KNN)](#7-k-nearest-neighbors-knn)
8. [Stacking & Boosting](#8-stacking--boosting)
9. [AdaBoost](#9-adaboost)
10. [Gradient Boosting](#10-gradient-boosting)
11. [XGBoost](#11-xgboost)
12. [Dimensionality Reduction](#12-dimensionality-reduction)
13. [Naive Bayes](#13-naive-bayes)
14. [Support Vector Machine (SVM)](#14-support-vector-machine-svm)
15. [Hierarchical Clustering](#15-hierarchical-clustering)
16. [DBSCAN](#16-dbscan)

---

# 1. Machine Learning Introduction

## Phase 0: Foundations

### Prerequisites

- [ ] Python
- [ ] NumPy
- [ ] Pandas
- [ ] Matplotlib
- [ ] Seaborn
- [ ] Statistics
- [ ] Probability
- [ ] Hypothesis Testing
- [ ] EDA

### Mathematical Foundations

- [ ] Basic Algebra
- [ ] Functions
- [ ] Coordinates
- [ ] Gradients (Basic Intuition)

---

## Phase 1: Why Machine Learning Exists

### The Problem

- [ ] Rule-Based Systems
- [ ] Limitations of Hard-Coded Logic
- [ ] Pattern Recognition Problems

### First Principles

- [ ] What is Learning?
- [ ] What is Intelligence?
- [ ] What is Prediction?

### Understand

- [ ] Programming vs Machine Learning
- [ ] Explicit Rules vs Learned Rules

### Examples

- [ ] Spam Detection
- [ ] House Price Prediction
- [ ] Recommendation Systems
- [ ] Fraud Detection

---

## Phase 2: Machine Learning Workflow

### Big Picture

- [ ] Problem Definition
- [ ] Data Collection
- [ ] Data Cleaning
- [ ] Feature Engineering
- [ ] Model Training
- [ ] Model Evaluation
- [ ] Deployment
- [ ] Monitoring

### Understand

- [ ] End-to-End ML Lifecycle

---

## Phase 3: Types of Machine Learning

### Supervised Learning

**Learn**
- [ ] Labeled Data
- [ ] Input Features
- [ ] Target Variable

**Problems**
- [ ] Classification
- [ ] Regression

### Unsupervised Learning

**Learn**
- [ ] Unlabeled Data

**Problems**
- [ ] Clustering
- [ ] Dimensionality Reduction

### Reinforcement Learning

**Learn**
- [ ] Agent
- [ ] Environment
- [ ] Reward

**Understand**
- [ ] Learning by Interaction

---

## Phase 4: Data in Machine Learning

### Learn

- [ ] Features
- [ ] Labels
- [ ] Samples
- [ ] Dataset

### Dataset Structure

- [ ] Rows
- [ ] Columns
- [ ] X (Features)
- [ ] y (Target)

### Exercises

- [ ] Identify features and target

---

## Phase 5: Feature Engineering Fundamentals

### Learn

- [ ] Raw Features
- [ ] Engineered Features

### Data Preparation

- [ ] Encoding Categorical Variables
- [ ] Scaling Numerical Variables
- [ ] Handling Missing Values

### Exercises

- [ ] Prepare Superstore dataset

---

## Phase 6: Train-Test Split

### Learn

- [ ] Training Data
- [ ] Testing Data

### Concepts

- [ ] Why evaluate on unseen data
- [ ] Data Leakage
- [ ] Generalization

### Exercises

- [ ] Split datasets properly

---

## Phase 7: Regression Problems

### Learn

- [ ] Predict Continuous Values
- [ ] Input → Number

### Examples

- [ ] House Prices
- [ ] Revenue Prediction
- [ ] Sales Forecasting

---

## Phase 8: Classification Problems

### Learn

- [ ] Predict Categories
- [ ] Input → Class

### Examples

- [ ] Spam Detection
- [ ] Fraud Detection
- [ ] Customer Churn

---

## Phase 9: Machine Learning Metrics

### Regression Metrics

- [ ] MAE
- [ ] MSE
- [ ] RMSE
- [ ] R²
- [ ] Prediction Error (concept)

### Classification Metrics

- [ ] Accuracy
- [ ] Precision
- [ ] Recall
- [ ] F1 Score
- [ ] Confusion Matrix (concept)

---

## Phase 10: Overfitting & Underfitting

### Learn

- [ ] Overfitting
- [ ] Underfitting
- [ ] Memorization vs Learning
- [ ] Bias vs Variance

### Exercises

- [ ] Identify overfit models

---

## Phase 11: Cross Validation

### Learn

- [ ] Validation Set
- [ ] K-Fold Cross Validation
- [ ] Reliable model evaluation

### Exercises

- [ ] Compare model performance

---

## Phase 12: Scikit-Learn Fundamentals

### Learn

- [ ] scikit-learn ecosystem
- [ ] fit()
- [ ] predict()
- [ ] transform()

### Exercises

- [ ] First ML pipeline

---

## Phase 13: Machine Learning Pipelines

### Learn

- [ ] Pipeline Concept
- [ ] Preprocessing
- [ ] Feature Engineering
- [ ] Model
- [ ] Reproducibility

---

## Phase 14: Feature Scaling

### Learn

- [ ] Standardization
- [ ] Normalization
- [ ] Distance-Based Algorithms

### Exercises

- [ ] Scale datasets

---

## Phase 15: Data Leakage

### Learn

- [ ] Leakage Definition
- [ ] Target Leakage
- [ ] Train-Test Contamination

### Exercises

- [ ] Detect leakage scenarios

---

## Phase 16: Model Selection

### Learn

- [ ] Baseline Model
- [ ] Candidate Models
- [ ] Simplicity vs Complexity

### Exercises

- [ ] Compare multiple models

---

## Phase 17: Explainability

### Learn

- [ ] Feature Importance
- [ ] Why predictions happen
- [ ] Interpretability vs Explainability

---

## Phase 18: Business Thinking

### Learn

- [ ] Business Objective
- [ ] Technical Metric
- [ ] Business Metric
- [ ] Accuracy is not always enough

### Exercises

- [ ] Connect models to business goals

---

## Phase 19: Production Mindset

### Learn

- [ ] Training
- [ ] Serving
- [ ] Monitoring
- [ ] Model Drift
- [ ] Data Drift

---

## Phase 20: Real Projects

### Beginner

- [ ] House Price Prediction
- [ ] Student Score Prediction

### Intermediate

- [ ] Customer Churn Prediction
- [ ] Sales Forecasting

### Advanced

- [ ] Fraud Detection System
- [ ] Recommendation Prototype

---

## Phase 21: ML Algorithm Roadmap

### Regression Algorithms

- [ ] Linear Regression
- [ ] Polynomial Regression

### Classification Algorithms

- [ ] Logistic Regression
- [ ] Decision Trees
- [ ] Random Forest

### Unsupervised Algorithms

- [ ] K-Means
- [ ] PCA

### Deep Learning Preview

- [ ] Neural Networks
- [ ] Deep Learning Overview

---

## Final Mastery

**Can Explain:**
- [ ] What Machine Learning Is
- [ ] Why Machine Learning Exists
- [ ] Supervised / Unsupervised / Reinforcement Learning
- [ ] Features vs Labels
- [ ] Train/Test Split
- [ ] Evaluation Metrics
- [ ] Overfitting & Underfitting
- [ ] Cross Validation
- [ ] Data Leakage
- [ ] ML Pipeline

**Can Build:**
- [ ] End-to-End ML Workflow
- [ ] Data Preparation Pipeline
- [ ] Model Evaluation Pipeline
- [ ] Business-Oriented ML Solution

---

# 2. Linear Regression & Gradient Descent

## Phase 0: Prerequisites

### Machine Learning Foundations

- [ ] Features (X) / Target (y)
- [ ] Training Data / Test Data
- [ ] Regression Problems

### Statistics Foundations

- [ ] Mean, Variance, Correlation
- [ ] Scatter Plots

### Math Foundations

- [ ] Functions, Coordinates, Slope
- [ ] Basic Algebra

---

## Phase 1: Why Linear Regression Exists

### The Problem

- [ ] Predict numerical values
- [ ] Estimate future outcomes
- [ ] Find relationships between variables

### Examples

- [ ] House Price Prediction
- [ ] Salary Prediction
- [ ] Sales / Revenue Forecasting

### First Principles

- [ ] Inputs affect outputs
- [ ] Relationship discovery
- [ ] Pattern learning

---

## Phase 2: Understanding Relationships

### Learn

- [ ] Independent Variable
- [ ] Dependent Variable

### Visual Analysis

- [ ] Scatter Plot
- [ ] Positive / Negative / No Relationship

### Exercises

- [ ] Plot real datasets and interpret relationships

---

## Phase 3: Correlation Foundations

### Learn

- [ ] Positive / Negative / Zero Correlation
- [ ] Correlation ≠ Causation

### Exercises

- [ ] Correlation analysis

---

## Phase 4: Best Fit Line Intuition

### Learn

- [ ] Line through data points
- [ ] Best Fit Concept
- [ ] Why a single line?

### Exercises

- [ ] Draw best-fit lines manually

---

## Phase 5: Linear Equation Foundations

### Learn

- [ ] Slope-Intercept Form: y = mx + b
- [ ] Slope (m) and Intercept (b)
- [ ] Prediction using a line

### Exercises

- [ ] Calculate predictions manually
- [ ] Interpret slope

---

## Phase 6: ML Version of Linear Regression

### Learn

- [ ] Single Feature Model: ŷ = w·x + b
- [ ] Weight (w), Bias (b), Predicted Value (ŷ)

### Exercises

- [ ] Predict using learned weights

---

## Phase 7: Errors & Residuals

### Learn

- [ ] Actual Value vs Predicted Value
- [ ] Residual = Actual − Predicted
- [ ] Why predictions are imperfect

### Exercises

- [ ] Compute residuals manually

---

## Phase 8: Cost Function Intuition

### Learn

- [ ] Model Error
- [ ] Cost Function: Lower cost = better model
- [ ] Need to measure "badness"

### Exercises

- [ ] Compare multiple candidate lines

---

## Phase 9: Mean Squared Error (MSE)

### Learn

- [ ] MSE = (1/n) Σ(y − ŷ)²
- [ ] Squaring errors penalizes large mistakes

### Exercises

- [ ] Compute MSE manually

---

## Phase 10: Optimization Problem

### Learn

- [ ] Many possible lines → need best line
- [ ] Minimization
- [ ] Optimization: Search for lowest cost

---

## Phase 11: Gradient Fundamentals

### Learn

- [ ] Gradient / Derivative
- [ ] Slope of a curve
- [ ] Direction of steepest increase
- [ ] Why gradients matter

### Exercises

- [ ] Visualize slopes

---

## Phase 12: Gradient Descent Intuition

### Learn

- [ ] Hill Analogy / Downhill Movement
- [ ] Move opposite gradient
- [ ] Repeated improvement

### Exercises

- [ ] Simulate gradient descent manually

---

## Phase 13: Gradient Descent Algorithm

### Learn

- [ ] Update Rule: w = w − α · ∇L
- [ ] Learning Rate (α)
- [ ] Gradient and Weight Update
- [ ] Iterative optimization

---

## Phase 14: Learning Rate

### Learn

- [ ] Learning Rate (α)
- [ ] Too small → slow learning
- [ ] Too large → overshooting
- [ ] Good rate → efficient convergence

### Exercises

- [ ] Compare learning rates

---

## Phase 15: Convergence

### Learn

- [ ] Convergence
- [ ] Local vs Global minimum (intuition)

### Exercises

- [ ] Track cost reduction

---

## Phase 16: Types of Gradient Descent

### Variants

- [ ] Batch Gradient Descent (entire dataset)
- [ ] Stochastic Gradient Descent (one sample)
- [ ] Mini-Batch Gradient Descent (small batches)
- [ ] Tradeoffs between each

---

## Phase 17: Multiple Linear Regression

### Learn

- [ ] Multiple Features: ŷ = w₁x₁ + w₂x₂ + ... + b
- [ ] Multiple predictors / feature contributions

### Exercises

- [ ] Multi-feature prediction

---

## Phase 18: Model Evaluation

### Metrics

- [ ] MAE, MSE, RMSE, R² Score

### Exercises

- [ ] Evaluate models

---

## Phase 19: Assumptions of Linear Regression

- [ ] Linearity
- [ ] Independence
- [ ] Constant Variance (Homoscedasticity)
- [ ] Normal Residuals
- [ ] When regression works well

---

## Phase 20: Failure Modes

- [ ] Underfitting / Overfitting
- [ ] Outlier Sensitivity
- [ ] Multicollinearity

### Exercises

- [ ] Diagnose problems

---

## Phase 21: Scikit-Learn Implementation

### Learn

- [ ] LinearRegression()
- [ ] fit() / predict() / score()

### Exercises

- [ ] House price model
- [ ] Salary prediction model

---

## Phase 22: Build From Scratch

### Implement

- [ ] MSE from scratch
- [ ] Gradient calculation
- [ ] Gradient Descent
- [ ] Linear Regression

---

## Phase 23: Real Projects

### Beginner

- [ ] Student Score Prediction
- [ ] Salary Prediction

### Intermediate

- [ ] House Price Prediction
- [ ] Sales Forecasting

### Advanced

- [ ] Multiple Regression Project
- [ ] Business Revenue Prediction

---

## Final Mastery

**Can Explain:** Linear Regression, Best Fit Line, Residuals, MSE, Cost Function, Optimization, Gradient, Gradient Descent, Learning Rate, Convergence, Batch vs SGD vs Mini-Batch, Multiple Linear Regression, Regression Assumptions

**Can Build:** Linear Regression from Scratch, Gradient Descent from Scratch, Regression Models in Scikit-Learn, Business Prediction Systems

---

# 3. Regularization

## Phase 0: Prerequisites

### Machine Learning Foundations

- [ ] Features, Target Variable, Training/Testing Data

### Linear Regression

- [ ] Best Fit Line, Cost Function, MSE, Gradient Descent, Multiple Linear Regression

### Evaluation

- [ ] Train Error, Test Error, Generalization

---

## Phase 1: Why Regularization Exists

### The Problem

- [ ] Overfitting / Memorization vs Learning / Poor Generalization

### First Principles

- [ ] Simple vs Complex Models
- [ ] Occam's Razor
- [ ] Why complexity can hurt performance

### Exercises

- [ ] Compare underfit vs overfit models

---

## Phase 2: Bias-Variance Tradeoff

### Learn

- [ ] Bias → Underfitting
- [ ] Variance → Overfitting
- [ ] Goal: Balance bias and variance

### Exercises

- [ ] Identify bias/variance scenarios

---

## Phase 3: Complexity in Linear Models

### Learn

- [ ] Model Complexity
- [ ] Feature Explosion
- [ ] Large Coefficients
- [ ] Why large weights are risky

### Exercises

- [ ] Analyze coefficient growth

---

## Phase 4: Introduction to Regularization

### Learn

- [ ] Regularization Concept
- [ ] Penalty Term
- [ ] Penalize complexity → Better generalization

### Exercises

- [ ] Compare regularized vs non-regularized models

---

## Phase 5: Cost Function with Regularization

### Learn

- [ ] Original Cost Function + Penalty Term
- [ ] Objective Function / Optimization with Constraints

---

## Phase 6: Ridge Regression (L2)

### Learn

- [ ] Ridge Regression / L2 Regularization
- [ ] Formula: Cost + λ·Σw²
- [ ] Shrinks weights, keeps all features
- [ ] Reduced variance, better stability

### Exercises

- [ ] Train Ridge models, compare coefficient shrinkage

---

## Phase 7: Lasso Regression (L1)

### Learn

- [ ] Lasso Regression / L1 Regularization
- [ ] Formula: Cost + λ·Σ|w|
- [ ] Forces coefficients to zero → automatic feature selection
- [ ] Sparse, simpler models

### Exercises

- [ ] Observe feature elimination

---

## Phase 8: Ridge vs Lasso

| | Ridge | Lasso |
|---|---|---|
| Weight Shrinkage | Yes | Yes |
| Feature Selection | No | Yes |
| Stability | Higher | Lower |
| Zeros | No | Yes |

### Exercises

- [ ] Compare outputs on same dataset

---

## Phase 9: Elastic Net

### Learn

- [ ] Elastic Net = L1 + L2 combination
- [ ] Best of Ridge and Lasso
- [ ] Feature selection + stability

### Exercises

- [ ] Compare with Ridge and Lasso

---

## Phase 10: Regularization Strength (Lambda)

### Learn

- [ ] Lambda (λ): controls penalty strength
- [ ] Small λ → weak regularization
- [ ] Large λ → strong regularization, underfitting risk

### Exercises

- [ ] Tune lambda values

---

## Phase 11: Feature Scaling and Regularization

### Learn

- [ ] Standardization / Normalization
- [ ] Scaling is essential for regularization

### Exercises

- [ ] Ridge/Lasso with and without scaling

---

## Phase 12: Geometry Intuition

- [ ] Ridge: Circular constraint
- [ ] Lasso: Diamond constraint — why Lasso creates zeros

### Exercises

- [ ] Visualize parameter space

---

## Phase 13: Hyperparameter Tuning

### Learn

- [ ] Grid Search / Cross Validation
- [ ] Selecting optimal lambda

### Exercises

- [ ] Tune Ridge and Lasso models

---

## Phase 14: Regularization in Practice

### Use Cases

- [ ] Multicollinearity
- [ ] High-Dimensional Data
- [ ] Noisy / Correlated Features

### Exercises

- [ ] Real-world datasets

---

## Phase 15: Scikit-Learn Implementation

- [ ] Ridge() / Lasso() / ElasticNet()
- [ ] fit() / predict() / score()

### Exercises

- [ ] End-to-end regularized regression

---

## Phase 16: Failure Modes

- [ ] Over-Regularization → Excessive bias
- [ ] Under-Regularization → Insufficient control

### Exercises

- [ ] Diagnose poor tuning

---

## Phase 17: Connections to Deep Learning

- [ ] Weight Decay
- [ ] Regularization in Neural Networks

---

## Phase 18: Real Projects

### Beginner → Housing Price Prediction
### Intermediate → Customer Revenue Prediction
### Advanced → High-Dimensional Regression
### Expert → Automated Model Selection Pipeline

---

## Final Mastery

**Can Explain:** Overfitting, Bias-Variance Tradeoff, Regularization, Ridge, Lasso, Elastic Net, Lambda, Feature Selection, Coefficient Shrinkage, Why Scaling Matters

**Can Apply:** Reduce Overfitting, Tune Lambda, Select Features, Compare Ridge/Lasso/ElasticNet, Build Robust Regression Models

---

# 4. Logistic Regression

## Phase 0: Prerequisites

### Machine Learning Foundations

- [ ] Features (X) / Target (y)
- [ ] Train/Test Split / Cross Validation

### Statistics Foundations

- [ ] Probability, Conditional Probability, Odds, Logarithms

### Linear Regression Foundations

- [ ] Best Fit Line, Cost Function, Gradient Descent, Regularization, Overfitting vs Underfitting

---

## Phase 1: Why Logistic Regression Exists

### The Problem

Linear Regression predicts continuous values (prices, revenue, temperature).
Many real-world problems require category prediction (spam, fraud, churn, disease).

### First Principles

- [ ] Regression: Input → Number
- [ ] Classification: Input → Category
- [ ] Why Linear Regression fails for classification
- [ ] Why outputs must be probabilities

---

## Phase 2: Probability Thinking

### Learn

- [ ] Probability as confidence (0 to 1)
- [ ] Likelihood

### Exercises

- [ ] Interpret prediction probabilities

---

## Phase 3: Odds and Log Odds

### Odds

- [ ] Odds Definition
- [ ] Probability vs Odds
- [ ] Examples: sports betting, risk estimation

### Log Odds

- [ ] Logit Function
- [ ] Why transform probabilities

### Exercises

- [ ] Convert probability → odds → log odds

---

## Phase 4: Sigmoid Function

### Learn

- [ ] σ(z) = 1 / (1 + e⁻ᶻ)
- [ ] S-Shaped Curve, maps values to 0–1
- [ ] Properties: output range, smoothness, differentiability

### Exercises

- [ ] Plot sigmoid curve and analyze outputs

---

## Phase 5: Logistic Regression Model

### Learn

- [ ] ŷ = σ(w·x + b)
- [ ] Weights, Bias, Probability prediction

### Exercises

- [ ] Manual probability calculations

---

## Phase 6: Decision Boundary

### Learn

- [ ] Classification Threshold
- [ ] P > 0.5 → Class 1 / P < 0.5 → Class 0
- [ ] Decision boundary as separation line

### Exercises

- [ ] Adjust thresholds and observe classification changes

---

## Phase 7: Cost Function Intuition

### Learn

- [ ] Why MSE is problematic (non-convex, poor learning)
- [ ] Need: likelihood-based optimization

---

## Phase 8: Log Loss (Binary Cross Entropy)

### Learn

- [ ] Log Loss = −(1/n) Σ [y·log(ŷ) + (1−y)·log(1−ŷ)]
- [ ] Punishes confident wrong predictions
- [ ] Rewards confident correct predictions

### Exercises

- [ ] Calculate log loss manually

---

## Phase 9: Maximum Likelihood Estimation (MLE)

### Learn

- [ ] Likelihood / Maximum Likelihood
- [ ] Why logistic regression uses MLE
- [ ] Relationship with log loss

---

## Phase 10: Gradient Descent in Logistic Regression

### Learn

- [ ] Optimization process: weight updates, loss minimization

### Exercises

- [ ] Visualize training process

---

## Phase 11: Binary Classification

### Examples

- [ ] Spam Detection / Customer Churn / Fraud Detection

### Exercises

- [ ] Build binary classifiers

---

## Phase 12: Evaluation Metrics

### Accuracy

- [ ] Definition, Strengths, Weaknesses

### Confusion Matrix

- [ ] True Positive / True Negative / False Positive / False Negative

### Precision, Recall, F1 Score

- [ ] Definitions and use cases
- [ ] Precision-Recall balance

### ROC-AUC

- [ ] ROC Curve / AUC Score

### Exercises

- [ ] Evaluate multiple models

---

## Phase 13: Threshold Tuning

### Learn

- [ ] Threshold Selection
- [ ] Precision vs Recall Tradeoff

### Exercises

- [ ] Compare thresholds

---

## Phase 14: Class Imbalance

### Learn

- [ ] Imbalanced Datasets (fraud, disease detection)
- [ ] Accuracy trap
- [ ] Techniques: Class Weighting, Oversampling, Undersampling

---

## Phase 15: Regularized Logistic Regression

### Learn

- [ ] Ridge Logistic Regression (L2)
- [ ] Lasso Logistic Regression (L1)
- [ ] Overfitting prevention

### Exercises

- [ ] Compare regularization strengths

---

## Phase 16: Multiclass Logistic Regression

### Learn

- [ ] One-vs-Rest (OvR)
- [ ] Softmax Regression

### Exercises

- [ ] Multi-class classification

---

## Phase 17: Feature Engineering for Logistic Regression

### Learn

- [ ] Feature Scaling / Categorical Encoding
- [ ] Impact on model performance

### Exercises

- [ ] Build preprocessing pipelines

---

## Phase 18: Assumptions of Logistic Regression

- [ ] Independent Observations
- [ ] Low Multicollinearity
- [ ] Linear Relationship with Log Odds

---

## Phase 19: Failure Modes

- [ ] Underfitting / Overfitting / Multicollinearity / Poor Feature Engineering

### Exercises

- [ ] Diagnose bad models

---

## Phase 20: Scikit-Learn Implementation

### Learn

- [ ] LogisticRegression()
- [ ] fit() / predict() / predict_proba()

### Exercises

- [ ] Spam Detection / Churn Prediction

---

## Phase 21: Build from Scratch

### Implement

- [ ] Sigmoid Function
- [ ] Log Loss
- [ ] Gradient Descent
- [ ] Binary Classifier

---

## Phase 22: Real Projects

### Beginner → Student Pass/Fail, Loan Approval
### Intermediate → Customer Churn, Email Spam Detection
### Advanced → Fraud Detection, Medical Risk Prediction

---

## Phase 23: Interview Readiness

**Can Explain:** Why Logistic Regression is called regression, Sigmoid Function, Odds and Log Odds, Log Loss, MLE, Decision Boundary, Precision vs Recall, ROC-AUC, Class Imbalance, Regularized Logistic Regression

**Can Compare:** Linear vs Logistic Regression, Accuracy vs F1, Precision vs Recall, Logistic Regression vs Decision Tree

**Can Build:** End-to-End Classification Pipeline, Feature Engineering Pipeline, Production-Ready Binary Classifier

---

# 5. Decision Trees

## Phase 0: Prerequisites

### Machine Learning Foundations

- [ ] Features (X) / Target (y)
- [ ] Train/Test Split / Cross Validation

### Statistics Foundations

- [ ] Probability / Conditional Probability / Entropy Intuition

### Previous ML Models

- [ ] Linear Regression / Logistic Regression / Classification Metrics

---

## Phase 1: Why Decision Trees Exist

### The Problem

Linear models assume linear relationships and struggle with complex rules.
Real-world problems need non-linear patterns and rule-based decisions.

### Examples

- [ ] Loan Approval / Customer Churn / Fraud Detection / Medical Diagnosis

### First Principles

- [ ] Trees mimic human reasoning
- [ ] Trees learn rules from data

---

## Phase 2: Anatomy of a Decision Tree

### Learn

- [ ] Root Node / Internal Node / Branch / Leaf Node
- [ ] Decision Path / Prediction Flow

### Exercises

- [ ] Draw trees manually, trace prediction paths

---

## Phase 3: Classification Trees

### Learn

- [ ] Predicting categories

### Examples

- [ ] Spam Detection / Disease Detection / Customer Churn

---

## Phase 4: Regression Trees

### Learn

- [ ] Predicting continuous values

### Examples

- [ ] House Prices / Revenue Prediction

---

## Phase 5: How Trees Learn

### Core Question

At each node: Which feature to split on? Where to split?

- [ ] Goal: Create pure groups

---

## Phase 6: Entropy

### Learn

- [ ] Disorder / Uncertainty / Impurity
- [ ] Pure Node: all same class
- [ ] Impure Node: mixed classes
- [ ] Lower entropy = better

### Exercises

- [ ] Compare pure vs impure nodes

---

## Phase 7: Information Gain

### Learn

- [ ] Information Gain: reduction in uncertainty
- [ ] Parent Entropy, Child Entropy, Gain Calculation

### Exercises

- [ ] Rank split quality

---

## Phase 8: Gini Impurity

### Learn

- [ ] Gini Impurity: alternative to entropy, faster computation

### Exercises

- [ ] Analyze split quality, compare Entropy vs Gini

---

## Phase 9: Splitting Strategies

### Numerical Features

- [ ] Threshold Splits (e.g., Age > 30)

### Categorical Features

- [ ] Category-based splits

### Exercises

- [ ] Design split rules

---

## Phase 10: Tree Growth

### Learn

- [ ] Recursive Splitting
- [ ] Trees grow top-down (greedy optimization)

### Exercises

- [ ] Build tree manually

---

## Phase 11: Leaf Predictions

### Classification → Majority Class
### Regression → Mean Value

---

## Phase 12: Overfitting in Trees

### Learn

- [ ] Deep Trees / Memorization
- [ ] Perfect training accuracy, poor test performance
- [ ] High variance problem

---

## Phase 13: Tree Pruning

### Learn

- [ ] Pre-Pruning / Post-Pruning
- [ ] max_depth / min_samples_split / min_samples_leaf

### Exercises

- [ ] Tune tree depth

---

## Phase 14: Hyperparameters

- [ ] max_depth / min_samples_split / min_samples_leaf / max_features

### Exercises

- [ ] Hyperparameter tuning

---

## Phase 15: Feature Importance

### Learn

- [ ] Feature Importance Scores
- [ ] Which variables matter most

### Exercises

- [ ] Interpret feature rankings

---

## Phase 16: Evaluation Metrics

### Classification: Accuracy, Precision, Recall, F1 Score, ROC-AUC
### Regression: MAE, MSE, RMSE, R²

### Exercises

- [ ] Evaluate tree performance

---

## Phase 17: Visualizing Trees

### Learn

- [ ] Tree Diagrams / Reading learned rules

### Exercises

- [ ] Explain model decisions

---

## Phase 18: Decision Tree Assumptions

- [ ] No scaling required
- [ ] No normality assumption
- [ ] Handles non-linear data
- [ ] Advantages: Interpretability, Flexibility

---

## Phase 19: Failure Modes

- [ ] Overfitting / Unstable Trees / Data Sensitivity

### Exercises

- [ ] Diagnose instability

---

## Phase 20: Scikit-Learn Implementation

### Learn

- [ ] DecisionTreeClassifier() / DecisionTreeRegressor()
- [ ] fit() / predict() / score()

### Exercises

- [ ] Churn Prediction / House Price Prediction

---

## Phase 21: Build From Scratch

### Implement

- [ ] Entropy / Information Gain / Gini Impurity
- [ ] Recursive Splitting / Tree Construction

---

## Phase 22: Business Applications

### Classification: Fraud Detection, Credit Risk, Customer Churn
### Regression: Sales Forecasting, Revenue Prediction

---

## Phase 23: Interview Readiness

**Can Explain:** Decision Tree, Entropy, Information Gain, Gini Impurity, Tree Growth, Pruning, Feature Importance, Overfitting, Hyperparameters

**Can Compare:** Logistic Regression vs Decision Tree, Entropy vs Gini, Classification Tree vs Regression Tree

**Can Build:** Decision Tree from Scratch, Production Tree Model, Interpretable ML Pipeline

---

## Phase 24: Transition to Ensemble Learning

### Why Single Trees Are Limited

- [ ] High Variance / Instability / Overfitting

---

# 6. Random Forest

## Phase 0: Prerequisites

### Decision Tree Foundations

- [ ] Tree Structure, Entropy, Information Gain, Gini Impurity, Tree Growth, Pruning

### Machine Learning Foundations

- [ ] Overfitting/Underfitting, Bias/Variance, Train/Test Split, Cross Validation

---

## Phase 1: Why Random Forest Exists

### The Problem

Single Decision Trees: overfit easily, high variance, unstable predictions.

### First Principles — Wisdom of Crowds

One doctor can be wrong. 100 doctors aggregating opinions → usually better.

### Understand

- [ ] One tree is fragile; many trees are more reliable

---

## Phase 2: Ensemble Learning Introduction

### Learn

- [ ] Ensemble Learning: combining multiple models
- [ ] Types: Bagging, Boosting, Stacking

---

## Phase 3: Bagging Foundations

### Learn

- [ ] Bootstrap Aggregating
- [ ] Dataset → Multiple Samples → Multiple Trees → Combine Predictions
- [ ] Variance reduction / Stability improvement

### Exercises

- [ ] Visualize bagging process

---

## Phase 4: Bootstrap Sampling

### Learn

- [ ] Sampling With Replacement
- [ ] Duplicate observations possible
- [ ] Every tree sees slightly different data

### Exercises

- [ ] Generate bootstrap datasets

---

## Phase 5: Building Multiple Trees

### Learn

- [ ] Independent Tree Training
- [ ] Each tree learns differently — diversity is beneficial

---

## Phase 6: Aggregation

### Classification Forest → Majority Voting
### Regression Forest → Averaging Predictions

### Exercises

- [ ] Manual ensemble predictions

---

## Phase 7: Random Feature Selection

### The Problem

Trees may choose the same feature repeatedly, making all trees similar.

### Learn

- [ ] Feature Subsampling
- [ ] Tree diversity / Decorrelation

---

## Phase 8: Random Forest Algorithm

### Complete Workflow

Dataset → Bootstrap Sample → Random Feature Selection → Decision Tree → Repeat Hundreds of Times → Aggregate Predictions

---

## Phase 9: Bias-Variance Perspective

### Decision Tree: Low Bias, High Variance
### Random Forest: Similar Bias, Lower Variance → Better generalization

---

## Phase 10: Out-of-Bag (OOB) Evaluation

### Learn

- [ ] Out-of-Bag Samples: internal validation, performance estimation

### Exercises

- [ ] Analyze OOB score

---

## Phase 11: Hyperparameters

- [ ] n_estimators (more trees → better stability, higher cost)
- [ ] max_depth / min_samples_split / min_samples_leaf / max_features

### Exercises

- [ ] Tune forest parameters

---

## Phase 12: Feature Importance

- [ ] Impurity-Based Importance

### Exercises

- [ ] Interpret importance rankings

---

## Phase 13: Classification with Random Forest

### Applications: Churn Prediction, Fraud Detection, Spam Detection
### Metrics: Accuracy, Precision, Recall, F1 Score, ROC-AUC

---

## Phase 14: Regression with Random Forest

### Applications: House Prices, Sales Forecasting
### Metrics: MAE, RMSE, R²

---

## Phase 15: Advantages

- [ ] Handles Non-Linear Data
- [ ] Robust to Outliers
- [ ] Automatic Feature Selection
- [ ] Works with Mixed Data Types

---

## Phase 16: Failure Modes

- [ ] Overfitting with noisy data
- [ ] Large memory usage / Slow inference
- [ ] Interpretability limitations

---

## Phase 17: Feature Engineering Considerations

### Learn

- [ ] Missing Values / Encoding Categorical Variables
- [ ] Scaling generally unnecessary (compare to Logistic Regression)

---

## Phase 18: Scikit-Learn Implementation

### Learn

- [ ] RandomForestClassifier() / RandomForestRegressor()
- [ ] fit() / predict() / predict_proba()

---

## Phase 19: Hyperparameter Tuning

### Learn

- [ ] Grid Search / Random Search
- [ ] Tune: n_estimators, max_depth, max_features, min_samples_leaf

---

## Phase 20: Build from Scratch

### Implement

- [ ] Bootstrap Sampling / Multiple Trees
- [ ] Majority Voting / Prediction Averaging

---

## Phase 21: Business Applications

### Classification: Fraud Detection, Customer Churn, Risk Assessment
### Regression: Revenue Forecasting, Demand Forecasting

---

## Phase 22: Model Explainability

### Learn

- [ ] Feature Importance / Permutation Importance / SHAP (Overview)

---

## Phase 23: Interview Readiness

**Can Explain:** Why Random Forest Exists, Bagging, Bootstrap Sampling, Feature Subsampling, Majority Voting, OOB Error, Variance Reduction, Feature Importance

**Can Compare:** Decision Tree vs Random Forest, Bagging vs Boosting, Random Forest vs Logistic Regression

**Can Build:** Random Forest from Scratch, Production Classification/Regression Pipeline

---

## Phase 24: Transition to Advanced Ensembles

- [ ] Forests average predictions — they don't learn sequentially

---

# 7. K-Nearest Neighbors (KNN)

## Phase 0: Prerequisites

### Machine Learning Foundations

- [ ] Features (X) / Target (y) / Training/Testing Data / Classification / Regression

### Mathematics Foundations

- [ ] Coordinates / Distance / Geometry Basics

### Evaluation

- [ ] Accuracy / Precision / Recall / F1 Score

---

## Phase 1: Why KNN Exists

### First Principles

People with similar characteristics often behave similarly.

- [ ] Similar customers buy similar products
- [ ] Similar houses have similar prices
- [ ] Similar patients may have similar diagnoses

### Core Idea

New Data Point → Find Similar Points → Use Their Outcomes → Make Prediction

- [ ] Similarity-based / Instance-based learning

---

## Phase 2: What KNN Actually Is

### Learn

- [ ] Lazy Learning / Memory-Based Learning
- [ ] No real training phase — stores data, computes during prediction

### Compare

- [ ] Logistic Regression learns parameters; KNN memorizes examples

---

## Phase 3: Distance Intuition

- [ ] Distance Metrics: smaller distance = more similar

---

## Phase 4: Euclidean Distance

### Learn

- [ ] d = √Σ(xᵢ − yᵢ)²
- [ ] Straight-line / Geometric interpretation

### Exercises

- [ ] Compute distances manually, plot neighboring points

---

## Phase 5: Other Distance Metrics

### Manhattan Distance

- [ ] Σ|xᵢ − yᵢ| — city block distance

### Minkowski Distance

- [ ] Generalized distance

### Hamming Distance

- [ ] Categorical comparison

### Compare

- [ ] Euclidean vs Manhattan / Numerical vs Categorical data

---

## Phase 6: Understanding K

### Small K → Sensitive to noise, high variance
### Large K → Oversmoothing, high bias

### Exercises

- [ ] Compare multiple K values

---

## Phase 7: KNN Classification

### Workflow

New Point → Find K Neighbors → Majority Vote → Class Prediction

### Exercises

- [ ] Manual classification examples

---

## Phase 8: KNN Regression

### Workflow

New Point → Find K Neighbors → Average Values → Prediction

### Exercises

- [ ] House price examples

---

## Phase 9: Decision Boundaries

### Small K → Complex boundary / Large K → Smooth boundary

### Exercises

- [ ] Visualize boundaries

---

## Phase 10: Feature Scaling

### Why It Matters

Distance calculations are sensitive to scale (e.g., Age 20–60 vs Salary 20K–500K).

### Learn

- [ ] Standardization / Normalization: equal feature contribution

### Exercises

- [ ] KNN with and without scaling

---

## Phase 11: Curse of Dimensionality

### Learn

- [ ] High-Dimensional Data: distances become less meaningful, neighbors less informative

---

## Phase 12: Choosing K

### Learn

- [ ] Validation Set / Cross Validation

### Exercises

- [ ] Find optimal K

---

## Phase 13: Weighted KNN

### Learn

- [ ] Closer neighbors → more influence / farther neighbors → less influence

---

## Phase 14: Computational Complexity

### Learn

- [ ] Prediction cost: distance calculations, neighbor search
- [ ] Why KNN becomes slow / scalability limitations

---

## Phase 15: Optimization Techniques

- [ ] KD Trees / Ball Trees / Approximate Nearest Neighbors

---

## Phase 16: Advantages

- [ ] Simple / No training phase / Non-linear decision boundaries / Easy to understand

---

## Phase 17: Failure Modes

- [ ] Sensitive to noise and scaling / Slow prediction / Curse of dimensionality / Imbalanced datasets

---

## Phase 18–19: Evaluation Metrics

### Classification: Accuracy, Precision, Recall, F1 Score, ROC-AUC
### Regression: MAE, RMSE, R²

---

## Phase 20: Scikit-Learn Implementation

### Learn

- [ ] KNeighborsClassifier() / KNeighborsRegressor()
- [ ] fit() / predict() / score()

### Exercises

- [ ] Iris Classification / House Price Regression

---

## Phase 21: Build from Scratch

### Implement

- [ ] Distance Functions / Neighbor Search / Majority Voting / Regression Averaging

---

## Phase 22: Business Applications

### Classification: Customer Segmentation, Fraud Detection, Medical Diagnosis
### Regression: House Prices, Product Pricing

---

## Phase 23: Interview Readiness

**Can Explain:** KNN, Lazy Learning, Euclidean/Manhattan Distance, Choosing K, Feature Scaling, Curse of Dimensionality, Weighted KNN

**Can Compare:** KNN vs Logistic Regression, KNN vs Decision Tree, KNN Classification vs Regression

**Can Build:** KNN from Scratch, End-to-End Classification/Regression Pipeline

---

## Phase 24: Model Selection Perspective

### Use KNN For: Small to Medium Datasets, Local Patterns, Simple Baselines
### Avoid KNN For: Very Large Datasets, High-Dimensional Data, Low-Latency Production Systems

---

## Final Mastery

**Can Explain:** Similarity-Based Learning, Distance Metrics, Neighbor Search, Classification Voting, Regression Averaging, Curse of Dimensionality, Hyperparameter K, Feature Scaling

**Can Apply:** Select appropriate distance metric, tune K, scale features, build and evaluate KNN classifiers/regressors

---

# 8. Stacking & Boosting

## Phase 0: Prerequisites

### Core Machine Learning

- [ ] Train/Test Split / Cross Validation / Bias / Variance / Overfitting / Underfitting

### Models

- [ ] Logistic Regression / Decision Trees / Random Forest / KNN

### Ensemble Foundations

- [ ] Bagging / Bootstrap Sampling / Majority Voting / Prediction Averaging

---

## Phase 1: Why Ensemble Learning Exists

### The Problem

Single models have weaknesses: high bias, high variance, limited capacity.

### Types of Ensembles

- [ ] Bagging → Parallel Learning
- [ ] Boosting → Sequential Learning
- [ ] Stacking → Meta Learning

---

## BOOSTING

### Phase 2: Why Boosting Exists

Random Forest trees learn independently and don't learn from mistakes.

**Boosting Idea:** Model 1 → Find mistakes → Model 2 learns mistakes → Find remaining mistakes → Model 3 learns... (sequential improvement, error correction)

---

### Phase 3: Boosting Fundamentals

- [ ] Weak Learner → many weak models combined → Strong Learner

---

### Phase 4: Weak Learners

- [ ] Decision Stumps / Shallow Trees
- [ ] Simple models, slightly better than random

---

### Phase 5: AdaBoost

- [ ] Adaptive Boosting
- [ ] Misclassified points get higher weight → next model focuses on difficult cases
- [ ] Weighted learning / Error correction

---

### Phase 6: AdaBoost Components

- [ ] Sample Weights / Learner Weight
- [ ] Importance weighting / Influence of strong learners

---

### Phase 7: Gradient Boosting Intuition

Instead of correcting samples, correct residual errors:

Prediction Error → New model learns residuals → Add correction → Improve prediction

---

### Phase 8: Residual Learning

- [ ] Residual = Actual − Prediction

### Exercises

- [ ] Compute residuals manually

---

### Phase 9: Gradient Boosting Algorithm

Initial Prediction → Calculate Residuals → Train Small Tree → Predict Residuals → Update Model → Repeat

---

### Phase 10: Learning Rate (Shrinkage)

- [ ] Small learning rate → slower, more stable
- [ ] Large learning rate → faster, higher overfitting risk

---

### Phase 11: Gradient Boosting Hyperparameters

- [ ] n_estimators / learning_rate / max_depth / min_samples_leaf

---

### Phase 12: XGBoost

- [ ] Extreme Gradient Boosting
- [ ] Improvements: Regularization, Faster Training, Parallelization, Missing Value Handling

---

### Phase 13: LightGBM

- [ ] Histogram-Based Learning / Leaf-Wise Growth
- [ ] Fast training, large dataset support

---

### Phase 14: CatBoost

- [ ] Categorical Feature Handling
- [ ] Minimal preprocessing, strong default performance

---

### Phase 15: Boosting Failure Modes

- [ ] Overfitting / Noise Sensitivity / Long Training Time

---

## STACKING

### Phase 16: Why Stacking Exists

Different models learn different patterns. Can we combine them intelligently?

- [ ] Logistic Regression → linear relationships
- [ ] Decision Tree → rule-based patterns
- [ ] KNN → local patterns

---

### Phase 17: Stacking Fundamentals

**Workflow:** Dataset → Multiple Models → Predictions → Meta Model → Final Prediction

- [ ] Base Models / Meta Model

---

### Phase 18: Base Learners

- [ ] Logistic Regression / Decision Trees / Random Forest / KNN / SVM

---

### Phase 19: Meta Learner

- [ ] Second-Level Model (commonly Logistic Regression or XGBoost)

---

### Phase 20: Out-of-Fold Predictions

- [ ] OOF Predictions: prevents data leakage, proper stacking workflow

---

### Phase 21: Stacking Architecture

- [ ] Level 0: Base Models
- [ ] Level 1: Meta Model

---

### Phase 22: Stacking vs Voting

- [ ] Voting: average predictions
- [ ] Stacking: learn how to combine predictions (intelligent aggregation)

---

### Phase 23: Hyperparameter Tuning

- [ ] Base Model Tuning / Meta Model Tuning

---

### Phase 24: Explainability

- [ ] Boosting: Feature Importance
- [ ] Stacking: Model Contribution Analysis
- [ ] SHAP Overview / Permutation Importance

---

### Phase 25: Scikit-Learn Implementation

- [ ] AdaBoostClassifier() / GradientBoostingClassifier()
- [ ] StackingClassifier() / StackingRegressor()

---

### Phase 26: Real Projects

### Beginner → Titanic Survival
### Intermediate → Customer Churn
### Advanced → Fraud Detection
### Expert → Kaggle-Style Ensemble Pipeline

---

### Phase 27: Interview Readiness

**Can Explain (Boosting):** Weak Learners, AdaBoost, Gradient Boosting, Residual Learning, Learning Rate, XGBoost, LightGBM, CatBoost

**Can Explain (Stacking):** Base Learners, Meta Learner, OOF Predictions, Data Leakage Prevention

**Can Compare:** Bagging vs Boosting, Random Forest vs XGBoost, Voting vs Stacking, XGBoost vs LightGBM

**Can Build:** Boosting Pipeline, Stacking Pipeline, Kaggle-Level Ensemble Model

---

# 9. AdaBoost

## Phase 0: Prerequisites

### Machine Learning Foundations

- [ ] Classification / Regression / Train/Test Split / Cross Validation

### Decision Trees

- [ ] Fundamentals / Tree Splits / Gini Impurity / Entropy

### Ensemble Learning

- [ ] Ensemble Concepts / Bagging / Random Forest / Boosting Overview

---

## Phase 1: Why AdaBoost Exists

**Problem:** Single trees and random forests don't focus on past mistakes.

**Core Idea:** Model 1 → Find mistakes → Increase importance of mistakes → Model 2 focuses on mistakes → Repeat

---

## Phase 2: What is a Weak Learner?

### Learn

- [ ] Weak Learner: slightly better than random
- [ ] Strong Learner: high predictive power
- [ ] Decision Stump: tree with depth = 1

---

## Phase 3: AdaBoost Intuition

Dataset → Train Weak Learner → Identify Mistakes → Increase Weight of Mistakes → Train Next Learner → Repeat

- [ ] Hard examples become more important; easy examples less important

---

## Phase 4: Sample Weights

### Initial State: every sample has equal importance

### After Training:
- [ ] Correctly classified → lower importance
- [ ] Misclassified → higher importance

### Exercises

- [ ] Track weight changes manually

---

## Phase 5: Decision Stumps in AdaBoost

- [ ] Why stumps: fast, weak, easy to combine

---

## Phase 6: Learner Error Rate

- [ ] Weighted Error: not all mistakes are equal

### Exercises

- [ ] Calculate weighted error

---

## Phase 7: Learner Importance (Alpha)

- [ ] Better learner → higher influence
- [ ] Poor learner → lower influence

---

## Phase 8: Weight Updates

- [ ] Wrong predictions → weight increases
- [ ] Correct predictions → weight decreases

### Exercises

- [ ] Perform manual weight updates

---

## Phase 9: AdaBoost Training Cycle

Initialize Weights → Train Stump → Calculate Error → Calculate Learner Weight → Update Sample Weights → Normalize Weights → Repeat

---

## Phase 10: Final Prediction

### Weighted Voting

- [ ] Strong learners → more influence; weak learners → less influence

---

## Phase 11: Classification AdaBoost

### Applications: Spam Detection, Fraud Detection, Churn Prediction

---

## Phase 12: Multi-Class AdaBoost

- [ ] Multi-class extensions

---

## Phase 13: Hyperparameters

- [ ] n_estimators / learning_rate
- [ ] More estimators → more learning, more overfitting risk

---

## Phase 14: Learning Rate

- [ ] Small → slow, better generalization
- [ ] Large → fast, higher overfitting risk

---

## Phase 15: Bias-Variance Perspective

- [ ] Decision Stump → High bias
- [ ] AdaBoost → Reduces bias

---

## Phase 16: AdaBoost vs Random Forest

| | Random Forest | AdaBoost |
|---|---|---|
| Learning | Parallel | Sequential |
| Strategy | Independent | Error Correction |
| Effect | Variance Reduction | Bias Reduction |

---

## Phase 17: AdaBoost vs Gradient Boosting

- [ ] AdaBoost: reweights observations
- [ ] Gradient Boosting: learns residual errors directly

---

## Phase 18: Failure Modes

- [ ] Sensitivity to Outliers / Noise Amplification

---

## Phase 19: Feature Importance

- [ ] Importance scores / Feature contribution

---

## Phase 20: Evaluation Metrics

- [ ] Accuracy / Precision / Recall / F1 Score / ROC-AUC

---

## Phase 21: Scikit-Learn Implementation

- [ ] AdaBoostClassifier()
- [ ] fit() / predict() / predict_proba()

---

## Phase 22: Build from Scratch

### Implement

- [ ] Sample Weights / Weighted Error / Learner Weight / Weight Updates / Weighted Voting

---

## Phase 23: Business Applications

- [ ] Fraud Detection / Customer Churn / Credit Risk / Medical Diagnosis

---

## Phase 24: Interview Readiness

**Can Explain:** AdaBoost, Weak Learners, Decision Stumps, Sample Weights, Learner Weights, Weight Updates, Weighted Voting, Learning Rate, Failure Modes

**Can Compare:** Decision Tree vs AdaBoost, Random Forest vs AdaBoost, AdaBoost vs Gradient Boosting, Bagging vs Boosting

**Can Build:** AdaBoost from Scratch, Production AdaBoost Classifier, End-to-End Classification Pipeline

---

## Phase 25: Transition to Gradient Boosting

- [ ] AdaBoost focuses on misclassified samples
- [ ] Gradient Boosting learns residual errors directly
- [ ] Next: Gradient Boosting → XGBoost → LightGBM → CatBoost

---

# 10. Gradient Boosting

## Phase 0: Prerequisites

### Machine Learning Foundations

- [ ] Supervised Learning / Regression / Classification / Train/Test Split / Cross Validation

### Decision Trees

- [ ] Fundamentals / Regression Trees / Tree Depth / Overfitting

### Ensemble Learning

- [ ] Bagging / Random Forest / AdaBoost

### Mathematics

- [ ] Loss Functions / Optimization / Gradient Intuition / Gradient Descent

---

## Phase 1: Why Gradient Boosting Exists

Decision Trees overfit; Random Forest reduces variance but doesn't explicitly correct mistakes; AdaBoost has limited flexibility.

**Key Insight:** Can we directly learn prediction errors instead of re-training on the original target?

---

## Phase 2: Core Intuition

Prediction → Error → Learn Error → Correct Prediction → Repeat

Each tree learns what previous trees got wrong.

---

## Phase 3: Residuals

**Residual = Actual − Prediction**

Residuals represent remaining information / unexplained patterns.

### Exercises

- [ ] Calculate residuals manually, visualize errors

---

## Phase 4: Residual Learning

Tree 1 → Prediction → Residuals → Tree 2 learns residuals → Updated prediction → New residuals → Repeat

Each tree is a correction model.

---

## Phase 5: Gradient Boosting Architecture

Initial Model → Tree 1 → Tree 2 → Tree 3 → ... → Final Prediction

- [ ] Base Prediction / Residual Models / Sequential Updates

---

## Phase 6: Loss Functions

### Regression: MSE, MAE
### Classification: Log Loss, Cross Entropy

Gradient Boosting optimizes the loss function.

---

## Phase 7: Gradient Intuition

Gradient = Direction of steepest increase. To minimize loss, move opposite the gradient.

### Exercises

- [ ] Visualize gradient descent

---

## Phase 8: Why It's Called Gradient Boosting

Instead of learning residuals directly, Gradient Boosting learns **negative gradients**, which generalizes to any differentiable loss function.

---

## Phase 9: Gradient Boosting Algorithm

Initialize Prediction → Calculate Loss → Compute Negative Gradient → Train Tree on Gradient → Update Prediction → Repeat

---

## Phase 10: Learning Rate (Shrinkage)

- [ ] Small → slower, better generalization
- [ ] Large → faster, overfitting risk

---

## Phase 11–12: Number of Trees & Tree Depth

- [ ] More trees → better fit, more complexity
- [ ] Shallow trees → weak learners / Deep trees → stronger but more overfitting risk

---

## Phase 13: Regularization

- [ ] Learning Rate / Tree Depth Limits / Minimum Samples

---

## Phase 14–15: Applications

### GradientBoostingRegressor: House Prices, Revenue/Demand Forecasting
### GradientBoostingClassifier: Churn, Fraud, Risk Assessment

---

## Phase 16: Feature Importance

- [ ] Importance Scores: which features drive predictions

---

## Phase 17: Hyperparameter Tuning

- [ ] n_estimators / learning_rate / max_depth / min_samples_leaf / subsample
- [ ] Grid Search / Random Search

---

## Phase 18: Stochastic Gradient Boosting

- [ ] Subsampling: train on random subsets → faster training, reduced overfitting

---

## Phase 19: Failure Modes

- [ ] Overfitting / Long Training Time / Poor Hyperparameters / Noisy Data

---

## Phase 20: Scikit-Learn Implementation

- [ ] GradientBoostingRegressor() / GradientBoostingClassifier()
- [ ] fit() / predict() / predict_proba()

---

## Phase 21: Build from Scratch

### Implement

- [ ] Residual Computation / Sequential Trees / Prediction Updates / Gradient Approximation

---

## Phase 22: Evaluation

### Classification: Accuracy, Precision, Recall, F1 Score, ROC-AUC
### Regression: MAE, RMSE, R²

---

## Phase 23: Business Applications

### Classification: Fraud Detection, Customer Churn, Credit Risk
### Regression: Pricing Models, Sales/Revenue Forecasting

---

## Phase 24: Interview Readiness

**Can Explain:** Why Gradient Boosting Exists, Residual Learning, Gradient Concept, Sequential Learning, Learning Rate, Tree Depth, Loss Functions, Stochastic Gradient Boosting

**Can Compare:** AdaBoost vs Gradient Boosting, Random Forest vs Gradient Boosting, Bagging vs Boosting

**Can Build:** Gradient Boosting Pipeline, Regression/Classification Solution

---

## Phase 25: Transition to Modern Boosting

### Gradient Boosting Limitations: Slow Training, Sequential Processing

### Next Topics: XGBoost → LightGBM

---

# 11. XGBoost

## Phase 0: Prerequisites

### Machine Learning Foundations

- [ ] Supervised Learning / Regression / Classification / Train/Test Split / Cross Validation

### Decision Trees

- [ ] Trees / Splits / Pruning / Feature Importance

### Ensemble Learning

- [ ] Random Forest / AdaBoost / Gradient Boosting

### Mathematics

- [ ] Loss Functions / Gradient Descent / First & Second Derivatives (Basic Intuition)

---

## Phase 1: Why XGBoost Exists

Traditional Gradient Boosting: slow, high memory, overfitting risk, limited optimization.

**XGBoost makes Gradient Boosting:** Faster + More Accurate + More Scalable + More Regularized

---

## Phase 2: XGBoost Big Picture

Gradient Boosting + Engineering Improvements + Mathematical Improvements + System Optimizations = XGBoost

**XGBoost IS advanced Gradient Boosting, NOT a new algorithm family.**

---

## Phase 3: Architecture Overview

Still boosting: Prediction → Residual Errors → New Tree → Prediction Update → Repeat (but aggressively optimized)

---

## Phase 4: Objective Function

**Goal:** Good Predictions + Simple Trees (Training Loss + Regularization Penalty)

---

## Phase 5: Regularization in XGBoost

- [ ] L1 (Lasso Style) / L2 (Ridge Style)
- [ ] Why XGBoost generalizes well

---

## Phase 6: Tree Complexity Control

- [ ] max_depth / min_child_weight / gamma

---

## Phase 7: Gradient and Hessian

- [ ] First Order Gradient: direction of improvement
- [ ] Second Order Gradient: curvature information
- [ ] Traditional GBM: first-order only / XGBoost: first + second order → faster convergence

---

## Phase 8: Tree Split Finding

- [ ] Gain Calculation: choose best split based on loss reduction

---

## Phase 9: Pruning Strategy

- [ ] Traditional Trees: pre-pruning
- [ ] XGBoost: post-pruning (grow tree → evaluate splits → remove weak branches)

---

## Phase 10: Missing Value Handling

- [ ] Automatic missing value support — no mandatory imputation

---

## Phase 11: Shrinkage (Learning Rate)

- [ ] eta: each tree contributes partially
- [ ] Small eta → better generalization

---

## Phase 12: Subsampling

- [ ] Row Sampling: subsample
- [ ] Column Sampling: colsample_bytree
- [ ] Reduces overfitting, increases diversity

---

## Phase 13: Hyperparameters

| Category | Parameters |
|---|---|
| Learning | learning_rate |
| Trees | n_estimators, max_depth |
| Regularization | gamma, reg_alpha, reg_lambda |
| Sampling | subsample, colsample_bytree |

---

## Phase 14: Feature Importance

- [ ] Weight / Gain / Cover (different importance measures)

---

## Phase 15–16: Applications

### XGBClassifier: Churn, Fraud, Credit Scoring, Medical Risk
### XGBRegressor: House Prices, Revenue/Demand Forecasting

---

## Phase 17: Multi-Class Classification

- [ ] Softmax / Multi-Class Log Loss

---

## Phase 18: Imbalanced Data

- [ ] scale_pos_weight: handling rare classes (Fraud, Disease)

---

## Phase 19: Early Stopping

- [ ] Stop when validation performance stops improving
- [ ] Faster training / Reduced overfitting

---

## Phase 20: Cross Validation

- [ ] K-Fold CV / Stratified CV

---

## Phase 21: Model Explainability

- [ ] Built-in: Gain, Cover / Advanced: SHAP Values

---

## Phase 22: Failure Modes

- [ ] Overfitting / Excessive Trees / Poor Hyperparameters / Data Leakage

---

## Phase 23: Scikit-Learn API

- [ ] XGBClassifier() / XGBRegressor()
- [ ] fit() / predict() / predict_proba()

---

## Phase 24: Build Understanding from Scratch

- [ ] Residual Learning / Gain Calculation / Regularization / Tree Growth

---

## Phase 25: Real Projects

### Beginner → Titanic Survival
### Intermediate → Customer Churn
### Advanced → Credit Risk Modeling, Fraud Detection
### Expert → Kaggle Competition Pipeline

---

## Phase 26: Interview Readiness

**Can Explain:** XGBoost, Why it Exists, Gradient Boosting Foundation, Regularization, First vs Second Order Optimization, Gain, Missing Value Handling, Early Stopping, Feature Importance

**Can Compare:** Random Forest vs XGBoost, AdaBoost vs XGBoost, Gradient Boosting vs XGBoost

**Can Build:** Classification/Regression Pipeline, Hyperparameter Tuning Workflow, Explainable ML Solution

---

# 12. Dimensionality Reduction

## Phase 0: Prerequisites

### Mathematics

- [ ] Vectors, Coordinates, Distance, Variance, Covariance

### Statistics

- [ ] Correlation, Variance, Distribution of Data

### Machine Learning

- [ ] Features, Feature Engineering, KNN, Logistic Regression, Decision Trees

---

## Phase 1: Why Dimensionality Reduction Exists

More Features → More Complexity → More Noise → Slower Training → Overfitting Risk

Not all features contain useful information. Many may overlap (e.g., Salary, Monthly Income, Annual Income, Income Category).

- [ ] Redundant / Correlated / Noisy Features

---

## Phase 2: Curse of Dimensionality

As dimensions increase: distances become less meaningful, data becomes sparse, KNN performance drops, computation increases.

---

## Phase 3: Goals of Dimensionality Reduction

- [ ] Faster Models (fewer features)
- [ ] Better Generalization (remove noise)
- [ ] Visualization (2D/3D representation)
- [ ] Storage Efficiency

---

## Phase 4: Types of Dimensionality Reduction

### Feature Selection

Keep important features, remove others.

- [ ] Lasso / Tree Feature Importance / Mutual Information

### Feature Extraction

Create new features.

- [ ] PCA / LDA / Autoencoders

---

## FEATURE SELECTION

### Phase 5: Filter Methods

- [ ] Correlation Filtering / Variance Threshold / Chi-Square Selection

---

### Phase 6: Wrapper Methods

- [ ] Forward Selection / Backward Elimination / Recursive Feature Elimination (RFE)

---

### Phase 7: Embedded Methods

- [ ] Lasso (automatic feature removal) / Tree Importance / XGBoost Importance

---

## PCA

### Phase 8: Introduction to PCA

**Can we create fewer features that preserve most information?** Answer: PCA (Principal Component Analysis)

---

### Phase 9: Variance Intuition

- [ ] High variance → more information / Low variance → less information

---

### Phase 10: Principal Components

- [ ] PC1: Maximum Variance / PC2: Second Highest / PC3: Third Highest

---

### Phase 11: PCA Geometry

- [ ] Coordinate Rotation / Projection
- [ ] PCA rotates coordinate system to capture variance efficiently

---

### Phase 12: Explained Variance

- [ ] Explained Variance Ratio: how much information is preserved?
- [ ] Example: PC1 = 70%, PC2 = 20%, Total = 90%

### Exercises

- [ ] Select optimal number of components

---

### Phase 13: PCA Workflow

Standardize Data → Compute Covariance Matrix → Find Principal Components → Project Data → Reduced Dataset

---

### Phase 14: Choosing Number of Components

- [ ] Scree Plot / Explained Variance Curve
- [ ] Tradeoff: Information vs Feature Count

---

### Phase 15: PCA Applications

- [ ] Visualization / Noise Reduction / Compression / Faster ML

---

## LDA

### Phase 16: Linear Discriminant Analysis

- [ ] PCA: preserve variance / LDA: separate classes
- [ ] Between-Class Variance / Within-Class Variance
- [ ] Maximize separation, minimize overlap

---

## NON-LINEAR METHODS

### Phase 17: t-SNE

- [ ] t-Distributed Stochastic Neighbor Embedding
- [ ] Preserves local neighborhoods
- [ ] Use for: Visualization, Cluster inspection
- [ ] Limitations: slow, not ideal for production features

---

### Phase 18: UMAP

- [ ] Uniform Manifold Approximation and Projection
- [ ] Faster than t-SNE, preserves structure better
- [ ] Use for: Large datasets, Visualization

---

## AUTOENCODERS

### Phase 19: Autoencoder Introduction

Neural Network Compression: Encoder → Bottleneck Layer → Decoder

Input → Compress → Reconstruct

---

## Phase 20: Dimensionality Reduction Pipeline

Raw Data → Feature Selection → Scaling → PCA/LDA → Model Training

---

## Phase 21: Impact on ML Models

### Helps: KNN, Clustering, Linear Models
### Sometimes Unnecessary: Trees, Random Forest, XGBoost

---

## Phase 22: Evaluation

- [ ] Compare model performance before vs after reduction
- [ ] Tradeoffs: Accuracy, Speed, Interpretability

---

## Phase 23: Scikit-Learn Implementation

- [ ] PCA() / LinearDiscriminantAnalysis()
- [ ] SelectKBest() / RFE()

---

## Phase 24: Failure Modes

- [ ] Information Loss / Poor Component Selection / Overcompression / Misinterpreting PCA Components

---

## Phase 25: Real Projects

### Beginner → PCA on Iris Dataset
### Intermediate → Customer Segmentation
### Advanced → Fraud Detection Pipeline
### Expert → High-Dimensional Feature Store Optimization

---

## Phase 26: Interview Readiness

**Can Explain:** Curse of Dimensionality, Feature Selection, Feature Extraction, PCA, Principal Components, Explained Variance, LDA, t-SNE, UMAP, Autoencoders

**Can Compare:** PCA vs LDA, PCA vs Feature Selection, t-SNE vs UMAP, PCA vs Autoencoders

**Can Build:** PCA Pipeline, Feature Selection Pipeline, Visualization Workflow, Production DR Pipeline

---

# 13. Naive Bayes

## Phase 0: Prerequisites

### Statistics Foundations

- [ ] Probability / Conditional Probability / Independent Events / Probability Distributions / Random Variables

### Machine Learning Foundations

- [ ] Classification / Features (X) / Labels (y) / Train/Test Split

---

## Phase 1: Why Naive Bayes Exists

**Question:** Given some features, what is the probability that an observation belongs to a particular class?

- [ ] Spam? / Customer Churn? / Disease?

**First Principles:** Instead of learning complex boundaries, can we use probability? Answer: Naive Bayes

---

## Phase 2: Bayes Theorem Foundation

**Formula:** P(A|B) = P(B|A) · P(A) / P(B)

- [ ] Prior Probability: initial belief
- [ ] Likelihood: evidence strength
- [ ] Posterior Probability: updated belief
- [ ] Evidence: observed data

### Exercises

- [ ] Medical diagnosis examples / Spam detection examples

---

## Phase 3: Probability Intuition

- [ ] Prior: before seeing data / Posterior: after seeing data
- [ ] Data changes beliefs

---

## Phase 4: The "Naive" Assumption

**Assumption:** Features are independent given the class.

**Example (Spam):** Words "Free", "Money", "Offer" contribute independently.

**Why Naive Bayes Still Works:** Simple, Fast, Often surprisingly effective

---

## Phase 5: Naive Bayes Classification Workflow

New Observation → Calculate Class Probabilities → Choose Highest Probability → Prediction

---

## Phase 6–7: Likelihood & Posterior

- [ ] Likelihood: probability of observing features given a class
- [ ] Posterior: probability of class given observed features → final decision metric

---

## Phase 8: Types of Naive Bayes

Different data types require different assumptions.

---

### Phase 9: Gaussian Naive Bayes

- [ ] GaussianNB
- [ ] Features follow Normal Distribution
- [ ] For continuous numerical data (Age, Salary, Height)
- [ ] Uses mean and variance for estimation

---

### Phase 10: Multinomial Naive Bayes

- [ ] MultinomialNB
- [ ] For text classification, word counts
- [ ] Spam Detection / News Classification

---

### Phase 11: Bernoulli Naive Bayes

- [ ] BernoulliNB
- [ ] For binary features (word present / absent)

---

### Phase 12: Complement Naive Bayes

- [ ] ComplementNB
- [ ] For imbalanced text datasets

---

## Phase 13: Laplace Smoothing

**Problem:** Zero probability when a word has never been seen → entire prediction collapses.

**Solution:** Laplace (Add-One) Smoothing — avoids zero probabilities.

---

## Phase 14: Feature Engineering

- [ ] Tokenization / Stop Words / Stemming / Lemmatization
- [ ] Bag of Words / TF-IDF

---

## Phase 15: Classification Metrics

- [ ] Accuracy / Precision / Recall / F1 Score / ROC-AUC

---

## Phase 16: Handling Imbalanced Data

- [ ] Accuracy can mislead
- [ ] Use Precision / Recall / F1

---

## Phase 17: Decision Boundaries

- [ ] Probability-based decisions differ from Logistic Regression

---

## Phase 18: Naive Bayes vs Logistic Regression

| | Naive Bayes | Logistic Regression |
|---|---|---|
| Approach | Probabilistic | Learns weights |
| Independence | Assumes independence | No assumption |

---

## Phase 19: Advantages

- [ ] Fast Training/Prediction / Works with Small Data / Effective for Text
- [ ] Applications: NLP, Spam Detection, Sentiment Analysis

---

## Phase 20: Failure Modes

- [ ] Correlated Features / Wrong Distribution Assumptions / Poor Probability Estimates

---

## Phase 21: Scikit-Learn Implementation

- [ ] GaussianNB() / MultinomialNB() / BernoulliNB()
- [ ] fit() / predict() / predict_proba()

---

## Phase 22: Build from Scratch

### Implement

- [ ] Prior Calculation / Likelihood Calculation / Posterior Calculation / Prediction Logic

---

## Phase 23: Real Projects

### Beginner → Spam Detection
### Intermediate → News Classification
### Advanced → Sentiment Analysis
### Expert → Document Categorization System

---

## Phase 24: Interview Readiness

**Can Explain:** Bayes Theorem, Prior/Posterior/Likelihood, Independence Assumption, Gaussian/Multinomial/Bernoulli NB, Laplace Smoothing

**Can Compare:** Naive Bayes vs Logistic Regression, Gaussian vs Multinomial NB, Naive Bayes vs Decision Trees

**Can Build:** Spam Classifier, Text Classification Pipeline, End-to-End Naive Bayes Solution

---

## Phase 25: Connections to NLP

Naive Bayes historically dominated: Spam Filtering, Email Classification, News Categorization

**Next Topics:** SVM → K-Means Clustering → NLP Feature Engineering → TF-IDF Deep Dive

---

# 14. Support Vector Machine (SVM)

## Phase 0: Prerequisites

### Mathematics

- [ ] Coordinates / Distance / Vectors / Dot Product / Geometry Basics

### Machine Learning Foundations

- [ ] Classification / Regression / Features and Labels / Train/Test Split

### Previous Algorithms

- [ ] Logistic Regression / KNN / Decision Trees

---

## Phase 1: Why SVM Exists

Many classifiers can separate classes. **The key question:** Which separator is the BEST separator?

**Core Idea:** Choose the separator that leaves the largest safety gap between classes.

- [ ] SVM separates classes **optimally**, not just correctly

---

## Phase 2: Linear Separability

- [ ] Data separable using a straight line
- [ ] Examples: two distinct groups, simple classification problems

---

## Phase 3: Decision Boundary

- [ ] The line (or hyperplane) used to separate classes

---

## Phase 4: Margin Intuition

**Margin = Distance from decision boundary to nearest points**

- [ ] Large Margin → Better generalization
- [ ] Small Margin → Higher risk of mistakes

---

## Phase 5: Maximum Margin Classifier

Among all valid boundaries, choose the **largest margin**.

- [ ] Better robustness and generalization

---

## Phase 6: Support Vectors

- [ ] Points closest to boundary that **determine** the classifier
- [ ] Removing distant points barely changes the boundary
- [ ] Removing support vectors changes it significantly

---

## Phase 7–8: Hard vs Soft Margin SVM

### Hard Margin SVM

- [ ] Perfect separation assumed, no noise — rare in real-world data

### Soft Margin SVM

- [ ] Allow some mistakes for better generalization
- [ ] Handles noise, outliers, and overlap

---

## Phase 9: Regularization Parameter (C)

| C Value | Effect |
|---|---|
| Large C | Fewer mistakes, smaller margin, more overfitting |
| Small C | Larger margin, more tolerance, better generalization |

---

## Phase 10–11: Non-Linear Problems & Feature Transformation

Many datasets can't be separated with a straight line. Transform data into higher dimensions where separability appears (2D → 3D).

---

## Phase 12: Kernel Trick

**Idea:** Compute similarity without explicitly creating higher dimensions.

- [ ] Efficient transformation into new feature spaces

---

## Phase 13: Linear Kernel

- [ ] For linearly separable data and high-dimensional text data
- [ ] Fastest kernel

---

## Phase 14: Polynomial Kernel

- [ ] Captures feature interactions

---

## Phase 15: RBF Kernel (Radial Basis Function)

- [ ] Most common kernel
- [ ] Captures complex, non-linear boundaries

---

## Phase 16: Gamma Parameter

| Gamma | Effect |
|---|---|
| Small | Smooth boundary, simpler model |
| Large | Complex boundary, overfitting risk |

---

## Phase 17: SVM Regression (SVR)

- [ ] SVM can perform regression, not just classification
- [ ] Applications: Price Prediction, Revenue Forecasting

---

## Phase 18: Hyperparameter Tuning

- [ ] C, Gamma, Kernel Type
- [ ] Grid Search / Cross Validation

---

## Phase 19: Feature Scaling

- [ ] SVM is distance-based — scaling is **critical**
- [ ] StandardScaler / MinMaxScaler

---

## Phase 20: Evaluation Metrics

### Classification: Accuracy, Precision, Recall, F1 Score, ROC-AUC
### Regression: MAE, RMSE, R²

---

## Phase 21: Advantages

- [ ] Effective in high dimensions / Strong theoretical foundation / Robust decision boundaries
- [ ] Applications: Text Classification, Image Classification, Bioinformatics

---

## Phase 22: Failure Modes

- [ ] Slow on huge datasets / Sensitive to parameter tuning / Scaling requirements / Difficult interpretation

---

## Phase 23: Scikit-Learn Implementation

- [ ] SVC() / SVR()
- [ ] fit() / predict() / score()

---

## Phase 24: Build Intuition from Scratch

- [ ] Margin maximization / Support vectors / Kernel transformation

---

## Phase 25: Real Projects

### Beginner → Iris Classification
### Intermediate → Spam Detection
### Advanced → Customer Churn Prediction
### Expert → High-Dimensional Text Classification

---

## Phase 26: Interview Readiness

**Can Explain:** SVM, Margin, Support Vectors, Hard/Soft Margin, Kernel Trick, Linear/Polynomial/RBF Kernel, C Parameter, Gamma Parameter

**Can Compare:** Logistic Regression vs SVM, KNN vs SVM, Linear vs RBF Kernel, SVM vs Decision Tree

**Can Build:** Classification/SVR Pipeline, Tuned Production SVM Model

---

## Phase 27: Advanced Topics

- [ ] Multi-Class SVM / One-vs-Rest / One-vs-One

---

## Phase 28: When to Use SVM

### Good For: Medium-sized datasets, High-dimensional data, Text classification
### Avoid For: Massive datasets, Real-time systems, Easily explainable models

---

## Final Mastery

**Can Explain:** Margin Maximization, Support Vectors, Soft Margin, Kernel Trick, C Parameter, Gamma Parameter, SVM Classification, SVR Regression

**Can Apply:** Choose Proper Kernel, Scale Features, Tune C and Gamma, Build/Evaluate SVM Pipelines

---

# 15. Hierarchical Clustering

## Phase 0: Prerequisites

### Statistics

- [ ] Distance Concepts / Euclidean & Manhattan Distance / Similarity vs Dissimilarity

### Machine Learning

- [ ] Supervised vs Unsupervised Learning / Clustering Fundamentals

### Mathematics

- [ ] Coordinates / Distance Matrices / Basic Tree Structures

---

## Phase 1: Why Hierarchical Clustering Exists

K-Means requires knowing K upfront. Hierarchies exist everywhere naturally.

**Question:** What if we don't know the number of clusters?

**Answer:** Hierarchical Clustering — builds a tree instead of a fixed number.

---

## Phase 2: Types of Hierarchical Clustering

### Agglomerative (Bottom-Up) — Most Common

Every point = own cluster → Merge closest clusters → Repeat → One giant cluster

### Divisive (Top-Down)

All points → Split into groups → Split again → Repeat

---

## Phase 3: Agglomerative Clustering Deep Dive

Initial State: Each point = cluster

Find closest clusters → Merge → Update distances → Repeat

---

## Phase 4: Distance Matrix

- [ ] Stores pairwise distances between all points

### Exercises

- [ ] Create distance matrices manually

---

## Phase 5: Cluster Linkage

When clusters contain multiple points, how do we measure distance between clusters?

---

### Single Linkage (Minimum Distance)

- [ ] Closest points determine distance
- [ ] Captures irregular shapes
- [ ] Failure mode: chaining effect

---

### Complete Linkage (Maximum Distance)

- [ ] Farthest points determine distance
- [ ] Compact clusters
- [ ] Failure mode: sensitive to outliers

---

### Average Linkage

- [ ] Average distance between all pairs
- [ ] Balanced, general-purpose strategy

---

### Ward Linkage

- [ ] Minimize variance increase after merging
- [ ] Often best default choice
- [ ] Compact clusters, great for business analytics

---

## Phase 6: Dendrogram

- [ ] Tree representation of cluster merges
- [ ] Components: Branches, Merge Heights, Leaves
- [ ] Cut at a height to determine number of clusters

### Exercises

- [ ] Read dendrograms, interpret merge levels

---

## Phase 7: Distance Metrics

- [ ] Euclidean (most common) / Manhattan (grid-based) / Cosine (text similarity)

---

## Phase 8: Feature Scaling

- [ ] Distance-based → scaling is critical
- [ ] StandardScaler / MinMaxScaler

---

## Phase 9: Evaluating Clusters

- [ ] Silhouette Score / Davies-Bouldin Index / Calinski-Harabasz Index

---

## Phase 10: Advantages

- [ ] No need for K initially
- [ ] Dendrogram interpretation
- [ ] Flexible cluster structures
- [ ] Hierarchical relationships visible

---

## Phase 11: Failure Modes

- [ ] Computationally expensive / Sensitive to noise and scaling / Irreversible merges

---

## Phase 12: Comparisons

### Hierarchical vs K-Means

| | K-Means | Hierarchical |
|---|---|---|
| Requires K | Yes | No |
| Speed | Fast | Slower |
| Structure | Centroid-based | Tree-based |
| Interpretability | Lower | Higher |

### Hierarchical vs DBSCAN

- [ ] Hierarchical: tree structure, global clustering
- [ ] DBSCAN: density-based, noise detection

---

## Phase 13: Scikit-Learn Implementation

- [ ] AgglomerativeClustering()
- [ ] Parameters: n_clusters, linkage, metric

---

## Phase 14: Visualization

- [ ] Dendrogram Plot / Cluster Scatter Plot / Heatmaps

---

## Phase 15: Business Applications

- [ ] Customer Segmentation / User Group Discovery / Gene Clustering / Document Grouping

---

## Phase 16: Build from Scratch

### Implement

- [ ] Distance Matrix / Linkage Calculation / Cluster Merging / Dendrogram Logic

---

## Phase 17: Interview Readiness

**Can Explain:** Hierarchical Clustering, Agglomerative/Divisive, Distance Matrix, Single/Complete/Average/Ward Linkage, Dendrogram

**Can Compare:** Hierarchical vs K-Means, Hierarchical vs DBSCAN, Single vs Complete Linkage, Average vs Ward Linkage

**Can Build:** Customer Segmentation Pipeline, Dendrogram Analysis Workflow, Production Clustering Solution

---

## Final Mastery

**Can Explain:** Why Hierarchical Clustering Exists, Bottom-Up vs Top-Down, Linkage Methods, Dendrogram Interpretation, Cluster Evaluation, Scaling Requirements

**Can Apply:** Select Proper Linkage, Read Dendrograms, Determine Cluster Count, Evaluate Clustering Quality, Build Real-World Segmentation Models

---

# 16. DBSCAN

## Phase 0: Prerequisites

### Mathematics

- [ ] Distance Concepts / Euclidean Distance / Neighborhood Radius

### Machine Learning Foundations

- [ ] Unsupervised Learning / Clustering Basics / Similarity vs Dissimilarity

### Previous Clustering Algorithms

- [ ] K-Means / Hierarchical Clustering

---

## Phase 1: Why DBSCAN Exists

K-Means struggles with non-spherical clusters, noise, outliers, and unknown K.
Hierarchical Clustering is expensive and sensitive to noise.

**DBSCAN** identifies clusters based on **density** instead of centroids or hierarchies.

---

## Phase 2: What is DBSCAN?

**DBSCAN = Density-Based Spatial Clustering of Applications with Noise**

- [ ] Dense regions → Clusters
- [ ] Sparse regions → Noise / Separation

---

## Phase 3: Density Intuition

- [ ] Dense area: many nearby points
- [ ] Sparse area: few nearby points

---

## Phase 4: Epsilon (ε) — Neighborhood Radius

- [ ] Defines neighborhood size
- [ ] Small ε → tiny clusters, more noise
- [ ] Large ε → bigger clusters, possible over-merging

---

## Phase 5: MinPts — Minimum Points

- [ ] Minimum neighbors required to form a dense region
- [ ] Small MinPts → sensitive to noise
- [ ] Large MinPts → requires denser clusters

---

## Phase 6: Point Types

### Core Point

- [ ] Has enough neighbors (≥ MinPts within ε)

### Border Point

- [ ] Near dense region but insufficient neighbors itself

### Noise Point

- [ ] Outlier not belonging to any cluster

**DBSCAN explicitly detects noise — unlike K-Means.**

---

## Phase 7: Cluster Formation

Find Core Point → Expand Neighborhood → Connect Nearby Core Points → Grow Cluster

- [ ] Clusters grow organically

---

## Phase 8: Density Reachability & Connectivity

- [ ] Density-Reachable: connected through dense regions
- [ ] Density-Connected: connected indirectly through dense chains

---

## Phase 9: DBSCAN Algorithm

Select Point → Check Neighborhood → Core Point? → Yes: Expand Cluster / No: Noise/Border → Repeat

---

## Phase 10: Choosing Parameters

### Choosing ε

- [ ] K-Distance Plot: find elbow point in neighbor distances

### Choosing MinPts

- [ ] Rule: MinPts ≥ dimensions + 1
- [ ] Higher dimensions need larger MinPts

---

## Phase 11: Cluster Shapes

- [ ] DBSCAN handles arbitrary, curved, irregular shapes
- [ ] K-Means: spherical only / DBSCAN: flexible

---

## Phase 12: Noise Handling

- [ ] Unlike K-Means, DBSCAN can leave points unclustered
- [ ] Applications: Fraud Detection, Anomaly Detection

---

## Phase 13: Advantages

- [ ] No need for K / Handles arbitrary shapes / Detects outliers / Robust clustering

---

## Phase 14: Failure Modes

- [ ] Struggles with varying densities / Sensitive to ε / High-dimensional problems

---

## Phase 15: Comparisons

### DBSCAN vs K-Means

| | K-Means | DBSCAN |
|---|---|---|
| Method | Centroid-based | Density-based |
| Requires K | Yes | No |
| Outlier Detection | No | Yes |
| Cluster Shape | Spherical | Arbitrary |

### DBSCAN vs Hierarchical Clustering

- [ ] Hierarchical: tree-based / DBSCAN: density expansion

---

## Phase 16: Evaluation Metrics

- [ ] Silhouette Score / Davies-Bouldin Index / Cluster Visualization

---

## Phase 17: Scikit-Learn Implementation

- [ ] DBSCAN()
- [ ] Parameters: eps, min_samples, metric

### Exercises

- [ ] Customer segmentation / Geographic clustering

---

## Phase 18: Visualization

- [ ] Scatter plots / Cluster coloring / Noise highlighting

---

## Phase 19: Real Projects

### Beginner → Simple spatial clustering
### Intermediate → Customer segmentation
### Advanced → Fraud detection, GPS trajectory clustering
### Expert → Large-scale anomaly detection system

---

## Phase 20: Build from Scratch

### Implement

- [ ] Neighborhood Search / Core Point Detection / Cluster Expansion / Noise Detection

---

## Phase 21: Interview Readiness

**Can Explain:** DBSCAN, Density-Based Clustering, ε Parameter, MinPts Parameter, Core/Border/Noise Points, Density Reachability, Cluster Expansion

**Can Compare:** DBSCAN vs K-Means, DBSCAN vs Hierarchical Clustering, Density-Based vs Centroid-Based Clustering

**Can Build:** DBSCAN Pipeline, Outlier Detection Workflow, Production Clustering Solution

---

## Phase 22: Advanced Topics

- [ ] OPTICS / HDBSCAN / Density Peak Clustering

---

## Final Mastery

**Can Explain:** Why DBSCAN Exists, Density-Based Clustering, Cluster Expansion, Noise Detection, Arbitrary Cluster Shapes, Parameter Tuning

**Can Apply:** Choose ε and MinPts, Detect Outliers, Cluster Non-Linear Data, Evaluate Clustering Quality, Build Real-World Clustering Pipelines
