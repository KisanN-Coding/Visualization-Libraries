# Overview of Notebook 1 — Seaborn

**Goal:** Get comfortable with Seaborn’s core plotting APIs, the difference between figure-level and axes-level functions, and how to facet and size your visuals.

## Topics Covered
- **Setup & Imports**
  - `seaborn as sns`, `matplotlib.pyplot as plt`, `pandas as pd`, `numpy as np`
- **Figure-level vs Axes-level**
  - Figure-level: `sns.relplot`, `sns.displot` (create their own figure; easy faceting & sizing)
  - Axes-level: `sns.scatterplot`, `sns.lineplot`, `sns.histplot`, `sns.kdeplot`, `sns.rugplot`
- **Relational Plots**
  - `scatterplot` (bivariate relationships)
  - `lineplot` (trend/series)
  - `relplot` with **faceting** via `row=`, `col=`, `hue=`
- **Distribution Plots**
  - Univariate: `displot(kind="hist")`, `histplot`, `kdeplot`, `rugplot`
  - Bivariate: `displot(kind="hist", x=..., y=...)` (2D histogram), `displot(kind="kde", x=..., y=...)` (2D KDE)
- **Faceting & Layout Controls**
  - `row=`, `col=`, `col_wrap=`
  - Size controls for figure-level functions: `height=`, `aspect=`
- **Matrix Plots**
  - `heatmap` (e.g., correlation/pivot-style grids)
  - `clustermap` (clustered heatmap)
- **Grids & Multi-plot Concepts**
  - Concepts introduced: `FacetGrid`, `PairGrid`, `JointGrid` (what they are and when to reach for them)

## Common Parameters Used
- Mapping: `x=`, `y=`, `data=`
- Grouping/Faceting: `hue=`, `row=`, `col=`, `col_wrap=`
- Aggregation/Layout: `estimator=`, `height=`, `aspect=`, `kind=`, `order=`

## Datasets Used
- `tips`, `titanic`

## What You’ll Walk Away With
- Know when to choose **figure-level** vs **axes-level** functions
- Create **faceted views** to compare subsets quickly
- Use **distribution** and **matrix** plots to summarize structure and relationships
- Control plot **size**, **aspect**, and **layout** like a pro


---

# Overview of Notebook 2 — Seaborn Part 2

**Goal:** Dive deeper into categorical, regression, and multi-plot grids, with heavy use of `catplot` and grid objects.

## Topics Covered
- **Categorical Plots (axes-level + figure-level)**
  - Scatter-style: `stripplot`, `swarmplot`
  - Distribution/summary: `boxplot`, `violinplot`
  - Aggregated summaries: `barplot` (e.g., mean by category), `pointplot` (mean + CI), `countplot`
  - Figure-level wrapper: **`catplot`** (used extensively) with `kind=` to switch among the above and `row=`, `col=`, `hue=` for faceting
- **Faceting with `catplot`**
  - Build small multiples via `row=`, `col=`, optionally `col_wrap=`
  - Control size with `height=`, `aspect=`
  - Sort/arrange categories via `order=`
  - Aggregate via `estimator=` and show uncertainty with `ci=`
- **Regression Plots**
  - `regplot` (axes-level), `lmplot` (figure-level), `residplot` (residual diagnostics)
- **Multi-plot Grids**
  - `pairplot` / **`PairGrid`** (pairwise relationships across variables)
  - `jointplot` / **`JointGrid`** (bivariate distribution + marginal plots)
  - `FacetGrid` (an alternative/”second way” to build faceted figures)
- **In-built Seaborn Datasets**
  - Browsing/using built-ins (e.g., `get_dataset_names`, `load_dataset`)

## Common Parameters Used
- Mapping: `x=`, `y=`, `data=`
- Grouping/Faceting: `hue=`, `row=`, `col=`, `col_wrap=`
- Aggregation/Layout: `kind=`, `estimator=`, `order=`, `height=`, `aspect=`

## Datasets Used
- `tips`, `iris`, `planets`

## What You’ll Walk Away With
- Choose the **right categorical plot** (strip/swarm/box/violin/bar/point/count)
- Master **`catplot`** to facet and compare categories at scale
- Run quick **regression diagnostics** and trend visualizations
- Build **pairwise** and **bivariate** multi-plot layouts with grid objects

