# eBay Predict Used Car Prices
Cars are well-known as having a high depreciation rate. Therefore, purchasing used car can usually be economically more favorable for many people. *eBay Kleinanzeigen* is a classfied advertising section of the German eBay website. Here I will work with [a dataset](https://www.kaggle.com/orgesleka/used-cars-database/data) which was orinigally scraped from *eBay Kleinanzeigen*, for the used car sell information. **My goal is to build a model that predicts the price of the used car**..

## Code and Resources Used

**Python Version**: 3.7

**Packages**: pandas, numpy 

**Data Source**: https://www.kaggle.com/orgesleka/used-cars-database/data

## Data Cleaning
The following data cleaning steps were applied:
- Removed irrelevant columns
- Removed missing data
- Fill missing data with proper values. I noticed *brand* column does not have missing data, therefore I filled missing data that is relevant to brand by the most frequent value in each brand
- Removed outliers in price, odometer reading, registration year, and power
- Removed odometer reading for final model building as it contains significant number of same values

# Model Building
I built a model using Random Forest Regressor and performed hyper-parameter tuning. The final accuracy is **87.5%**.
