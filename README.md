# Soda Container Taste Analysis

## Overview

Does the type of container you drink soda from affect how it tastes?

This project investigates whether soda served in a **glass bottle, aluminum can, or plastic cup** produces differences in perceived taste and crispness. The experiment was conducted using a **Randomized Complete Block Design (RCBD)**, and the resulting data were analyzed in R.

Four experimenters each randomly selected three participants, with every participant receiving all three container treatments in a randomized order.

## Research Question

**After accounting for block effects, is there evidence that mean taste/crispness ratings differ among glass bottles, cans, and plastic cups?**

## Methods

The dataset contains **36 observations** across:

- 4 experimental blocks
- 3 container treatments
- 3 replicates per block-treatment combination

The analysis includes:

- Exploratory data analysis and visualization
- Descriptive statistics
- Randomized Complete Block Design (RCBD)
- Analysis of Variance (ANOVA)
- Model and residual diagnostics
- Bartlett's test for equal variances
- Bonferroni-adjusted pairwise comparisons

## Key Findings

The RCBD ANOVA found **no statistically significant effect of container type** on perceived soda taste/crispness:

**F(2, 30) = 0.99, p = 0.385**

Although cans produced the highest observed mean rating, the differences among container types were not large enough relative to the variability in the sample to provide statistically significant evidence of a container effect.

## Technologies

- R
- Quarto
- RStudio
- knitr
- Statistical modeling and hypothesis testing
- Data visualization

## Repository Contents

```text
soda-container-taste-analysis/
├── raw_soda_data.csv
├── soda-container-taste-analysis.qmd
├── soda-container-taste-analysis.html
└── README.md
```

- **`raw_soda_data.csv`** — Raw experimental data used in the analysis
- **`soda-container-taste-analysis.qmd`** — Quarto source containing the R analysis and report
- **`soda-container-taste-analysis.html`** — Rendered interactive report
- **`README.md`** — Project overview and documentation

## Reproducing the Analysis

Clone or download the repository and open `soda-container-taste-analysis.qmd` in RStudio.

The analysis imports the raw dataset using:

```r
soda_data <- read.csv("raw_soda_data.csv")
```

Because the dataset uses a relative file path, the analysis can be reproduced without changing file paths as long as the CSV and QMD remain in the same directory.

Render the Quarto document to generate the complete HTML report.

## Skills Demonstrated

This project demonstrates experience with **experimental design, statistical inference, R programming, data visualization, model diagnostics, reproducible analysis, and communicating statistical results**.
