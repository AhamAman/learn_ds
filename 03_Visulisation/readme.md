# Data Visualization Mastery Checklists

> A complete, phase-by-phase learning roadmap covering data visualization with Matplotlib, Seaborn, Power BI, and Tableau — from fundamentals to publication-quality graphics and enterprise-level dashboards.

---

## Table of Contents

1. [Matplotlib](#1-matplotlib)
2. [Seaborn](#2-seaborn)
3. [Power BI](#3-power-bi)
4. [Tableau](#4-tableau)

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

---

# 3. Power BI

*From Beginner → Analyst → Enterprise-Level Reporting*

---

## Phase 0: Prerequisites

### Data Fundamentals

- [ ] Tables, rows, columns
- [ ] Relationships between tables
- [ ] Data types (text, number, date, boolean)

### Excel Basics

- [ ] Formulas and functions
- [ ] Pivot Tables
- [ ] Basic charts

### Statistics Basics

- [ ] Mean, median, sum, count
- [ ] Percentages and ratios
- [ ] Trend interpretation

---

## Phase 1: Why Power BI Exists

### The Problem

- [ ] Excel struggles with large datasets
- [ ] Manual reporting takes too long
- [ ] Insights are buried in spreadsheets
- [ ] Reports can't update automatically

### First Principles

- [ ] What is Business Intelligence (BI)?
- [ ] What is a dashboard?
- [ ] Self-service analytics concept

### Understand

- [ ] Power BI Desktop vs Power BI Service vs Power BI Mobile
- [ ] Report vs Dashboard vs Dataset distinction
- [ ] When Power BI beats Excel
- [ ] When to use Power BI vs Tableau vs Python

---

## Phase 2: Power BI Ecosystem

### Products

- [ ] Power BI Desktop (free, build reports)
- [ ] Power BI Service (cloud, share reports)
- [ ] Power BI Mobile (view on phone)
- [ ] Power BI Report Server (on-premise)

### Related Tools

- [ ] Power Query (data transformation)
- [ ] Power Pivot (data modeling)
- [ ] DAX (Data Analysis Expressions)

### Understand

- [ ] Full workflow: Desktop → Publish → Service → Share

---

## Phase 3: Connecting to Data

### File Sources

- [ ] Excel / CSV / JSON / XML
- [ ] PDF (Added)
- [ ] Folder (load all files at once)

### Database Sources

- [ ] SQL Server
- [ ] MySQL / PostgreSQL
- [ ] Azure SQL Database

### Cloud Sources

- [ ] SharePoint
- [ ] Google Analytics
- [ ] Salesforce
- [ ] Web (scrape from URL)

### Understand

- [ ] Import mode vs DirectQuery vs Live Connection
- [ ] When each connection mode is appropriate
- [ ] Refresh frequency and data currency

---

## Phase 4: Power Query (Data Transformation)

### Core Concepts

- [ ] What is Power Query?
- [ ] M language (behind the scenes)
- [ ] Applied Steps — every action recorded

### Common Transformations

- [ ] Remove columns / rows
- [ ] Rename columns
- [ ] Change data types
- [ ] Filter rows
- [ ] Replace values
- [ ] Handle missing values (null)
- [ ] Split columns (by delimiter, position)
- [ ] Merge / Append queries

### Advanced Transformations

- [ ] Pivot / Unpivot columns
- [ ] Group By (aggregate)
- [ ] Custom columns with M formula
- [ ] Conditional columns
- [ ] Index columns

### Understand

- [ ] Why transform in Power Query vs DAX
- [ ] Wide vs long format for visuals
- [ ] Query folding concept

**Exercises**
- [ ] Clean a messy CSV in Power Query
- [ ] Merge two tables on a common key

---

## Phase 5: Data Modeling

### Core Concepts

- [ ] Fact Table (measures, transactions)
- [ ] Dimension Table (descriptions, categories)
- [ ] Star Schema
- [ ] Snowflake Schema

### Relationships

- [ ] One-to-Many (most common)
- [ ] Many-to-Many
- [ ] One-to-One
- [ ] Active vs Inactive relationships
- [ ] Cross-filter direction (single vs both)

### Understand

- [ ] Why data modeling matters for accurate reports
- [ ] Cardinality concept
- [ ] Avoid many-to-many where possible
- [ ] Role-playing dimensions (e.g. date used as order date and ship date)

**Exercises**
- [ ] Build a star schema from flat files
- [ ] Set up relationships between tables

---

## Phase 6: DAX Fundamentals

### What is DAX?

- [ ] Data Analysis Expressions
- [ ] Formula language for calculated columns and measures

### Types of Calculations

- [ ] Calculated Column (row-by-row, stored)
- [ ] Measure (dynamic, evaluated at query time)

### Basic DAX Functions

**Aggregation**
- [ ] SUM() / AVERAGE() / COUNT() / COUNTROWS() / MIN() / MAX()

**Logical**
- [ ] IF() / AND() / OR() / SWITCH()

**Text**
- [ ] CONCATENATE() / LEFT() / RIGHT() / LEN() / FORMAT()

**Date**
- [ ] YEAR() / MONTH() / DAY() / TODAY() / DATEDIFF()

**Filter**
- [ ] CALCULATE() / FILTER() / ALL() / ALLEXCEPT()

### Understand

- [ ] Measures vs calculated columns — when to use each
- [ ] How CALCULATE() changes filter context
- [ ] Row context vs filter context (critical concept)

**Exercises**
- [ ] Total Sales measure
- [ ] Profit Margin % measure
- [ ] YTD Sales measure

---

## Phase 7: Advanced DAX

### Time Intelligence

- [ ] TOTALYTD() / TOTALQTD() / TOTALMTD()
- [ ] DATEADD() / SAMEPERIODLASTYEAR()
- [ ] PARALLELPERIOD()
- [ ] Running totals

### Filter Context Manipulation

- [ ] CALCULATE() with multiple filters
- [ ] ALL() — remove all filters
- [ ] ALLEXCEPT() — remove all filters except specified
- [ ] KEEPFILTERS()
- [ ] REMOVEFILTERS()

### Iterator Functions

- [ ] SUMX() / AVERAGEX() / COUNTX()
- [ ] RANKX()
- [ ] MAXX() / MINX()

### Relationship Functions

- [ ] RELATED() — lookup value from related table
- [ ] RELATEDTABLE()
- [ ] USERELATIONSHIP() — activate inactive relationship

### Understand

- [ ] CALCULATE() is the most important DAX function
- [ ] When iterators are necessary
- [ ] Context transition concept

**Exercises**
- [ ] Sales vs prior year comparison
- [ ] Running total measure
- [ ] Dynamic ranking measure

---

## Phase 8: Visualizations

### Basic Visuals

- [ ] Bar / Column Chart
- [ ] Line Chart
- [ ] Pie / Donut Chart
- [ ] Card (single KPI number)
- [ ] Table / Matrix
- [ ] Scatter Chart

### Intermediate Visuals

- [ ] Clustered vs Stacked Bar
- [ ] Combo Chart (line + bar)
- [ ] Treemap
- [ ] Funnel Chart
- [ ] Gauge Chart
- [ ] Map (filled, bubble)

### Advanced Visuals

- [ ] Waterfall Chart
- [ ] Ribbon Chart
- [ ] Decomposition Tree
- [ ] Key Influencers
- [ ] Smart Narrative
- [ ] Custom Visuals from AppSource

### Understand

- [ ] Choosing the right visual for the question
- [ ] When NOT to use pie charts
- [ ] KPI visual vs Card visual

---

## Phase 9: Filters & Slicers

### Filter Types

- [ ] Visual-level filter
- [ ] Page-level filter
- [ ] Report-level filter
- [ ] Drillthrough filter

### Slicers

- [ ] Dropdown / List / Between / Relative Date
- [ ] Sync slicers across pages
- [ ] Slicer panel (toggle visibility)

### Understand

- [ ] Filter pane vs slicer (same result, different UX)
- [ ] How filters interact with DAX measures
- [ ] Edit interactions between visuals

**Exercises**
- [ ] Build a report with synced date slicer

---

## Phase 10: Report Design

### Layout Principles

- [ ] Grid alignment
- [ ] Consistent fonts and colors
- [ ] Visual hierarchy (most important = largest)
- [ ] White space usage

### Branding

- [ ] Custom themes (JSON file)
- [ ] Company colors and fonts
- [ ] Logo placement

### Navigation

- [ ] Bookmarks (save view states)
- [ ] Buttons for navigation
- [ ] Tooltip pages (hover details)
- [ ] Drillthrough pages

### Best Practices

- [ ] No more than 5–7 visuals per page
- [ ] Clear page titles and labels
- [ ] Consistent date filters across pages
- [ ] Mobile layout view

**Exercises**
- [ ] Build a multi-page sales report

---

## Phase 11: Row-Level Security (RLS)

### Learn

- [ ] What is RLS?
- [ ] Static RLS — fixed rules per role
- [ ] Dynamic RLS — uses USERNAME() or USERPRINCIPALNAME()

### Understand

- [ ] How to define roles in Desktop
- [ ] How to assign users to roles in Service
- [ ] Testing RLS before publishing

**Exercises**
- [ ] Region-based RLS for sales report

---

## Phase 12: Power BI Service

### Learn

- [ ] Publishing from Desktop to Service
- [ ] Workspaces (My Workspace vs shared)
- [ ] Dashboards (pin visuals from reports)
- [ ] Scheduled Refresh setup
- [ ] Data Gateway (for on-premise sources)

### Sharing & Collaboration

- [ ] Share report link
- [ ] Publish to web (public)
- [ ] Power BI Apps (package reports for distribution)
- [ ] Workspace roles (Admin, Member, Contributor, Viewer)

---

## Phase 13: Performance Optimization

### Data Model

- [ ] Remove unused columns
- [ ] Use integer keys instead of text keys
- [ ] Avoid bidirectional relationships where possible
- [ ] Use summarized tables for large datasets

### DAX

- [ ] Prefer measures over calculated columns
- [ ] Avoid iterating over large tables unnecessarily
- [ ] Use variables (`VAR`) to avoid recalculation

### Report

- [ ] Reduce number of visuals per page
- [ ] Use import mode over DirectQuery for speed
- [ ] Aggregation tables for large datasets

**Exercises**
- [ ] Performance Analyzer tool usage

---

## Phase 14: Advanced Features

### What-If Parameters

- [ ] Dynamic scenario analysis
- [ ] Slider-based sensitivity analysis

### Calculation Groups

- [ ] Reusable time intelligence logic
- [ ] Avoid DAX duplication

### Field Parameters

- [ ] User-switchable axes/measures in visuals

### Deployment Pipelines

- [ ] Development → Test → Production workflow

### Paginated Reports

- [ ] Pixel-perfect printing
- [ ] SSRS-style reports in Power BI

---

## Phase 15: Real Projects

### Beginner
- [ ] Personal Expense Dashboard
- [ ] Student Results Report

### Intermediate
- [ ] Sales Performance Dashboard
- [ ] HR Analytics Report

### Advanced
- [ ] Financial P&L Report
- [ ] Supply Chain Analytics Dashboard

### Expert
- [ ] Enterprise Multi-Department BI Solution
- [ ] Real-Time Streaming Dashboard
- [ ] Embedded Power BI in Web App

---

## Final Mastery

**Can Explain:** Power Query, Data Modeling, Star Schema, DAX measures vs calculated columns, Filter context vs row context, CALCULATE(), Time Intelligence, RLS, DirectQuery vs Import, Report vs Dashboard

**Can Build:** End-to-end BI reports, Star schema data models, Complex DAX measures, Multi-page dashboards, Row-level security, Scheduled refresh pipelines

---

# 4. Tableau

*From Beginner → Analyst → Advanced Visual Analytics*

---

## Phase 0: Prerequisites

### Data Fundamentals

- [ ] Tables, rows, columns
- [ ] Data types (string, number, date, boolean)
- [ ] Aggregations (sum, avg, count)

### Statistics Basics

- [ ] Mean, median, percentages
- [ ] Distributions and trends

### Visualization Basics

- [ ] Chart types and when to use them
- [ ] What makes a good dashboard

---

## Phase 1: Why Tableau Exists

### The Problem

- [ ] Business users need fast visual insights without coding
- [ ] Excel charts are static and limited
- [ ] Traditional BI tools require SQL/IT involvement

### First Principles

- [ ] Visual analytics concept
- [ ] Drag-and-drop data exploration
- [ ] Show Me — intelligent chart suggestions

### Understand

- [ ] Tableau Desktop vs Tableau Public vs Tableau Server vs Tableau Cloud
- [ ] Tableau vs Power BI — key differences
- [ ] When Tableau's visualization flexibility wins
- [ ] Tableau licensing model

---

## Phase 2: Tableau Ecosystem

### Products

- [ ] Tableau Desktop (full authoring, paid)
- [ ] Tableau Public (free, public publishing)
- [ ] Tableau Prep (data preparation)
- [ ] Tableau Server (on-premise sharing)
- [ ] Tableau Cloud (cloud sharing)

### Understand

- [ ] Tableau Public is free and great for learning
- [ ] Tableau Prep = ETL tool equivalent to Power Query

---

## Phase 3: Connecting to Data

### File Sources

- [ ] Excel / CSV / JSON / PDF / Spatial files

### Database Sources

- [ ] SQL Server / MySQL / PostgreSQL
- [ ] BigQuery / Redshift / Snowflake

### Cloud Sources

- [ ] Google Sheets
- [ ] Salesforce
- [ ] Web Data Connector

### Understand

- [ ] Live connection vs Extract
- [ ] Extracts (.hyper files) for performance
- [ ] When to use live vs extract

---

## Phase 4: Tableau Interface

### Key Areas

- [ ] Data pane (dimensions and measures)
- [ ] Shelves (Rows, Columns, Color, Size, Label, Detail, Tooltip)
- [ ] Canvas / View
- [ ] Show Me panel
- [ ] Marks card

### Understand

- [ ] Dimensions (categorical, blue pills)
- [ ] Measures (numerical, green pills)
- [ ] Discrete vs Continuous fields
- [ ] Blue pill vs green pill behavior difference

**Exercises**
- [ ] Build first bar chart by drag and drop

---

## Phase 5: Building Basic Charts

### Learn

- [ ] Bar Chart
- [ ] Line Chart
- [ ] Scatter Plot
- [ ] Pie / Donut Chart
- [ ] Map (filled, symbol)
- [ ] Treemap
- [ ] Bubble Chart
- [ ] Histogram (bin creation)
- [ ] Box and Whisker Plot

### Show Me Panel

- [ ] When to use Show Me
- [ ] Understanding Show Me's chart suggestions

**Exercises**
- [ ] Sales by region bar chart
- [ ] Monthly revenue trend line chart
- [ ] Profit vs Sales scatter plot

---

## Phase 6: Sorting & Filtering

### Sorting

- [ ] Manual sort
- [ ] Sort by field (ascending/descending)
- [ ] Nested sort

### Filters

- [ ] Dimension filter
- [ ] Measure filter
- [ ] Date filter (relative, range, discrete)
- [ ] Context filter
- [ ] Top N filter
- [ ] Condition filter

### Filter Order of Operations

- [ ] Extract → Data Source → Context → Dimension → Measure → Table Calc

### Understand

- [ ] Why context filters exist
- [ ] Filter order affects results

**Exercises**
- [ ] Top 10 products by sales
- [ ] Sales for last 12 months

---

## Phase 7: Calculated Fields

### Types

- [ ] Basic calculated field
- [ ] Aggregate calculation
- [ ] Table calculation
- [ ] Level of Detail (LOD) expression

### Basic Calculations

- [ ] Arithmetic: `[Sales] - [Cost]`
- [ ] String: `LEFT([Name], 3)`
- [ ] Date: `DATEDIFF('month', [Order Date], TODAY())`
- [ ] Logical: `IF [Sales] > 1000 THEN "High" ELSE "Low" END`
- [ ] NULL handling: `ISNULL()`, `ZN()`, `IFNULL()`

### Understand

- [ ] When to calculate vs transform in Prep/source

**Exercises**
- [ ] Profit Margin % calculated field
- [ ] Customer age from birthdate

---

## Phase 8: Table Calculations

### Learn

- [ ] Running Total
- [ ] Percent of Total
- [ ] Rank
- [ ] Moving Average
- [ ] Difference / Percent Difference from previous

### Understand

- [ ] Table calculations run after aggregation
- [ ] Compute using: Table (across/down), Pane, Cell, Specific dimension
- [ ] Direction matters: across vs down

**Exercises**
- [ ] Running total sales by month
- [ ] Percent of total by category

---

## Phase 9: Level of Detail (LOD) Expressions

### Types

- [ ] FIXED — compute at specified level, ignore view filters
- [ ] INCLUDE — add granularity beyond view
- [ ] EXCLUDE — remove granularity from view

### Understand

- [ ] LOD vs Table Calculation vs Aggregate
- [ ] When each is appropriate
- [ ] LOD interacts with context filters, not dimension filters

**Exercises**
- [ ] Customer-level average vs order-level average
- [ ] Sales per customer using FIXED LOD

---

## Phase 10: Parameters

### Learn

- [ ] Create parameters (integer, float, string, date, list)
- [ ] Reference parameter in calculated field
- [ ] Show parameter control in view

### Use Cases

- [ ] Dynamic top N filter
- [ ] What-if analysis
- [ ] User-selectable metric (Sales vs Profit toggle)
- [ ] Dynamic reference lines

**Exercises**
- [ ] Top N parameter-driven bar chart
- [ ] Switch between metrics dynamically

---

## Phase 11: Maps & Geospatial

### Learn

- [ ] Symbol Map (point locations)
- [ ] Filled Map (shaded regions)
- [ ] Density Map
- [ ] Custom territory creation
- [ ] Dual-axis map

### Understand

- [ ] How Tableau geocodes data
- [ ] Editing unrecognized locations
- [ ] Custom geocoding with lat/long

**Exercises**
- [ ] Sales by country filled map
- [ ] Store locations symbol map

---

## Phase 12: Dashboard Design

### Layout

- [ ] Tiled vs floating objects
- [ ] Containers (horizontal/vertical)
- [ ] Consistent sizing and padding
- [ ] Device designer (desktop/tablet/phone)

### Interactivity

- [ ] Dashboard actions (filter, highlight, URL, go to sheet)
- [ ] Filter actions (click one chart to filter others)
- [ ] Highlight actions
- [ ] Sheet swapping with parameter + calculated field

### Navigation

- [ ] Button actions for navigation
- [ ] Tooltip design
- [ ] Custom shapes and images

### Design Principles

- [ ] One clear message per dashboard
- [ ] Progressive disclosure
- [ ] Consistent color encoding
- [ ] Minimal but sufficient labels

**Exercises**
- [ ] 3-chart interactive sales dashboard
- [ ] Add filter action between charts

---

## Phase 13: Stories

### Learn

- [ ] Story points concept
- [ ] Adding sheets as story points
- [ ] Annotations and narration
- [ ] Presenting with Tableau Stories

### Understand

- [ ] Story vs Dashboard vs Sheet
- [ ] When to use stories (presentations, guided analysis)

---

## Phase 14: Analytics Pane

### Learn

- [ ] Reference Lines (constant, average, median)
- [ ] Reference Bands
- [ ] Trend Lines (linear, polynomial, exponential, logarithmic)
- [ ] Forecasting (built-in exponential smoothing)
- [ ] Cluster analysis (k-means built-in)
- [ ] Box Plot statistics

### Understand

- [ ] Tableau forecasting limitations
- [ ] When to trust built-in analytics vs export to Python/R

---

## Phase 15: Tableau Prep

### Learn

- [ ] Connect to data sources
- [ ] Profile pane (data quality view)
- [ ] Clean steps (rename, filter, split, replace)
- [ ] Pivot (wide to long)
- [ ] Aggregate step
- [ ] Join / Union
- [ ] Output to extract or database

### Understand

- [ ] Tableau Prep vs Power Query
- [ ] When to use Prep vs clean in Desktop

---

## Phase 16: Performance Optimization

### Data

- [ ] Use extracts over live connections
- [ ] Aggregate to appropriate granularity
- [ ] Filter early in Prep/data source

### Workbook

- [ ] Reduce marks in view
- [ ] Avoid unnecessary detail marks
- [ ] Use context filters correctly
- [ ] Limit LOD expressions

### Tools

- [ ] Performance Recording (built-in profiler)
- [ ] VizQL query inspection

---

## Phase 17: Tableau Server / Cloud

### Learn

- [ ] Publishing workbooks
- [ ] Permissions and content levels
- [ ] Data source publishing (centralized)
- [ ] Scheduled extract refreshes
- [ ] Subscriptions (email reports)
- [ ] Embedding Tableau in web apps

### Understand

- [ ] Site → Project → Workbook → View hierarchy
- [ ] Row-level security options in Tableau

---

## Phase 18: Advanced Topics

### Extensions

- [ ] Dashboard Extensions API
- [ ] Integration with Python/R (TabPy, RServe)

### Tableau with Python (TabPy)

- [ ] Call Python functions from calculated fields
- [ ] Use ML model predictions in Tableau

### Tableau Bridge

- [ ] Live connection to on-premise data from Tableau Cloud

### Embedding

- [ ] Tableau JavaScript API
- [ ] Embedded analytics in web apps

---

## Phase 19: Real Projects

### Beginner
- [ ] Superstore Sales Dashboard (built-in dataset)
- [ ] Personal Finance Tracker

### Intermediate
- [ ] Sales Performance Dashboard
- [ ] Customer Cohort Analysis

### Advanced
- [ ] Executive KPI Dashboard
- [ ] Supply Chain Analytics

### Expert
- [ ] Real-Time Operational Dashboard
- [ ] Embedded Analytics in Web Application
- [ ] Tableau Public Portfolio (5+ published dashboards)

---

## Final Mastery

**Can Explain:** Dimensions vs Measures, Discrete vs Continuous, Live vs Extract, Tableau calculation types (basic, table calc, LOD), Parameters, Dashboard actions, Filter order of operations, FIXED vs INCLUDE vs EXCLUDE LOD

**Can Build:** Multi-chart interactive dashboards, LOD-powered analytics, Parameter-driven views, Geographic analyses, Storytelling presentations, Published Tableau Public portfolio