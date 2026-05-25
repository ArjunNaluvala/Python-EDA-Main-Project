# IPL Ball-by-Ball Data Analysis

# Overview

This project performs **end-to-end Exploratory Data Analysis (EDA)** on IPL ball-by-ball cricket data covering **18 IPL seasons (2007–2025)**.

The project focuses on analyzing:

* Match trends
* Batting performance
* Bowling statistics
* Toss decisions
* Venue-wise scoring patterns
* Seasonal run trends
* Over-phase scoring behavior

Using Python-based analytics techniques, the project converts raw cricket data into meaningful sports insights through advanced visualization and statistical analysis.

# Business Problem

Cricket generates massive amounts of ball-by-ball data every season, making it difficult to manually identify:

* Player performance trends
* Match-winning patterns
* Scoring behavior across overs
* Venue performance
* Team strategies
* Toss impact on results

This project solves the problem by using data analytics to extract actionable sports insights from IPL match data.

# Objectives

* Perform large-scale sports data analysis
* Clean and preprocess IPL ball-by-ball data
* Analyze batting and bowling performance
* Study toss and match-winning relationships
* Identify scoring patterns across overs
* Generate data-driven cricket insights

# Dataset Information

| Attribute       | Details                  |
| --------------- | ------------------------ |
| Dataset         | IPL Ball-by-Ball Dataset |
| Total Rows      | 278,205                  |
| Columns         | 64                       |
| Seasons Covered | 18                       |
| Domain          | Sports Analytics         |

# Technologies Used

## Python Libraries

```python id="f7q9nd"
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
```

# Data Cleaning

## Cleaning Techniques Used

* Handled missing values using fillna()
* Validated outliers using boxplots
* Standardized categorical features
* Checked data consistency
* Performed feature engineering
* Verified match-level data quality

# Feature Engineering

## Engineered Features

* Over Phase Classification
* Powerplay Overs
* Middle Overs
* Death Overs
* Strike Rate Calculation
* Seasonal Performance Metrics

# Exploratory Data Analysis (EDA)

## Univariate Analysis

* Run distribution
* Match result distribution
* Toss decision patterns

## Bivariate Analysis

* Toss winner vs match winner
* Team comparison analysis
* Venue scoring analysis

## Multivariate Analysis

* Correlation analysis
* Seasonal trend analysis
* Player performance comparison
* Venue impact analysis

# Analysis Performed

## Batting Analysis

* Top batsmen by runs
* Strike rate analysis
* Season-wise top scorers
* Power hitters analysis

## Bowling Analysis

* Top wicket takers
* Wicket distribution analysis
* Bowling performance trends

## Match Analysis

* Toss impact analysis
* Venue scoring trends
* Match-winning patterns

## Over Phase Analysis

* Powerplay scoring
* Middle overs performance
* Death overs acceleration

# Advanced Techniques Used

* groupby()
* pivot_table()
* crosstab()
* idxmax()
* Correlation Heatmaps
* Statistical Analysis
* Aggregation Analysis

# Visualizations Used

* Histograms
* Bar Charts
* Line Charts
* Countplots
* Heatmaps
* Boxplots
* Crosstab Gradients
* Correlation Matrix

# Sample Code Snippets

## Top Run Scorers

```python id="cx4s9v"
df.groupby("batter")["batsman_runs"].sum().sort_values(ascending=False)
```

## Strike Rate Calculation

```python id="g7d2qm"
strike_rate = (runs / balls_faced) * 100
```

## Correlation Heatmap

```python id="2kz8fp"
sns.heatmap(df.corr(), annot=True)
```

# Key Insights

## Match Insights

* Toss win does not guarantee match victory
* Certain venues consistently produced high-scoring matches
* Death overs generated the highest scoring rates

## Batting Insights

* Top-order batsmen contributed the majority of runs
* Strike rates increased significantly during death overs
* Some players consistently dominated across multiple seasons

## Venue Insights

* Batting-friendly venues showed consistently high totals
* Pitch conditions significantly impacted scoring behavior

## Team Strategy Insights

* Aggressive powerplay batting improved winning probability
* Teams accelerated scoring heavily in final overs

# Business Impact

This project demonstrates how sports analytics can help:

* Teams improve match strategies
* Analysts evaluate player performance
* Coaches identify tactical patterns
* Broadcasters enhance match insights
* Fans understand statistical trends

# Project Workflow

```text id="t9p5xd"
Data Collection
      ↓
Data Cleaning
      ↓
Feature Engineering
      ↓
Exploratory Data Analysis
      ↓
Visualization
      ↓
Insight Generation
      ↓
Sports Analytics Reporting
```

# Skills Demonstrated

* Python Programming
* Exploratory Data Analysis
* Sports Analytics
* Data Cleaning
* Feature Engineering
* Statistical Analysis
* Data Visualization
* Analytical Thinking

# Tools & Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook

---
