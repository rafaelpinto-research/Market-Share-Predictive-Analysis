# Predicting Product Market Share: Pricing & Promotional Analysis

> **Project Status:** Completed
> **Tools Used:** R, Multiple Linear Regression, Statistical Modeling

## Executive Summary
This project investigates the key drivers of a product's market share using 36 months of transactional data from a national Nielsen database. By building a **Multiple Linear Regression model**, the analysis quantifies the independent effects of pricing strategies, advertising exposure (GNR points), and promotional activities on consumer behavior.

The study reveals that **price discounts** are the most significant driver of market share growth, while traditional advertising showed no statistically significant impact in this specific context.

## Technical Stack
*   **Language:** R
*   **Libraries:** `ggplot2`, `readxl`, `plotly`
*   **Methodology:**
    *   Exploratory Data Analysis (EDA) & Data Visualization.
    *   Multiple Linear Regression Modeling.
    *   Diagnostic Testing (Residuals vs Fitted, Q-Q Plots) to ensure OLS assumptions (Linearity, Homoscedasticity, Normality).

## Key Research Questions
1.  Which business factors (Price, Advertising, Discounts, Promotions) are statistically significant predictors of market share?
2.  What is the magnitude and direction of these effects?
3.  Can we build a robust model to explain market variance? (Result: **Adjusted R² = 0.6688**, explaining ~67% of the variance).

## 📈 Key Business Insights
Based on the regression coefficients ($\beta$), the analysis yielded the following strategic insights:

*   **Discounts are King:** The presence of a price discount was the strongest positive predictor ($\beta = 0.40$, $p < 0.001$). Holding other factors constant, a discount increases market share by 0.40 points.
*   **Promotions Work, but Less than Discounts:** Package promotions had a positive, significant effect ($\beta = 0.12$, $p = 0.039$), but the impact is less than one-third of that of a direct price discount.
*   **Price Sensitivity:** Higher base prices showed a marginally significant negative trend on market share, consistent with economic theory.
*   **The Advertising Paradox:** Surprisingly, advertising exposure (GNR Points) did **not** show a statistically significant relationship with market share ($p = 0.908$). This suggests that for this product, point-of-sale incentives (discounts) are far more effective than general media exposure.

## 📂 Repository Structure
*   `analysis_script.R`: The R script containing data cleaning, visualization, and regression modeling code.
*   `Project_Report.pdf`: The full academic report including literature review, detailed statistical interpretation, and limitations.
