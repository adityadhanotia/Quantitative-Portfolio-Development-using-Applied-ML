# Quantitative Portfolio Development and Evaluation with Applied ML 

## Overview
This project focuses on the development and evaluation of a stock portfolio strategy utilizing both traditional financial analysis and advanced machine learning techniques. Our objective was to create a robust investment approach that minimizes risk and maximizes potential returns by identifying 100 undervalued stocks to invest in from a universe of securities and use Machine Learning to re-balance the portfolio weights each month for optimal portfolio returns. The project is inspired by the long-investing value style approach highlighted by AQR Capital Management and Alpha Architect. 

### Data Source
The securities data used in this project is sourced from the CRSP and COMPUSTAT monthly stocks dataset, which can be accessed and downloaded from [Wharton Research Data Services](https://wrds-www.wharton.upenn.edu/).

### Filtering Process
Our strategy began with a comprehensive analysis of the dataset, employing a series of filters based on financial metrics and ratios. These filters aimed to identify undervalued stocks and minimize the risk of capital loss. Key criteria included:

- **Low Accruals**: To avoid companies potentially engaging in accounting manipulations.
- **Profitability**: Metrics highlighting the profitability of companies.
- **Debt Servicing Ability**: Indicators of a company's ability to service its debt.
- **Solvency**: Measures ensuring the financial health and sustainability of companies.

This rigorous filtering process was instrumental in narrowing down our initial universe to a select group of 100 undervalued stocks.

### Machine Learning Integration
In addition to traditional financial analysis, we incorporated machine learning techniques to estimate the expected returns of the selected stocks and allocated weights based on expected returns. Recognizing the difficulty of this task, we aimed to extract any useful signal from the models that will allow for a slightly improved portfolio weighting system that can provide marginally improved returns. Given our skepticism about the potential accuracy of these predictive models, however, we also need to be careful that we aren’t overly reliant on them and creating an irresponsible amount of variance in our weights that could greatly increase portfolio risk. More on weighting mechanism be found in the report. 

### Benchmark Comparison
To evaluate the effectiveness of our machine learning-augmented approach, we established a benchmark weighting system based on an equally weighted portfolio where each stock has a weight of 0.01. 

## Results
The report presents detailed results of our analysis, including performance metrics of the selected stock filters in various combinations. We also discuss the implications of these findings for the potential application and refinement of our investment strategy.

## How to Use
1. **Download the Data**: Access and download the CRSP monthly stocks dataset from [Wharton Research Data Services](https://wrds-www.wharton.upenn.edu/).
2. **Set Up Environment**: Ensure you have the required Python packages installed.
