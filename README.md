# Linear Regression Analysis: Age and BMI

## Overview
This project investigates the relationship between age and Body Mass Index (BMI) using data from the National Health and Nutrition Examination Survey (NHANES). Through linear regression analysis, we explore whether age is a significant predictor of BMI in the U.S. population.

## Research Question
**Does age have a significant relationship with BMI?**

## Key Findings
- Age is a **statistically significant** predictor of BMI (p < 0.001)
- Age explains approximately **16.6%** of BMI variation (R² = 0.166)
- For every one-year increase in age, BMI increases by approximately **0.06 units**
- The remaining **83%** of BMI variation is attributable to other factors (diet, genetics, physical activity, etc.)

## Files
- `analysis.Rmd` - R Markdown source code with full analysis
- `analysis.html` - Knitted HTML report with results and visualizations

## Dataset
**NHANES (National Health and Nutrition Examination Survey)**
- Sample size: 9,634 observations (after removing missing values)
- Variables analyzed: Age (years), BMI (Body Mass Index)
- Source: NHANES R package

## Methods
1. **Data Cleaning**: Removed observations with missing Age or BMI values
2. **Exploratory Analysis**: Examined data distribution and missing values
3. **Linear Regression**: Fitted model with BMI as outcome and Age as predictor
4. **Model Diagnostics**: Verified regression assumptions using diagnostic plots
5. **Visualization**: Created scatterplot with regression line

## Statistical Results
- **R² = 0.1664** (moderate effect size)
- **Adjusted R² = 0.1663**
- **F-statistic = 1922** (p < 2.2e-16)
- **Sample size = 9,634**

## Requirements
### R Packages
```r
install.packages(c("ggplot2", "NHANES", "tidyverse"))
```

### R Version
- R version 4.0 or higher recommended
- RStudio (optional, for knitting)

## How to Run
1. Clone this repository
```bash
git clone https://github.com/haruma-kurita/linear_regression.git
```

2. Open `analysis.Rmd` in RStudio

3. Install required packages (see Requirements above)

4. Click "Knit" to generate the HTML report

## View Results
[Click here to view the HTML report](https://htmlpreview.github.io/?https://github.com/haruma-kurita/linear_regression/blob/main/analysis.html)

## Visualizations
The analysis includes:
- Scatterplot of Age vs BMI with regression line
- Diagnostic plots for model validation (residuals, Q-Q plot, etc.)

## Interpretation
While age has a statistically significant relationship with BMI, the moderate R² value (0.166) indicates that age alone is not sufficient to predict BMI accurately. This finding suggests that BMI is influenced by multiple factors beyond age, including:
- Dietary habits
- Physical activity levels
- Genetic factors
- Socioeconomic status
- Lifestyle choices

A multifactorial approach is necessary for comprehensive understanding of BMI variation.

## Author
**Haruma Kurita**  
Date: October 28, 2025

## Acknowledgments
- Data provided by the NHANES R package

## Contact
For questions or feedback, please open an issue in this repository.
