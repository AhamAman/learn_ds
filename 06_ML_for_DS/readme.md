# Machine Learning Mastery Checklists

A phase-by-phase learning roadmap covering core ML concepts, algorithms, and techniques.

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
17. [Feature Engineering](#17-feature-engineering)
18. [Model Serialization & Deployment](#18-model-serialization--deployment)
19. [Model Explainability & Interpretability](#19-model-explainability--interpretability)

---

## 1. Machine Learning Introduction

### Prerequisites
- [ ] Python, NumPy, Pandas, Matplotlib, Seaborn
- [ ] Statistics, Probability, Hypothesis Testing, EDA
- [ ] Basic Algebra, Functions, Coordinates, Gradient Intuition

### Core Concepts
- [ ] Rule-based vs learned systems — what is learning, prediction, intelligence?
- [ ] Supervised / Unsupervised / Reinforcement Learning
- [ ] Classification vs Regression vs Clustering
- [ ] Features, Labels, Samples, Dataset structure (X, y)

### ML Workflow
- [ ] Problem Definition → Data Collection → Cleaning → Feature Engineering → Training → Evaluation → Deployment → Monitoring

### Key Topics
- [ ] Train/Test Split, Data Leakage, Generalization
- [ ] Feature Scaling (Standardization, Normalization)
- [ ] Overfitting, Underfitting, Bias-Variance Tradeoff
- [ ] Cross Validation (K-Fold)
- [ ] Regression Metrics: MAE, MSE, RMSE, R²
- [ ] Classification Metrics: Accuracy, Precision, Recall, F1, Confusion Matrix
- [ ] Scikit-Learn: `fit()`, `predict()`, `transform()`, Pipelines
- [ ] Model Selection, Feature Importance, Explainability
- [ ] Business thinking: connecting technical metrics to business goals
- [ ] Production mindset: model drift, data drift, serving vs training

### Algorithm Roadmap
- [ ] Regression: Linear, Polynomial
- [ ] Classification: Logistic Regression, Decision Trees, Random Forest
- [ ] Unsupervised: K-Means, PCA
- [ ] Deep Learning preview: Neural Networks overview

### Projects
- [ ] Beginner: House Price Prediction, Student Score Prediction
- [ ] Intermediate: Customer Churn, Sales Forecasting
- [ ] Advanced: Fraud Detection, Recommendation Prototype

---

## 2. Linear Regression & Gradient Descent

### Prerequisites
- [ ] Features/Target, Train/Test Split, Regression problems
- [ ] Mean, Variance, Correlation, Scatter Plots
- [ ] Functions, Coordinates, Slope, Basic Algebra

### Core Concepts
- [ ] Scatter plots, correlation (positive/negative/zero), correlation ≠ causation
- [ ] Best-fit line: `y = mx + b` → ML form: `ŷ = w·x + b`
- [ ] Residuals: Actual − Predicted
- [ ] Cost Function (MSE): `(1/n) Σ(y − ŷ)²` — lower = better
- [ ] Optimization: find weights that minimize MSE

### Gradient Descent
- [ ] Gradient = direction of steepest increase; move opposite to descend
- [ ] Update rule: `w = w − α · ∇L`
- [ ] Learning rate (α): too small → slow; too large → overshooting
- [ ] Convergence, local vs global minimum
- [ ] Variants: Batch GD, Stochastic GD, Mini-Batch GD

### Advanced Topics
- [ ] Multiple Linear Regression: `ŷ = w₁x₁ + w₂x₂ + ... + b`
- [ ] Assumptions: linearity, independence, homoscedasticity, normal residuals
- [ ] Failure modes: underfitting, outliers, multicollinearity

### Implementation
- [ ] `LinearRegression()` — `fit()`, `predict()`, `score()`
- [ ] Build from scratch: MSE, gradient calculation, gradient descent

### Projects
- [ ] Beginner: Student Score, Salary Prediction
- [ ] Intermediate: House Prices, Sales Forecasting
- [ ] Advanced: Multiple Regression, Business Revenue Prediction

---

## 3. Regularization

### Prerequisites
- [ ] Linear Regression, Cost Function, MSE, Gradient Descent, Overfitting/Underfitting

### Core Concepts
- [ ] Overfitting: model memorizes instead of learning
- [ ] Bias-Variance tradeoff: balance underfitting vs overfitting
- [ ] Regularization: add a penalty term to the cost function to discourage complexity

### Techniques

| Method | Formula | Effect |
|---|---|---|
| Ridge (L2) | Cost + λ·Σw² | Shrinks weights, keeps all features |
| Lasso (L1) | Cost + λ·Σ\|w\| | Forces some weights to zero (feature selection) |
| Elastic Net | Cost + λ·(L1 + L2) | Best of both; selection + stability |

- [ ] Lambda (λ): small = weak penalty; large = strong penalty, risk of underfitting
- [ ] **Feature scaling is essential** before applying regularization
- [ ] Geometry intuition: Ridge = circular constraint; Lasso = diamond constraint (why zeros appear)

### Implementation
- [ ] `Ridge()`, `Lasso()`, `ElasticNet()` — tune λ with Grid Search + Cross Validation
- [ ] Connection to deep learning: weight decay

### Projects
- [ ] Housing Prices → Customer Revenue → High-Dimensional Regression → Automated Model Selection

---

## 4. Logistic Regression

### Prerequisites
- [ ] Linear Regression, Cost Function, Gradient Descent, Regularization
- [ ] Probability, Conditional Probability, Odds, Logarithms

### Core Concepts
- [ ] Why not linear regression for classification: outputs aren't bounded to [0,1]
- [ ] Odds → Log Odds (Logit): `log(p / 1-p)`
- [ ] Sigmoid function: `σ(z) = 1 / (1 + e⁻ᶻ)` — maps any value to (0, 1)
- [ ] Model: `ŷ = σ(w·x + b)`
- [ ] Decision boundary: P > 0.5 → Class 1; adjust threshold based on use case

### Training
- [ ] Log Loss (Binary Cross Entropy): `−(1/n) Σ [y·log(ŷ) + (1−y)·log(1−ŷ)]`
- [ ] Maximum Likelihood Estimation (MLE)
- [ ] Gradient Descent to minimize log loss

### Evaluation
- [ ] Confusion Matrix: TP, TN, FP, FN
- [ ] Precision, Recall, F1 Score, ROC-AUC
- [ ] Threshold tuning: precision-recall tradeoff

### Advanced Topics
- [ ] Class imbalance: class weighting, oversampling, undersampling
- [ ] Regularized LR: L1 (sparse), L2 (stable)
- [ ] Multiclass: One-vs-Rest (OvR), Softmax Regression
- [ ] Assumptions: independent observations, low multicollinearity, linear log-odds relationship

### Implementation
- [ ] `LogisticRegression()` — `fit()`, `predict()`, `predict_proba()`
- [ ] Build from scratch: sigmoid, log loss, gradient descent

### Projects
- [ ] Beginner: Student Pass/Fail, Loan Approval
- [ ] Intermediate: Customer Churn, Spam Detection
- [ ] Advanced: Fraud Detection, Medical Risk Prediction

---

## 5. Decision Trees

### Prerequisites
- [ ] Features/Target, Train/Test Split, Classification/Regression Metrics
- [ ] Probability, Conditional Probability, Entropy intuition

### Core Concepts
- [ ] Tree anatomy: Root Node, Internal Nodes, Branches, Leaf Nodes
- [ ] Classification trees (majority class) vs Regression trees (mean value)
- [ ] At each node: choose the feature and split that reduces impurity most

### Splitting Criteria
- [ ] **Entropy**: measures disorder; lower = purer node
- [ ] **Information Gain**: reduction in entropy after a split
- [ ] **Gini Impurity**: alternative to entropy, faster to compute
- [ ] Numerical: threshold splits (Age > 30); Categorical: value-based splits

### Controlling Complexity
- [ ] Deep trees overfit (memorize training data)
- [ ] Pruning: `max_depth`, `min_samples_split`, `min_samples_leaf`, `max_features`

### Key Features
- [ ] Feature importance scores (based on impurity reduction)
- [ ] No feature scaling required; handles non-linear data
- [ ] Highly interpretable — tree diagrams show learned rules

### Implementation
- [ ] `DecisionTreeClassifier()`, `DecisionTreeRegressor()`
- [ ] Build from scratch: entropy, information gain, recursive splitting

### Projects
- [ ] Classification: Fraud Detection, Credit Risk, Customer Churn
- [ ] Regression: Sales Forecasting, Revenue Prediction

---

## 6. Random Forest

### Prerequisites
- [ ] Decision Trees (structure, entropy, pruning)
- [ ] Overfitting/Underfitting, Bias/Variance, Cross Validation

### Core Concepts
- [ ] Single trees: high variance, unstable → combine many trees for reliability
- [ ] **Bagging** (Bootstrap Aggregating): train each tree on a different bootstrap sample
- [ ] **Bootstrap sampling**: sample with replacement — each tree sees slightly different data
- [ ] **Random feature selection**: at each split, consider only a subset of features → decorrelates trees

### Aggregation
- [ ] Classification → Majority voting
- [ ] Regression → Average predictions

### Key Topics
- [ ] Bias-Variance: similar bias to single tree, much lower variance
- [ ] Out-of-Bag (OOB) evaluation: free internal validation using unused samples
- [ ] Hyperparameters: `n_estimators`, `max_depth`, `max_features`, `min_samples_leaf`
- [ ] Feature importance via mean impurity decrease
- [ ] Failure modes: slow inference, memory usage, limited interpretability

### Implementation
- [ ] `RandomForestClassifier()`, `RandomForestRegressor()`
- [ ] Tuning: Grid Search / Random Search
- [ ] Explainability: Feature Importance, Permutation Importance, SHAP overview
- [ ] Build from scratch: bootstrap, multiple trees, voting/averaging

### Projects
- [ ] Classification: Fraud Detection, Churn, Risk Assessment
- [ ] Regression: Revenue Forecasting, Demand Forecasting

---

## 7. K-Nearest Neighbors (KNN)

### Prerequisites
- [ ] Features/Target, Classification/Regression, Evaluation Metrics
- [ ] Coordinates, Distance, Geometry basics

### Core Concepts
- [ ] Similarity-based learning: similar inputs → similar outputs
- [ ] **Lazy learning**: no training phase — stores all data, computes at prediction time
- [ ] Algorithm: New point → Find K nearest neighbors → Vote (classification) or Average (regression)

### Distance Metrics
- [ ] Euclidean: `√Σ(xᵢ − yᵢ)²` — straight-line distance
- [ ] Manhattan: `Σ|xᵢ − yᵢ|` — city block distance
- [ ] Minkowski: generalized; Hamming: categorical data

### Choosing K
- [ ] Small K → noisy, high variance; Large K → oversmoothing, high bias
- [ ] Use cross validation to find optimal K
- [ ] Weighted KNN: closer neighbors have more influence

### Important Considerations
- [ ] **Feature scaling is critical** — distance is scale-sensitive
- [ ] Curse of dimensionality: distances lose meaning in high dimensions
- [ ] Slow prediction on large datasets; optimization: KD Trees, Ball Trees

### Implementation
- [ ] `KNeighborsClassifier()`, `KNeighborsRegressor()`
- [ ] Build from scratch: distance functions, neighbor search, voting/averaging

### When to Use
- [ ] Good for: small/medium datasets, local patterns, simple baselines
- [ ] Avoid for: large datasets, high-dimensional data, low-latency production

---

## 8. Stacking & Boosting

### Prerequisites
- [ ] Logistic Regression, Decision Trees, Random Forest, KNN
- [ ] Bagging, Bootstrap Sampling, Bias/Variance, Cross Validation

### Boosting

**Core idea**: train models sequentially — each corrects the errors of the previous.

- [ ] Weak learner (e.g., decision stump) → combine many → strong learner
- [ ] **AdaBoost**: misclassified samples get higher weight; next model focuses on them
- [ ] **Gradient Boosting**: each tree learns the residual errors of the previous model
- [ ] Learning rate (shrinkage): controls contribution per tree
- [ ] **XGBoost**: adds regularization, parallelization, missing value handling
- [ ] **LightGBM**: histogram-based, leaf-wise growth, fast on large datasets
- [ ] **CatBoost**: handles categoricals natively, minimal preprocessing

### Stacking

**Core idea**: combine diverse models using a meta-learner.

- [ ] Level 0 (Base learners): Logistic Regression, Decision Tree, KNN, Random Forest
- [ ] Level 1 (Meta learner): learns how to best combine base predictions
- [ ] Out-of-Fold (OOF) predictions: prevent data leakage in stacking

### Comparison

| | Bagging | Boosting | Stacking |
|---|---|---|---|
| Learning | Parallel | Sequential | Meta-learning |
| Goal | Variance reduction | Bias reduction | Intelligent combination |

### Implementation
- [ ] `AdaBoostClassifier()`, `GradientBoostingClassifier()`
- [ ] `StackingClassifier()`, `StackingRegressor()`
- [ ] Explainability: Feature Importance, SHAP, Permutation Importance

---

## 9. AdaBoost

### Prerequisites
- [ ] Decision Trees, Ensemble concepts, Bagging, Boosting overview

### Core Concepts
- [ ] Weak learner: slightly better than random (e.g., decision stump, depth=1)
- [ ] Training cycle: initialize equal weights → train stump → calculate weighted error → compute learner weight (alpha) → update sample weights → normalize → repeat
- [ ] Misclassified samples get higher weight; correctly classified get lower
- [ ] Final prediction: weighted vote — better learners have more influence

### Key Parameters
- [ ] `n_estimators`: more = more learning, but more overfitting risk
- [ ] `learning_rate`: small = slow/stable; large = fast/overfitting risk

### Comparison

| | Random Forest | AdaBoost |
|---|---|---|
| Learning | Parallel | Sequential |
| Strategy | Independent trees | Error correction |
| Effect | Variance reduction | Bias reduction |

- [ ] vs Gradient Boosting: AdaBoost reweights samples; GBM learns residuals directly
- [ ] Failure modes: sensitive to outliers and noisy data

### Implementation
- [ ] `AdaBoostClassifier()` — `fit()`, `predict()`, `predict_proba()`
- [ ] Build from scratch: sample weights, weighted error, alpha, weight updates, weighted voting

---

## 10. Gradient Boosting

### Prerequisites
- [ ] Decision Trees (regression trees), Ensemble Learning, AdaBoost
- [ ] Loss Functions, Gradient Descent, Gradient Intuition

### Core Concepts
- [ ] Each tree learns the **residual errors** of the previous model
- [ ] Residual = Actual − Prediction
- [ ] More precisely: trees learn **negative gradients** of the loss function (generalizes to any differentiable loss)
- [ ] Sequential architecture: Initial Prediction → Tree 1 (learns residuals) → Tree 2 → ... → Final Prediction

### Key Parameters
- [ ] `learning_rate`: contribution per tree — small = stable; large = faster but overfit risk
- [ ] `n_estimators`: more trees = better fit but more complexity
- [ ] `max_depth`: shallow = weak learners (preferred); deep = stronger but overfits
- [ ] `subsample`: train on random subsets (stochastic GBM) — reduces overfitting

### Loss Functions
- [ ] Regression: MSE, MAE
- [ ] Classification: Log Loss, Cross Entropy

### Implementation
- [ ] `GradientBoostingRegressor()`, `GradientBoostingClassifier()`
- [ ] Tuning: `n_estimators`, `learning_rate`, `max_depth`, `min_samples_leaf`, `subsample`
- [ ] Build from scratch: residual computation, sequential trees, prediction updates

---

## 11. XGBoost

### Prerequisites
- [ ] Gradient Boosting, Decision Trees, Regularization, Loss Functions
- [ ] Basic intuition for first and second derivatives

### Core Concepts
- [ ] XGBoost = Gradient Boosting + engineering + mathematical improvements
- [ ] Objective: minimize Training Loss + Regularization Penalty (good predictions + simple trees)
- [ ] Uses both **first-order gradient** (direction) and **second-order Hessian** (curvature) → faster convergence
- [ ] Post-pruning: grow full tree, then prune weak branches (vs traditional pre-pruning)
- [ ] Handles missing values automatically

### Regularization
- [ ] L1 (alpha) and L2 (lambda) regularization built in
- [ ] `gamma`: minimum gain to allow a split
- [ ] `min_child_weight`: controls leaf size

### Key Parameters

| Category | Parameters |
|---|---|
| Learning | `learning_rate` (eta) |
| Trees | `n_estimators`, `max_depth` |
| Regularization | `gamma`, `reg_alpha`, `reg_lambda` |
| Sampling | `subsample`, `colsample_bytree` |
| Imbalance | `scale_pos_weight` |

### Advanced Features
- [ ] Early stopping: halt when validation score stops improving
- [ ] Feature importance: Weight, Gain, Cover
- [ ] SHAP integration for explainability
- [ ] Multiclass: Softmax / multi-class log loss

### Implementation
- [ ] `XGBClassifier()`, `XGBRegressor()` — sklearn-compatible API
- [ ] Projects: Titanic → Churn → Credit Risk → Fraud Detection → Kaggle pipelines

---

## 12. Dimensionality Reduction

### Prerequisites
- [ ] Vectors, Variance, Covariance, Correlation
- [ ] Features, Feature Engineering, KNN, Logistic Regression

### Why It Matters
- [ ] More features → more noise, slower training, overfitting risk
- [ ] Curse of dimensionality: distances lose meaning as dimensions grow
- [ ] Goals: faster models, better generalization, visualization, storage efficiency

### Feature Selection (keep existing features)

| Method | Techniques |
|---|---|
| Filter | Variance threshold, Correlation, Chi-Square, Mutual Information |
| Wrapper | Forward Selection, Backward Elimination, RFE |
| Embedded | Lasso, Tree Importance, XGBoost Importance |

### Feature Extraction (create new features)

**PCA (Principal Component Analysis)**
- [ ] Finds directions of maximum variance in data
- [ ] PC1 = max variance, PC2 = second max, etc.
- [ ] Explained variance ratio: how much information each component captures
- [ ] Workflow: Standardize → Covariance Matrix → Eigenvectors → Project
- [ ] Choose components via Scree Plot or explained variance curve

**LDA (Linear Discriminant Analysis)**
- [ ] PCA: unsupervised, maximize variance; LDA: supervised, maximize class separation
- [ ] Maximizes between-class variance, minimizes within-class variance

**Non-Linear Methods**
- [ ] **t-SNE**: preserves local neighborhoods; great for visualization, not for features
- [ ] **UMAP**: faster than t-SNE, better structure preservation, good for large datasets

**Autoencoders**
- [ ] Neural network: Encoder → Bottleneck → Decoder
- [ ] Applications: compression, anomaly detection, representation learning

### Implementation
- [ ] `PCA()`, `LinearDiscriminantAnalysis()`, `SelectKBest()`, `RFE()`
- [ ] Helps: KNN, Clustering, Linear Models; Often unnecessary: Trees, XGBoost

---

## 13. Naive Bayes

### Prerequisites
- [ ] Probability, Conditional Probability, Independent Events, Distributions
- [ ] Classification, Features/Labels, Train/Test Split

### Core Concepts
- [ ] Based on Bayes Theorem: `P(A|B) = P(B|A) · P(A) / P(B)`
- [ ] Prior (initial belief) + Likelihood (evidence) → Posterior (updated belief)
- [ ] **"Naive" assumption**: features are independent given the class label
- [ ] Workflow: New sample → calculate class probabilities → predict highest

### Variants

| Type | Class | Data |
|---|---|---|
| Gaussian NB | `GaussianNB` | Continuous numerical (Age, Salary) |
| Multinomial NB | `MultinomialNB` | Word counts, text |
| Bernoulli NB | `BernoulliNB` | Binary features (word present/absent) |
| Complement NB | `ComplementNB` | Imbalanced text datasets |

- [ ] **Laplace Smoothing**: prevents zero probabilities for unseen feature values
- [ ] Text preprocessing: Tokenization, Stop Words, Stemming, Bag of Words, TF-IDF

### Comparison with Logistic Regression

| | Naive Bayes | Logistic Regression |
|---|---|---|
| Approach | Probabilistic | Weight learning |
| Independence assumption | Yes | No |
| Works well with small data | Yes | Less so |

### Projects
- [ ] Beginner: Spam Detection; Intermediate: News Classification
- [ ] Advanced: Sentiment Analysis; Expert: Document Categorization

---

## 14. Support Vector Machine (SVM)

### Prerequisites
- [ ] Coordinates, Vectors, Dot Product, Distance
- [ ] Logistic Regression, KNN, Decision Trees

### Core Concepts
- [ ] Goal: find the decision boundary with the **largest margin**
- [ ] Margin = distance from boundary to nearest points (support vectors)
- [ ] Support vectors: the points that define the classifier; removing others barely changes it
- [ ] **Hard Margin**: perfect separation (rare in practice); **Soft Margin**: allows some errors

### Regularization Parameter C

| C | Effect |
|---|---|
| Large | Fewer errors, smaller margin, more overfitting |
| Small | Larger margin, more tolerance, better generalization |

### Kernels (for non-linear data)
- [ ] **Linear**: fast; for linearly separable or high-dimensional text
- [ ] **Polynomial**: captures feature interactions
- [ ] **RBF** (Radial Basis Function): most common; handles complex boundaries

### Gamma Parameter (RBF)
- [ ] Small gamma → smooth, simpler boundary
- [ ] Large gamma → complex boundary, overfitting risk

### Key Considerations
- [ ] **Feature scaling is critical** (distance-based)
- [ ] SVM for regression: SVR (Support Vector Regression)
- [ ] Slow on very large datasets; powerful for high-dimensional data (e.g., text)

### Implementation
- [ ] `SVC()`, `SVR()` — tune C, gamma, kernel via Grid Search
- [ ] Projects: Iris → Spam Detection → Churn → High-Dimensional Text Classification

---

## 15. Hierarchical Clustering

### Prerequisites
- [ ] Distance Metrics (Euclidean, Manhattan), Similarity vs Dissimilarity
- [ ] Supervised vs Unsupervised Learning

### Core Concepts
- [ ] Doesn't require knowing K upfront — builds a tree of clusters instead
- [ ] **Agglomerative (bottom-up)**: each point starts as its own cluster → merge the closest repeatedly
- [ ] **Divisive (top-down)**: start with one cluster → split repeatedly (less common)

### Linkage Methods

| Linkage | Distance Measure | Notes |
|---|---|---|
| Single | Min distance | Captures irregular shapes; prone to chaining |
| Complete | Max distance | Compact clusters; sensitive to outliers |
| Average | Average of all pairs | Balanced, general-purpose |
| Ward | Minimize variance increase | Best default; compact, business-friendly |

### Dendrogram
- [ ] Tree diagram showing all merge steps
- [ ] Cut at a height to choose number of clusters
- [ ] Read branches, merge heights, and leaves

### Evaluation
- [ ] Silhouette Score, Davies-Bouldin Index, Calinski-Harabasz Index
- [ ] Feature scaling is critical (distance-based)

### Comparison

| | K-Means | Hierarchical |
|---|---|---|
| Requires K | Yes | No |
| Speed | Fast | Slower |
| Structure | Centroid-based | Tree-based |
| Interpretability | Lower | Higher |

### Implementation
- [ ] `AgglomerativeClustering()` — `n_clusters`, `linkage`, `metric`
- [ ] Applications: Customer Segmentation, Gene Clustering, Document Grouping

---

## 16. DBSCAN

### Prerequisites
- [ ] Distance metrics, Neighborhood Radius
- [ ] K-Means, Hierarchical Clustering basics

### Core Concepts
- [ ] **Density-based**: clusters = dense regions; sparse regions = noise/separation
- [ ] Does not require K upfront; naturally detects outliers

### Parameters
- [ ] **ε (epsilon)**: neighborhood radius — small = tiny clusters; large = over-merging
- [ ] **MinPts**: minimum neighbors to be a core point — higher = denser clusters required

### Point Types
- [ ] **Core Point**: ≥ MinPts neighbors within ε
- [ ] **Border Point**: within ε of a core point, but fewer than MinPts neighbors itself
- [ ] **Noise Point**: outlier; belongs to no cluster

### Algorithm
Select point → Check neighborhood → Core? → Yes: expand cluster / No: mark as noise/border → Repeat

### Parameter Selection
- [ ] ε: use K-distance plot, find the elbow
- [ ] MinPts: rule of thumb = dimensions + 1 (or higher for noisy data)

### Comparison

| | K-Means | DBSCAN |
|---|---|---|
| Method | Centroid-based | Density-based |
| Requires K | Yes | No |
| Outlier detection | No | Yes |
| Cluster shape | Spherical | Arbitrary |

- [ ] Failure modes: struggles with varying densities, sensitive to ε, poor in high dimensions

### Implementation
- [ ] `DBSCAN()` — `eps`, `min_samples`, `metric`
- [ ] Applications: GPS trajectory clustering, Fraud/Anomaly Detection, Customer Segmentation
- [ ] Advanced: OPTICS, HDBSCAN

---

## 17. Feature Engineering

### Why It Matters
Raw data is rarely ready for ML. Feature engineering transforms raw inputs into meaningful signals that improve model performance.

### Mindset
- [ ] Domain knowledge often creates the most useful features
- [ ] Ask: does this feature contain predictive information?
- [ ] Never use future information (data leakage)

### Missing Value Handling
- [ ] Numerical: mean, median, constant, KNN, or iterative imputation
- [ ] Categorical: mode or "Unknown" constant
- [ ] Know when mean imputation fails (skewed data, outliers)

### Categorical Encoding

| Method | When to Use |
|---|---|
| One-Hot Encoding | Nominal categories, low cardinality |
| Label Encoding | Only for tree models (ordinal implied) |
| Ordinal Encoding | When categories have a natural order |
| Target Encoding | High-cardinality; careful of leakage |
| Frequency Encoding | High-cardinality, no leakage risk |
| Hash Encoding | Very high-cardinality |

### Numerical Transformations
- [ ] Log (`log1p`), Square Root, Box-Cox, Yeo-Johnson — reduce skewness and outlier influence
- [ ] Binning: convert continuous to categorical ranges

### Scaling & Normalization

| Method | Formula | Use When |
|---|---|---|
| Standardization | `(x − mean) / std` | Linear models, PCA, SVM, NNs |
| Min-Max | `(x − min) / (max − min)` | Neural networks, bounded range |
| Robust Scaling | `(x − median) / IQR` | Data with outliers |

### Feature Construction
- [ ] Derived features: Profit = Revenue − Cost
- [ ] Ratios: Debt/Income, Profit Margin
- [ ] Business KPIs: Customer Lifetime Value
- [ ] Interaction features: Age × Income, City × Product cross-features
- [ ] Polynomial features: x², xy, y² — capture non-linear relationships

### Date & Time Features
- [ ] Extract: year, month, day, weekday, hour, quarter, week of year
- [ ] Cyclical encoding: `sin()`/`cos()` for month, hour, day of week
- [ ] Lag features (yesterday's sales), rolling features (7-day average)

### Text Features
- [ ] Bag of Words, Count Vectorizer, TF-IDF, N-grams
- [ ] Word embeddings: Word2Vec, GloVe, FastText, BERT

### Aggregation Features
- [ ] Group-by statistics: total orders, avg order value, max/min per customer

### Dimensionality Reduction
- [ ] Feature Selection: filter, wrapper, embedded methods
- [ ] Feature Extraction: PCA, LDA, SVD, Autoencoders
- [ ] See [Section 12](#12-dimensionality-reduction) for full details

### Model-Specific Notes
- [ ] **Trees**: minimal scaling needed; handle raw features well
- [ ] **Linear models**: require scaling, encoding, multicollinearity handling
- [ ] **Deep learning**: embeddings, learned representations, sequence features

### Production Pipeline
- [ ] `sklearn.Pipeline`, `ColumnTransformer`
- [ ] Feature versioning, monitoring, drift detection
- [ ] Feature stores: Feast, Tecton, Hopsworks (training features = serving features)

### Projects
- [ ] Titanic (missing values, encoding, feature creation)
- [ ] House Prices (selection, PCA, transformations)
- [ ] Customer Churn (aggregations, ratios, target encoding)
- [ ] Credit Risk (WOE, IV, binning)

---

## 18. Model Serialization & Deployment

### Why It Matters
Train once, save, reload, and predict — without retraining.

### Core Concepts
- [ ] **Serialization**: Python object → bytes → file
- [ ] **Deserialization**: file → bytes → Python object
- [ ] A model is just: learned parameters + configuration

### Serialization Libraries

| Tool | Best For | Notes |
|---|---|---|
| `pickle` | General Python objects | Built-in; Python-only; security risks |
| `joblib` | sklearn models, large NumPy arrays | Faster, better compression |
| `cloudpickle` | Lambdas, custom functions | Distributed systems (Spark, Ray) |

### Saving Full Pipelines
- [ ] Save the entire pipeline (Scaler + Encoder + Model) — not just the model
- [ ] Prevents training/inference mismatch
- [ ] `joblib.dump(pipeline, "pipeline.joblib")`

### Framework-Specific Formats

| Framework | Format | Save Method |
|---|---|---|
| TensorFlow/Keras | SavedModel or `.h5` / `.keras` | `model.save()` |
| PyTorch | `.pt` (weights only) | `torch.save(model.state_dict())` |
| TorchScript | Cross-platform | Deploy without Python (mobile, C++) |
| ONNX | Universal | Train anywhere, run anywhere |

### Model Versioning & Registry
- [ ] Version models with Git, DVC, or MLflow
- [ ] Track: hyperparameters, dataset version, metrics
- [ ] Registries (MLflow, SageMaker, Vertex): track Production / Staging / Archived models

### MLflow
- [ ] Experiment tracking, Model Registry, Artifact Storage
- [ ] Concepts: Run, Experiment, Artifact, Registry

### Inference Pipeline
Input → Validation → Transformation → Prediction → Output

### Production Considerations
- [ ] Version drift, data drift, dependency drift, schema drift
- [ ] Monitor: latency, accuracy, throughput

### Mastery Checklist
- [ ] Beginner: save/load with pickle and joblib
- [ ] Intermediate: save full pipelines, version models
- [ ] Advanced: ONNX, MLflow, deploy serialized models
- [ ] Expert: build model registries, design artifact systems

---

## 19. Model Explainability & Interpretability

### Why It Matters
A model that says "Loan Rejected" must be able to say *why* — required in banking, healthcare, insurance, legal, and government.

**Interpretability**: model is transparent by design (Linear Regression, small Decision Tree)
**Explainability**: post-hoc methods needed (Random Forest, XGBoost, Neural Networks)

### White Box vs Black Box

| White Box | Black Box |
|---|---|
| Linear/Logistic Regression | Random Forest |
| Small Decision Trees | XGBoost, LightGBM |
| — | Neural Networks, Transformers |

### Feature Importance Methods

| Method | Scope | Works With |
|---|---|---|
| Coefficient analysis | Global | Linear/Logistic Regression |
| Tree-based importance (Gini/Gain) | Global | Trees, Random Forest, XGBoost |
| Permutation Importance | Global | Any model |
| PDP (Partial Dependence Plot) | Global | Any model |
| ICE (Individual Conditional Expectation) | Local + Global | Any model |

- [ ] Permutation Importance: shuffle a feature → measure accuracy drop → bigger drop = more important
- [ ] PDP: shows average model behavior as one feature varies
- [ ] ICE: like PDP but per individual — reveals heterogeneity PDP hides

### LIME
- [ ] Local Interpretable Model-Agnostic Explanations
- [ ] Fit a simple local model around a single prediction to explain it
- [ ] Model-agnostic; can be unstable across runs

### SHAP
- [ ] SHapley Additive exPlanations — from game theory
- [ ] Fairly distributes prediction among features: Base value + contributions = prediction
- [ ] Consistent, locally accurate, model-agnostic

| SHAP Variant | For |
|---|---|
| TreeSHAP | Random Forest, XGBoost, LightGBM — fast and exact |
| DeepSHAP | Neural Networks |
| KernelSHAP | Any model (slow) |

**SHAP Visualizations**
- [ ] Summary plot: importance + direction for all features
- [ ] Force plot: single prediction breakdown
- [ ] Waterfall plot: base value → contributions → final prediction
- [ ] Dependence plot: feature value vs SHAP contribution

### Counterfactual Explanations
- [ ] "What would need to change to get a different outcome?"
- [ ] Example: "If income were ₹10,000 higher → Loan Approved"
- [ ] Actionable explanations for end users

### Domain-Specific Explainability
- [ ] **NLP**: Attention visualization, SHAP for text, LIME for text, Integrated Gradients
- [ ] **Computer Vision**: Saliency Maps, Grad-CAM, Occlusion Maps
- [ ] **Deep Learning**: SHAP, DeepSHAP, LIME, Integrated Gradients

### Fairness & Bias Analysis
- [ ] Does the model discriminate by gender, race, region, age?
- [ ] Metrics: Demographic Parity, Equal Opportunity, Equalized Odds

### Production & Regulatory
- [ ] Monitor: feature importance drift, SHAP drift, data drift
- [ ] Log: prediction + explanation + timestamp
- [ ] Regulations: GDPR, EU AI Act, Banking regulations require explainable decisions

### Mastery Checklist
- [ ] Beginner: feature importance, PDP, SHAP basics
- [ ] Intermediate: use SHAP and LIME, explain individual predictions
- [ ] Advanced: explain deep learning, counterfactuals, measure fairness
- [ ] Expert: build explainability platforms, production XAI systems, explain SHAP mathematically