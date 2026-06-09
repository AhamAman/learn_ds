# Matplotlib & Seaborn Mastery Checklists

> A complete, phase-by-phase learning roadmap covering data visualization with Matplotlib and Seaborn — from fundamentals to publication-quality graphics and production EDA workflows.

---

## Table of Contents

1. [Matplotlib](#1-matplotlib)
2. [Seaborn](#2-seaborn)

---

# 1. Matplotlib

---

## Phase 0: Prerequisites

### Python Fundamentals

- [ ] Functions & Modules
- [ ] OOP Basics (classes, methods)
- [ ] List comprehensions

### NumPy

- [ ] Arrays & Vectorized Operations
- [ ] Shape and Dimensions
- [ ] Boolean indexing

### Data Fundamentals

- [ ] Tables & DataFrames
- [ ] Time Series
- [ ] Distributions

---

## Phase 1: Why Visualization Exists

### The Problem

- [ ] Large datasets are hard to understand as tables
- [ ] Tables hide patterns, trends, and outliers
- [ ] Humans recognize visual patterns far faster than numbers

### First Principles

- [ ] What is data visualization?
- [ ] Why charts exist
- [ ] Choosing the right chart for the right question

### Chart Purpose Categories

- [ ] Trend — how does something change over time?
- [ ] Comparison — how do things differ?
- [ ] Distribution — how is data spread?
- [ ] Relationship — how do variables relate?
- [ ] Composition — what makes up the whole?

### Understand

- [ ] A chart should answer one clear question
- [ ] Wrong chart type = miscommunication
- [ ] Simplicity beats complexity in visualization

---

## Phase 2: Matplotlib Fundamentals

### Setup

- [ ] `import matplotlib.pyplot as plt`
- [ ] Create first plot
- [ ] Inline display in notebooks (`%matplotlib inline`)

### Core Functions

- [ ] `plt.plot()`
- [ ] `plt.show()`

### Understand

- [ ] Figure: the whole canvas
- [ ] Axes: a single plot within the figure
- [ ] Axis: the x or y number line

**Exercises**
- [ ] Plot a simple line chart from a list

---

## Phase 3: Figure & Axes Model

### Core Architecture

- [ ] Figure (top-level container)
- [ ] Axes (individual plot)
- [ ] Axis (x-axis, y-axis)
- [ ] Artist (everything drawn on figure)

### Learn

- [ ] `plt.figure()` — create figure
- [ ] `plt.subplots()` — create figure + axes together
- [ ] `fig, ax = plt.subplots()` pattern

### Two APIs

- [ ] pyplot API (stateful, quick plots): `plt.plot()`
- [ ] Object-Oriented API (recommended): `ax.plot()`

### Understand

- [ ] When to use each API
- [ ] Why OO API is better for complex figures

**Exercises**
- [ ] Create figure with multiple axes
- [ ] Use OO API for a two-panel chart

---

## Phase 4: Line Charts

### Learn

- [ ] `ax.plot(x, y)`
- [ ] Multiple lines on same axes

### Customization

- [ ] Labels: `ax.set_xlabel()`, `ax.set_ylabel()`
- [ ] Title: `ax.set_title()`
- [ ] Legend: `ax.legend()`
- [ ] Line color, style, width, marker

**Exercises**
- [ ] Temperature tracker over time
- [ ] Multi-line stock price graph

---

## Phase 5: Scatter Plots

### Learn

- [ ] `ax.scatter(x, y)`
- [ ] Color by category (`c=`)
- [ ] Size by value (`s=`)

### Understand

- [ ] Visualizing correlation
- [ ] Spotting outliers
- [ ] Overplotting and solutions (alpha, jitter) (Added)

**Exercises**
- [ ] Height vs Weight scatter plot
- [ ] Color-coded scatter by category

---

## Phase 6: Bar Charts

### Learn

- [ ] `ax.bar()` — vertical bars
- [ ] `ax.barh()` — horizontal bars
- [ ] Grouped bar charts (Added)
- [ ] Stacked bar charts (Added)

### Understand

- [ ] Category comparison
- [ ] When to use horizontal vs vertical

**Exercises**
- [ ] Product sales chart
- [ ] Grouped comparison chart

---

## Phase 7: Histograms

### Learn

- [ ] `ax.hist()`
- [ ] Bin count and bin edges
- [ ] Density parameter (`density=True`)

### Understand

- [ ] Distribution shape
- [ ] Bins: too few vs too many (Added)
- [ ] Frequency vs density

**Exercises**
- [ ] Exam score distribution
- [ ] Compare two distributions on same axes

---

## Phase 8: Pie Charts

### Learn

- [ ] `ax.pie()`
- [ ] Explode, labels, percentages

### Understand

- [ ] Part-to-whole relationships
- [ ] When NOT to use pie charts (Added — hard to compare slices)
- [ ] Prefer bar charts for comparisons

**Exercises**
- [ ] Budget allocation chart

---

## Phase 9: Subplots & Layouts

### Learn

- [ ] `plt.subplot()` — single subplot
- [ ] `plt.subplots(nrows, ncols)` — grid of subplots
- [ ] `fig.add_subplot()` — manual control

### Layouts

- [ ] Row and column grids
- [ ] Shared axes (`sharex=`, `sharey=`)
- [ ] `GridSpec` for complex layouts (Added)
- [ ] `constrained_layout=True` for spacing (Added)

**Exercises**
- [ ] 2×2 dashboard layout
- [ ] Shared-axis time series comparison

---

## Phase 10: Styling & Customization

### Learn

- [ ] Colors (named, hex, RGB)
- [ ] Line styles (solid, dashed, dotted)
- [ ] Markers
- [ ] `plt.style.use()` — built-in styles (Added)
- [ ] `mpl.rcParams` — global defaults (Added)

### Labels & Titles

- [ ] `ax.set_xlabel()` / `ax.set_ylabel()` / `ax.set_title()`
- [ ] Font size and weight
- [ ] `fig.suptitle()` — figure-level title (Added)

**Exercises**
- [ ] Professional report-ready chart
- [ ] Apply ggplot or seaborn style

---

## Phase 11: Legends & Annotations

### Learn

- [ ] `ax.legend()` — auto or manual
- [ ] Legend placement and style
- [ ] `ax.annotate()` — arrow + text
- [ ] `ax.text()` — plain text label (Added)
- [ ] `ax.axhline()` / `ax.axvline()` — reference lines (Added)
- [ ] `ax.axhspan()` / `ax.axvspan()` — shaded regions (Added)

### Understand

- [ ] Highlighting key data points
- [ ] Adding context to charts

**Exercises**
- [ ] Annotated stock chart with key events
- [ ] Chart with reference threshold line

---

## Phase 12: Axis Control

### Learn

- [ ] `ax.set_xlim()` / `ax.set_ylim()` — zoom
- [ ] `ax.set_xticks()` / `ax.set_yticks()` — tick positions
- [ ] `ax.set_xticklabels()` — custom labels
- [ ] Log scale: `ax.set_xscale('log')`
- [ ] `ax.invert_xaxis()` (Added)
- [ ] `ticker` module for formatting (Added)

**Exercises**
- [ ] Scientific data with log scale
- [ ] Custom tick labels (months, categories)

---

## Phase 13: Date & Time Visualization

### Learn

- [ ] Date axes with `matplotlib.dates`
- [ ] `DateFormatter` and `DateLocator`
- [ ] Pandas datetime integration (Added)

**Exercises**
- [ ] Monthly sales trend
- [ ] Time-series with formatted date axis

---

## Phase 14: Statistical Visualization

### Learn

- [ ] Box Plot: `ax.boxplot()`
- [ ] Violin Plot: `ax.violinplot()`
- [ ] Error Bars: `ax.errorbar()`
- [ ] Step plot: `ax.step()` (Added)
- [ ] Fill between: `ax.fill_between()` (Added — confidence bands)

### Understand

- [ ] Median, quartiles, IQR from box plots
- [ ] Distribution shape from violin plots
- [ ] Uncertainty representation with error bars

**Exercises**
- [ ] Student score box plot by group
- [ ] Confidence band on time series

---

## Phase 15: Heatmaps & Images

### Learn

- [ ] `ax.imshow()` — display image or matrix
- [ ] Color maps (`cmap=`)
- [ ] `plt.colorbar()` (Added)
- [ ] `ax.pcolormesh()` (Added — for grid data)

### Understand

- [ ] Pixel grids and color mapping
- [ ] Diverging vs sequential colormaps
- [ ] Perceptually uniform colormaps (viridis, plasma) (Added)

**Exercises**
- [ ] Correlation heatmap
- [ ] Display image data

---

## Phase 16: 3D Plotting

### Learn

- [ ] `from mpl_toolkits.mplot3d import Axes3D`
- [ ] Surface Plot: `ax.plot_surface()`
- [ ] 3D Scatter: `ax.scatter()`
- [ ] 3D Line: `ax.plot3D()` (Added)
- [ ] Contour Plot: `ax.contour()` (Added)

**Exercises**
- [ ] Terrain / function surface visualization
- [ ] 3D data exploration

---

## Phase 17: Animation

### Learn

- [ ] `FuncAnimation` from `matplotlib.animation`
- [ ] Frame update function
- [ ] `ArtistAnimation` (Added — precomputed frames)
- [ ] Saving animations as GIF/MP4 (Added)

**Exercises**
- [ ] Animated sine wave
- [ ] Animated scatter plot

---

## Phase 18: Saving Figures

### Learn

- [ ] `fig.savefig()`
- [ ] Formats: PNG, SVG, PDF, EPS

### Quality Control

- [ ] DPI (dots per inch)
- [ ] `bbox_inches='tight'` to avoid clipping (Added)
- [ ] Transparent background: `transparent=True` (Added)

**Exercises**
- [ ] Export publication-quality figures at 300 DPI

---

## Phase 19: Performance

### Understand

- [ ] Rendering cost with large datasets
- [ ] Raster vs vector formats

### Learn

- [ ] Downsampling before plotting (Added)
- [ ] `ax.plot()` vs `ax.scatter()` performance difference (Added)
- [ ] Blitting for animations (Added)

**Exercises**
- [ ] Plot 1M-point dataset efficiently

---

## Phase 20: Matplotlib Internals

### Architecture

- [ ] Artist Model (Figure, Axes, Line2D, Text are all Artists)
- [ ] Figure Canvas
- [ ] Renderer

### Backend System

- [ ] Interactive backends (TkAgg, Qt5Agg)
- [ ] Non-interactive backends (Agg for file output)
- [ ] Setting backends: `matplotlib.use()`

### Understand

- [ ] How Matplotlib draws: Artist → Canvas → Renderer
- [ ] Why understanding internals helps debugging

---

## Phase 21: Ecosystem Integration

### Learn

- [ ] Matplotlib + NumPy (direct array plotting)
- [ ] Matplotlib + Pandas (`df.plot()` uses Matplotlib)
- [ ] Matplotlib + Seaborn (Seaborn returns Axes objects)
- [ ] Matplotlib + Scikit-Learn (plotting decision boundaries) (Added)
- [ ] Matplotlib + SciPy (scientific plots) (Added)

---

## Phase 22: Visualization Design Principles

### Principles

- [ ] Clarity — one message per chart
- [ ] Simplicity — remove chart junk
- [ ] Data-Ink Ratio (Tufte) — maximize data, minimize ink
- [ ] Truthful scaling — don't truncate axes misleadingly (Added)
- [ ] Color accessibility — colorblind-friendly palettes (Added)

### Avoid

- [ ] Misleading charts (truncated y-axis, 3D pie charts)
- [ ] Excessive decoration (grid lines, backgrounds)
- [ ] Overloaded charts (too many series)

**Exercises**
- [ ] Redesign a poor visualization
- [ ] Audit a chart for misleading elements

---

## Phase 23: Real Projects

### Beginner
- [ ] Weather Dashboard
- [ ] Expense Tracker Charts

### Intermediate
- [ ] Sales Analytics Dashboard
- [ ] Financial Analytics Charts

### Advanced
- [ ] Scientific Visualization Tool
- [ ] Data Analysis Report Generator

### Expert
- [ ] Custom Plotting Library
- [ ] Research Publication Figures
- [ ] Interactive Dashboard (Added — with ipywidgets)

---

## Final Mastery

**Can Explain:** Figure, Axes, Artist Model, Renderer, Backends, pyplot vs OO API, Histograms, Scatter Plots, Box Plots, Animation Pipeline, Data-Ink Ratio

**Can Build:** Dashboards, Scientific Visualizations, Reports, Publication-Quality Graphics, Animated Charts, Custom Visualization Tools

---

# 2. Seaborn

---

## Phase 0: Prerequisites

### Python Fundamentals

- [ ] Functions & Modules
- [ ] Dictionaries
- [ ] List comprehensions

### NumPy

- [ ] Arrays & Broadcasting
- [ ] Aggregations

### Pandas

- [ ] DataFrame creation and indexing
- [ ] Filtering & GroupBy
- [ ] Missing Values handling
- [ ] Long vs wide format data (Added — Seaborn prefers long format)

### Matplotlib

- [ ] Figure & Axes model
- [ ] Plot basics
- [ ] OO API

---

## Phase 1: Why Seaborn Exists

### The Problem

- [ ] Matplotlib requires lots of boilerplate code
- [ ] Statistical charts (CI, regression) are tedious to build manually
- [ ] DataFrames should integrate directly with plotting

### First Principles

- [ ] Visualization vs Statistical Visualization
- [ ] Exploratory Data Analysis (EDA) workflow
- [ ] Data Storytelling

### Understand

- [ ] Seaborn is built on top of Matplotlib
- [ ] Seaborn works natively with DataFrames
- [ ] Seaborn handles statistical aggregation automatically
- [ ] Every Seaborn plot returns a Matplotlib Axes (or FacetGrid) object

---

## Phase 2: Seaborn Fundamentals

### Setup

- [ ] `import seaborn as sns`
- [ ] `sns.set_theme()` — apply default theme
- [ ] `sns.load_dataset()` — built-in datasets for practice

### Core Concepts

- [ ] Figure-level functions (return FacetGrid): `relplot()`, `catplot()`, `displot()`
- [ ] Axes-level functions (return Axes): `scatterplot()`, `boxplot()`, `histplot()`

### Understand

- [ ] When to use figure-level vs axes-level
- [ ] Figure-level → use for faceting and automatic layout
- [ ] Axes-level → use when embedding in custom Matplotlib figures

**Exercises**
- [ ] First Seaborn plot using a built-in dataset

---

## Phase 3: Understanding Data Types for Visualization

### Numerical Data

- [ ] Continuous variables
- [ ] Discrete variables

### Categorical Data

- [ ] Nominal (no order)
- [ ] Ordinal (ordered)

### Relationship Matrix

| X | Y | Best Chart |
|---|---|---|
| Numerical | Numerical | Scatter, Line |
| Categorical | Numerical | Bar, Box, Violin |
| Categorical | Categorical | Count, Heatmap |
| Numerical | — | Histogram, KDE |

### Understand

- [ ] Choosing the right chart based on data types
- [ ] How `hue=` adds a third variable to any plot

---

## Phase 4: Distribution Plots

### Learn

- [ ] `sns.histplot()` — histogram with optional KDE
- [ ] `sns.kdeplot()` — smooth density curve
- [ ] `sns.displot()` — figure-level distribution
- [ ] `sns.ecdfplot()` — empirical CDF (Added)
- [ ] `sns.rugplot()` — individual data marks (Added)

### Understand

- [ ] Distribution shape, center, spread
- [ ] Kernel density estimation intuition
- [ ] Bandwidth effect on KDE (Added)
- [ ] Overlapping distributions with `hue=`

**Exercises**
- [ ] Analyze exam score distribution
- [ ] Compare salary distributions by gender

---

## Phase 5: Relationship Plots

### Learn

- [ ] `sns.scatterplot()` — point cloud
- [ ] `sns.lineplot()` — line with CI band
- [ ] `sns.relplot()` — figure-level wrapper

### Understand

- [ ] Correlation direction and strength
- [ ] Trends over time
- [ ] Using `hue=`, `size=`, `style=` for extra dimensions (Added)

**Exercises**
- [ ] Height vs Weight scatter
- [ ] Sales trends with confidence bands

---

## Phase 6: Categorical Plots

### Learn

- [ ] `sns.barplot()` — mean with CI bars
- [ ] `sns.countplot()` — frequency of categories
- [ ] `sns.pointplot()` — means connected by lines (Added)
- [ ] `sns.stripplot()` — jittered data points (Added)
- [ ] `sns.swarmplot()` — non-overlapping points (Added)
- [ ] `sns.catplot()` — figure-level categorical

### Understand

- [ ] Difference between barplot (aggregated) and countplot (frequency)
- [ ] When to show raw data vs summary statistics

**Exercises**
- [ ] Product sales by category
- [ ] Count of customers by region

---

## Phase 7: Box Plots & Violin Plots

### Learn

- [ ] `sns.boxplot()` — five-number summary + outliers
- [ ] `sns.violinplot()` — distribution shape + box
- [ ] `sns.boxenplot()` — letter-value plot for large data (Added)

### Understand

- [ ] Median / Q1 / Q3 / IQR / whiskers / outliers from box plot
- [ ] Distribution shape from violin plot
- [ ] Box plot vs violin plot: when each is preferred

**Exercises**
- [ ] Salary comparison by department
- [ ] Score distribution by study group

---

## Phase 8: Pairwise Analysis

### Learn

- [ ] `sns.pairplot()` — all pairs of variables
- [ ] `kind=` parameter (scatter, kde, hist, reg)
- [ ] `diag_kind=` for diagonal plots
- [ ] `hue=` for color by category

### Understand

- [ ] Quick multi-variable exploration
- [ ] Identifying correlated features
- [ ] Distribution on diagonal vs relationship off diagonal

**Exercises**
- [ ] Iris dataset full pairplot
- [ ] Feature exploration before ML modeling

---

## Phase 9: Correlation Heatmaps

### Learn

- [ ] `sns.heatmap()` — matrix visualization
- [ ] `annot=True` — show values in cells
- [ ] `fmt=` — number format
- [ ] `cmap=` — colormap
- [ ] `mask=` — hide upper triangle (Added)
- [ ] `vmin=`, `vmax=` — fix color scale (Added)

### Understand

- [ ] Correlation matrix interpretation
- [ ] Positive / Negative / Zero correlation
- [ ] Diverging colormap for correlation (Added — center at 0)

**Exercises**
- [ ] Feature correlation study on a dataset
- [ ] Masked upper triangle heatmap

---

## Phase 10: Regression Visualization

### Learn

- [ ] `sns.regplot()` — scatter + regression line (axes-level)
- [ ] `sns.lmplot()` — regression with faceting (figure-level)
- [ ] `sns.residplot()` — regression residuals (Added)

### Understand

- [ ] Linear relationship visualization
- [ ] Confidence band around regression line
- [ ] Non-linear regression with `order=` (Added)
- [ ] Residual analysis for model diagnostics (Added)

**Exercises**
- [ ] House size vs price regression
- [ ] Faceted regression by category

---

## Phase 11: Faceting

### Learn

- [ ] `col=` — one column per category
- [ ] `row=` — one row per category
- [ ] `hue=` — color dimension
- [ ] `FacetGrid` — manual faceting
- [ ] `col_wrap=` — limit columns per row (Added)

### Understand

- [ ] Small multiples principle
- [ ] Multi-dimensional data exploration in one figure

**Exercises**
- [ ] Regional sales comparison across quarters
- [ ] Distribution by multiple categories

---

## Phase 12: Styling & Themes

### Learn

- [ ] `sns.set_theme()` — overall theme
- [ ] `sns.set_style()` — background style
- [ ] `sns.set_context()` — scale for output (paper, notebook, talk, poster) (Added)
- [ ] `sns.set_palette()` — color palette

### Styles

- [ ] whitegrid / darkgrid / white / ticks

### Context Scaling

- [ ] paper → smallest elements
- [ ] notebook → default
- [ ] talk → larger for presentations
- [ ] poster → largest

**Exercises**
- [ ] Style a chart for a business presentation
- [ ] Style a chart for a research paper

---

## Phase 13: Color Theory & Palettes

### Learn

- [ ] `sns.color_palette()` — view/create palette
- [ ] `sns.palplot()` — visualize palette

### Palette Types

- [ ] Sequential — one color gradient (low to high)
- [ ] Diverging — two-color gradient (negative to positive)
- [ ] Qualitative — distinct colors for categories

### Understand

- [ ] Match palette type to data type
- [ ] Colorblind-friendly palettes (Added — colorblind, crest, mako)
- [ ] Perceptually uniform palettes (Added — viridis, rocket)

**Exercises**
- [ ] Design an accessible chart with colorblind palette

---

## Phase 14: Figure-Level APIs

### Learn

- [ ] `sns.relplot()` — relationships
- [ ] `sns.catplot()` — categorical
- [ ] `sns.displot()` — distributions
- [ ] `sns.jointplot()` — bivariate + marginal distributions (Added)
- [ ] `sns.clustermap()` — hierarchical clustering heatmap (Added)

### Understand

- [ ] Figure-level functions return `FacetGrid` or `JointGrid`
- [ ] Access underlying axes via `.axes`, `.ax_joint` etc.
- [ ] Automatic figure sizing and layout

---

## Phase 15: Axes-Level APIs

### Learn

- [ ] `sns.scatterplot()` / `sns.lineplot()`
- [ ] `sns.boxplot()` / `sns.violinplot()`
- [ ] `sns.barplot()` / `sns.histplot()`

### Understand

- [ ] Returns Matplotlib Axes object
- [ ] Can be embedded in any Matplotlib figure
- [ ] Use `ax=` parameter to target specific subplot

**Exercises**
- [ ] Embed Seaborn plot in Matplotlib subplot grid

---

## Phase 16: Statistical Estimation

### Learn

- [ ] `estimator=` — function applied before plotting (default: mean)
- [ ] `errorbar=` — CI, SD, or SE (Added — replaces ci= in modern Seaborn)
- [ ] `n_boot=` — bootstrap samples for CI

### Understand

- [ ] Confidence intervals in Seaborn are bootstrapped by default
- [ ] How to show SD instead of CI
- [ ] When to show raw data instead of estimates

**Exercises**
- [ ] Compare group means with 95% CI
- [ ] Switch from CI to SD error bars

---

## Phase 17: Working with Real Data

### Learn

- [ ] Handling missing values before plotting
- [ ] Long format vs wide format (Added — Seaborn expects long)
- [ ] `pd.melt()` to convert wide → long (Added)
- [ ] Ordering categories with `order=` (Added)

**Exercises**
- [ ] Customer analytics EDA
- [ ] Sales analytics EDA

---

## Phase 18: Seaborn + Pandas

### Learn

- [ ] DataFrame integration with `data=`
- [ ] GroupBy → plot pipeline
- [ ] Using Pandas `category` dtype for ordered axes (Added)

**Exercises**
- [ ] Full EDA workflow: load → clean → explore → visualize

---

## Phase 19: Seaborn + Matplotlib

### Learn

- [ ] Customize Seaborn plots with Matplotlib commands
- [ ] `plt.gcf()` / `plt.gca()` to get current figure/axes
- [ ] Adding titles, annotations after Seaborn call

### Understand

- [ ] When to drop to Matplotlib for fine-grained control
- [ ] Seaborn as a starting point, Matplotlib for finishing

**Exercises**
- [ ] Add custom annotations to a Seaborn chart
- [ ] Combine Seaborn and Matplotlib in one figure

---

## Phase 20: Modern Seaborn Objects API (Added)

### Learn

- [ ] `so.Plot()` — new declarative API (Seaborn 0.12+)
- [ ] `so.Dot()`, `so.Line()`, `so.Bar()` marks
- [ ] `so.Agg()`, `so.Stack()` transforms
- [ ] Layering marks on one plot

### Understand

- [ ] Objects API vs legacy API
- [ ] More composable and consistent
- [ ] Still maturing — when to use vs legacy

---

## Phase 21: Performance

### Understand

- [ ] Large dataset visualization challenges
- [ ] Sampling strategies before plotting

### Learn

- [ ] Sample with `df.sample()` before plotting (Added)
- [ ] Use `sns.kdeplot()` instead of scatter for density (Added)
- [ ] Hexbin plot for large scatter data (Added)

**Exercises**
- [ ] Visualize 1M-row dataset effectively

---

## Phase 22: EDA Workflow

### Full EDA Process

1. [ ] Inspect data shape and types (`df.info()`, `df.describe()`)
2. [ ] Check missing values (`df.isnull().sum()`)
3. [ ] Analyze distributions (histplot, kdeplot per feature)
4. [ ] Analyze categorical frequencies (countplot)
5. [ ] Explore relationships (pairplot, scatterplot)
6. [ ] Check correlation (heatmap)
7. [ ] Find outliers (boxplot, violinplot)
8. [ ] Segment by group (`hue=`, faceting)
9. [ ] Build insights and document findings

**Exercises**
- [ ] Full EDA on Titanic dataset
- [ ] Full EDA on a business dataset

---

## Phase 23: Real Projects

### Beginner
- [ ] Student Performance Analysis
- [ ] Expense Analysis

### Intermediate
- [ ] Sales Analytics Dashboard
- [ ] HR Analytics Report

### Advanced
- [ ] Customer Segmentation Analysis
- [ ] Product Analytics Report

### Expert
- [ ] End-to-End EDA Framework
- [ ] Business Intelligence Visualization Suite
- [ ] Automated EDA Report Generator (Added)

---

## Final Mastery

**Can Explain:** Distribution Analysis, Relationship Analysis, Correlation, Confidence Intervals, Figure-level vs Axes-level APIs, Faceting, Seaborn Architecture, Long vs Wide Format, Statistical Estimation

**Can Build:** EDA Reports, Analytics Dashboards, Statistical Visualizations, Business Reports, Insight Presentations, Automated EDA Pipelines