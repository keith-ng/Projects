## Singapore Flats Prediction

### Description:

- This project seeks to utilise regression models to predict the prices of Flats in Singapore. 
- The valuation model will be constructed based on a data set with data from 2017 to early 2021. 
- Final model accuracy of 96.21%.

### Process:

- Data preprocessing. 
- Exploratory Data Analysis
- A variety of regression models were applied and the model with the highest R2 score was selected. 
- Data transformed and refined through normalisation.
- Final Model used: Random Forest with a R2 score of 0.9621

### Files used:

- dataset/prices.csv -- dataset containing details of Singapore flats transaction from 2017 to early 2021.

### Codebook / Data Dictionary:

**features.csv**
- month - date of transaction
- town - general location of flat
- flat_type - type of flat
- block - block number where flat resides in
- street_name - specific location of flat by street name
- floor_area_sqm - size of flat in square meters
- flat_model - model of flat
- lease_commence_date - year where lease starts
- remaining_lease - number of years and months remaining on lease
- resale_price - price where flat was sold
  
### Project Status:
- Plans to refine the model further are subjected to availability.
