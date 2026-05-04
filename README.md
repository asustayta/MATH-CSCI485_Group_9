# Predicting Life Expectancy in California 

**Author:** Maya A., Matthew B., Neil M., Anna S.

**MATH-CSCI485:** Group 9

## Overview

This project focuses on predicting life expectancy across California census tracts using neighborhood level health, demographic, economic, housing, education, and environmental indicators. We used the California Healthy Places Index 3.0 dataset and combined it with CDC USALEEP life expectancy data to create a cleaned modeling dataset. The main goal was to see whether machine learning models could predict census tract life expectancy better than using the overall HPI score alone. The project includes data cleaning, exploratory analysis, statistical testing, clustering, and predictive modeling using LASSO, two-way ANOVA, K-means, Random Forest, XGBoost, and SHAP interpretation.

## Files Included
   - `DataCleaning.Rmd`: 
   - `Final.Rmd`: 
   - `Final_Updated.Rmd`: 
   - `hpi_clean_full.csv`: cleaned data set aggregated from the following
      - `CA_A.CSV.xlsl`:  CDC’s USALEEP dataset, which provides official life expectancy estimates across the United States containing 7,516 observations and 7 variables.
      - `hpi_3_complete_file.csv`: the California Healthy Places Index 3.0 (HPI), containing 8,057 California census tracts and 84 variables representing various aspects of community health.
     
  
## Execution

Packages Included: 
  - tidyverse
  - ggplot2
  - glmnet
  - readxl
  - randomForest
  - rsample
  - shapviz
  - skimr
  - yardstick
  - xgboost

 ## Summary

The analysis showed that life expectancy is strongly related to neighborhood conditions, especially education, poverty, income, employment, housing, and demographic variables. LASSO was used to select the most important predictors, which were then used in clustering and machine learning models. The two-way ANOVA showed that both region and income quartile had significant relationships with life expectancy. K-means clustering grouped census tracts into four clusters that showed clear differences in average income, HPI score, and life expectancy. Random Forest and XGBoost were then used to predict life expectancy, and both performed better than the simple HPI baseline model. Overall, XGBoost had the best performance, suggesting that using multiple neighborhood indicators provides a better prediction of life expectancy than relying on the HPI score alone.
