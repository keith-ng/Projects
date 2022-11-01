## Walmart Sales Prediction

### Description:

- This project seeks to utilise regression models to predict future sales prices of Walmart's outlets & departments. 
- The valuation model will be constructed based on a data set with data from 2010 to 2012. 
- Final model accuracy is only approximately 92% and may be refined in the future.

### Process:

- Data cleaned in a manner deemed appropriate. 
- Removed outliers which adversely impact the model.
- Discover valuable interaction terms. 
- A variety of regression models were applied and the model with the highest R2 score was selected. 
- Data refined through normalisation, specifically using 'TransformedTargetRegressor'.
- Final Model used: Random Forest with a R2 score of 0.95.

### Differentiating Factors:

- Assigned ordinal variables' weight not proportional. 
- Interaction terms.   

### Files used:

- features.csv -- dataset containing details of some features.
- stores.csv -- dataset containing details of each store.
- train.csv -- dataset containing the target and features such as: 'Dept', 'Date', 'IsHoliday'.
- test.csv -- dataset containing all features data excluding the target.

### Codebook / Data Dictionary:

**features.csv**
- Store - the store number
- Date - the week
- Temperature - average temperature in the region
- Fuel_Price - cost of fuel in the region
- MarkDown1-5 - anonymized data related to promotional markdowns that Walmart is running. MarkDown data is only available after Nov 2011, and is not available for all stores all the time. Any missing value is marked with an NA.
- CPI - the consumer price index
- Unemployment - the unemployment rate
- IsHoliday - whether the week is a special holiday week

**train.csv**
- Store - the store number
- Dept - the department number
- Date - the week
- Weekly_Sales -  sales for the given department in the given store
- IsHoliday - whether the week is a special holiday week
  

### Project Status:
- Plans to refine the model further are subjected to availability.
