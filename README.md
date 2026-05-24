# SCE Expected Earnings Regression

This project analyzes expected annual earnings at respondents’ current jobs in 10 years using data from the Survey of Consumer Expectations and the Labor Market Survey. The analysis examines how expected future earnings are associated with age, education level, work status, and household income category.

## Research Question

How are expected annual earnings in 10 years associated with respondents’ age, education level, work status, and household income category?

## Data

The project uses two datasets:

- Survey of Consumer Expectations (SCE) public microdata
- Labor Market Survey public microdata

The datasets were combined using the shared `userid` variable. The outcome variable is `L4b`, which measures respondents’ expected annual earnings at their current job in 10 years.

## Methods

The analysis uses ordinary least squares (OLS) regression to estimate the association between expected future earnings and the following predictors:

- `Q32`: Age
- `Q36`: Education level
- `Q37`: Work status
- `Q47`: Household income category

The project also includes scatterplots showing the relationship between age and expected earnings, including one visualization using a pseudo-log y-axis to improve readability.

## Main Findings

The results suggest that education level and household income category are positively associated with expected future earnings. Work status is negatively associated with expected earnings based on the coding used in the dataset. Age is not statistically significant after controlling for the other predictors. The model explains a modest share of the variation in expected earnings, suggesting that additional job-specific and labor-market variables would improve the model.

## Files

- `SCEAnalysis.qmd`: Quarto source file for the analysis
- `SCEAnalysis.pdf`: Rendered report
- `README.md`: Project overview
