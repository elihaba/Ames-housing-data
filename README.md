# Analysis of Features That Drive Home Prices in Ames, IA

### Overview

The Central Iowa Board of Realtors seeks to understand the factors influencing home sale prices in Ames, Iowa, following a 1.5% decline in home values over the past year, despite a national increase of 2.7%. The objective is to analyze housing data to identify key variables that impact home prices at the time of sale. The insights from this analysis will inform pricing strategies and market predictions for real estate professionals in the region.

---

## Table of Contents
1. [Data](#Data)
2. [Requirements](#Requirements) 
3. [Executive Summary](#Executive-summary)

---

## Data
data source (kaggle)

- [Training Data](../datasets/train.csv)
- [Testing Data](../datasets/test.csv)


### Data Dictionary


|Feature|Type|Dataset|Description|
|---|---|---|---|
|SalePrice|int|train.csv|The price of a home at sale 
|Overall Qual|int|train.csv|The overall quality of a home on a scale of 1-10
|Gr Liv Area|int|train.csv|The total above ground square footage of a home 
|Garage Area|float|train.csv|The square footage of a home's garage 
|Total Bsmt SF|float|train.csv|The square footage of a home's basement 


---

## Requirements

- A programming environment such as Jupyter Lab
- pandas
- numpy
- matplotlib.pyplot
- scikit-learn
- seaborn

---

## Executive Summary
The real estate market in Ames, Iowa has enjoyed consistent growth in home values over the past 8 years (Zillow). However, recent data reveals the average home value in Ames has declined by 1.5% over the last year, in stark contrast to the national trend, where home values rose by 2.7% during the same period (Zillow). This discrepancy has raised questions among local real estate professionals, prompting the Central Iowa Board of Realtors, a local association understandably invested in sale prices, to seek a deeper understanding of the factors driving home prices.

To address this, I have been engaged to attempt to construct a model that can forecast a house's price at sale. The goal of this analysis is not understand local or national trends that might cause a dip or rise in home value, but to better understand the valuation of existing housing stock.


#### Purpose

The objective of this analysis is to leverage historical data provided by the Central Iowa Board of Realtors, including key housing features and corresponding sale prices, to develop an accurate model for forecasting the expected sale price of a home. The commission has set a performance benchmark, requiring a model to achieve a minimum R² score of 85% in order to be considered for integration into the pricing strategy. This analysis aims to deliver a robust, data-driven solution that enhances the accuracy and reliability of home price predictions in the Ames real estate market.
  
#### Methods
The dataset provided was comprehensive and offered a wealth of features to explore. I began by analyzing the data to identify the variables most strongly correlated with a home’s sale price. After compiling an initial list of relevant features, I developed a linear regression model and trained it on the dataset. Through an iterative process, I evaluated model performance and incrementally added features to improve predictive accuracy. Ultimately, I arrived at a model incorporating 29 predictors, achieving an R² score of 0.8917, or just over 89%.

#### Findings
The leading features that positively impacted home prices were square footage and overall quality of the home. Many other features contributed, both positively and negatively, but these two had the strongest correlations.

#### Next Steps
More research should be done on regional changes to uncover the cause of the drop in home value to better implement this model when setting home prices. 
