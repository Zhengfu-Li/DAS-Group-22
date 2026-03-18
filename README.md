### Formal Analysis and GLM Modeling

This repository contains the formal data analysis and Generalized Linear Model (GLM) implementation for [Project Name/Group 22]. The primary focus of this analysis is variable selection using the Akaike Information Criterion (AIC) and model performance evaluation.

#### Overview

The goal of this project is to build a robust statistical model to predict [yesno].

#### Key Analysis Steps

- **Variable Selection via AIC**
We utilized the Akaike Information Criterion (AIC) to determine the optimal set of predictors.
    - **Finding:** The analysis revealed that the variable `make` did not contribute significantly to the model's explanatory power.
    - **Action:** Consequently, `make` was excluded from the final model specification to prevent overfitting and improve model parsimony.
- **GLM Training Strategies**
To ensure the robustness of our findings, we conducted GLM training using two distinct approaches:
    - **Full Dataset Training:** A model trained on the entire dataset to capture the maximum amount of variance and establish baseline coefficients.
    - **Train-Test Split (80/20):** The data was partitioned into an 80% training set and a 20% testing set. This approach allows for the validation of model performance on unseen data, providing a more realistic estimate of predictive accuracy.



