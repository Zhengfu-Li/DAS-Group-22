# Group 22 Spam Email Analysis

This repository contains the Quarto report, dataset, and supporting project files for Group 22's coursework on spam email classification. The analysis focuses on exploratory data analysis of text-derived predictors and is intended to support later modelling work.

## Project overview

The dataset records whether an email is classified as spam (`y`) or non-spam (`n`) together with six explanatory variables:

- `crl.tot`
- `dollar`
- `bang`
- `money`
- `n000`
- `make`

The exploratory analysis in the report examines:

- class balance in the response variable
- grouped descriptive summaries of the predictors
- distributional differences between spam and non-spam emails
- pairwise relationships among the predictors
- the effect of duplicated rows on the main exploratory conclusions

## Main files

- `Group_22_Analysis.qmd` : main Quarto source document
- `Group_22_Analysis.html` : rendered report output
- `dataset22.csv` : dataset used in the analysis
- `DAS-Group-22.Rproj` : RStudio project file

## Reproducibility

The report is designed to be rendered from the project root so that file paths are handled consistently through the `here` package.

Required R packages:

- `tidyverse`
- `skimr`
- `janitor`
- `here`
- `GGally`

If needed, install them in R with:

```r
install.packages(c("tidyverse", "skimr", "janitor", "here", "GGally"))
```

To reproduce the report:

1. Open `DAS-Group-22.Rproj` in RStudio.
2. Open `Group_22_Analysis.qmd`.
3. Render the document to produce the HTML output.

## Notes on the analysis

- The EDA keeps duplicated rows in the main descriptive analysis so that the report reflects the supplied dataset.
- A duplicate-sensitivity check is included in the report to assess whether the main exploratory patterns change after deduplication.
- The Quarto document is the primary source for the written analysis and figure generation.
