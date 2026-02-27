# Predictive Real-Estate Analytics: Advanced Housing Valuation

## Overview

This project involves building a robust predictive model to estimate residential house prices using a comprehensive dataset of 1,460 observations and 81 features. The analysis transitions from exploratory data analysis (EDA) to feature engineering and automated model selection, culminating in a high-accuracy regression model.

## Key Technical Features

* 
**Statistical Foundation:** Leveraged **Linear Regression** and **Model Selection** techniques to identify the most significant drivers of property value.


* 
**Automated Feature Selection:** Utilized the `leaps` and `caret` libraries to perform subset selection, ensuring the final model balances complexity with predictive power.


* 
**Comprehensive EDA:** Conducted deep-dive analysis into variables like `OverallQual`, `GrLivArea`, and `YearBuilt` to understand their correlation with `SalePrice`.



## Tech Stack

* **Language:** R
* 
**Data Manipulation:** `tidyverse` (dplyr, tidyr, readr) 


* 
**Visualization:** `ggplot2`, `corrplot`, `GGally` 


* 
**Machine Learning:** `caret`, `caTools`, `leaps` 


* 
**Time-Series/Logistics:** `lubridate`, `zoo` 



## Methodology

1. 
**Data Ingestion & Cleaning:** Loaded training and test datasets, handling missing values in critical features like `LotFrontage` and `MasVnrArea`.


2. 
**Statistical Profiling:** Used `summary()` and `head()` functions to identify data types, distributions, and potential outliers in the 81 available features.


3. 
**Variable Correlation:** Analyzed the relationship between categorical features (e.g., `Neighborhood`, `SaleCondition`) and numerical features (e.g., `TotalBsmtSF`, `GarageArea`) to refine the feature set.


4. 
**Model Training:** Employed `caTools` for data splitting and `caret` for cross-validation and model training.



## Key Insights

* 
**Quality Metrics:** Features like `OverallQual` and `OverallCond` proved to be among the strongest predictors of sale price.


* 
**Spatial Analysis:** Geographic factors (Neighborhood) and property age (YearBuilt/YearRemodAdd) significantly influenced the final valuation.



---

### How to Run

1. Ensure R and RStudio are installed.
2. Install required packages:
```r
install.packages(c("tidyverse", "caret", "leaps", "corrplot", "GGally", "caTools", "zoo"))

```


3. Load the `train.csv` and `test.csv` files from the data directory.


4. Execute the analysis script to generate the summary statistics and predictive outputs.
