# Group 22 Spam Email Analysis

This repository contains the Quarto report, dataset, and supporting files for Group 22's coursework on spam email classification. The project investigates whether a small set of text-derived variables can distinguish spam emails from non-spam emails through exploratory data analysis and logistic regression modelling.

## Project Overview

The dataset records whether an email is classified as spam or non-spam together with six explanatory variables:

- `crl.tot`
- `dollar`
- `bang`
- `money`
- `n000`
- `make`

The aim of the project is to explore how these predictors differ between spam and non-spam emails and to assess their usefulness in a formal modelling framework.

## Analysis Included

The report currently includes:

- class balance checks for the response variable
- grouped descriptive summaries of the predictors
- distributional comparisons between spam and non-spam emails
- pairwise relationships among the explanatory variables
- a duplicate-sensitivity check
- logistic regression modelling and model comparison
- basic evaluation of predictive performance

## Main Files

- `Group_22_Analysis.qmd` : main Quarto source document
- `Group_22_Analysis.html` : rendered HTML report
- `dataset22.csv` : dataset used in the analysis

## Reproducibility

Required R packages include:

- `tidyverse`
- `skimr`
- `janitor`
- `here`
- `GGally`

To reproduce the report:

1. Open `DAS-Group-22.Rproj` in RStudio.
2. Open `Group_22_Analysis.qmd`.
3. Render the document to generate the HTML output.

## Current Progress

- Core EDA and GLM sections are now in place.
- Recent work has focused on checking for unclear wording, possible omissions, and overall consistency in the written report.
- The conclusion section has been further refined to better summarise the main findings from both the exploratory analysis and the modelling results.
