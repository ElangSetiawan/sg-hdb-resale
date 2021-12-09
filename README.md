# Capstone Project: Singapore HDB Resale Price Prediction
___

<p align = 'center'>
  <img src = "https://github.com/ElangSetiawan/sg-hdb-resale/blob/main/images/hdb_shintaro_tay_st_photo.jpg?raw=true" width = 75%>
<p/>
Source : https://www.straitstimes.com/singapore/housing/households-that-received-help-with-mortgage-payments-nearly-triple-that-of-same


**Problem Statement**

Public housing in Singapore is subsidised housing built and managed by the government under the Housing and Development Board (HDB). Most public housing in Singapore is owner-occupied. Under Singapore’s housing ownership programme, housing units are sold to applicants who meet certain income, citizenship and property ownership requirements, on a 99-year leasehold. The estate’s land and common areas continue to be owned by the government. Owner-occupied public housing can be sold to others in a resale market, subject to certain restrictions. Prices within the resale market are not regulated by the government.

Demand for resale flats since the end of the Circuit Breaker has pushed prices and sales to new highs. According to the HDB Price Index in Q2 2021, resale flat prices climbed 3% from Q1 2021, growing for the fifth consecutive quarter since Q2 2020. Prices were also 11% higher compared to a year ago. As data scientists, we want to understand the factors driving the price of resale flats as and provide predicted sale price for property portals.

**Model Explored**

|Models|Description|
|---|---|
|LinearRegression|
|XGBRegressor|


**Evaluation Metrics**

The evaluation metrics will be overfitting/underfitting of less than 2% between train and test data.

**Workflow Process**  
1. Notebook 1 of 2 : General EDA
2. Notebook 1 of 2 : Geolocation preprocessing


**Data Sources**  
1. Singapore postal sector and districts:<br> 
https://www.ura.gov.sg/realEstateIIWeb/resources/misc/list_of_postal_districts.htm
2. Singapore HDB information and resale prices<br>
https://data.gov.sg/dataset/hdb-property-information<br>
https://data.gov.sg/dataset/resale-flat-prices
3. Singapore primary schools<br>
https://en.wikipedia.org/wiki/List_of_schools_in_Singapore
4. Singapore MRT<br>
https://en.wikipedia.org/wiki/List_of_Singapore_MRT_stations
5. Singapore LRT<br>
https://en.wikipedia.org/wiki/List_of_Singapore_LRT_stations
6. Singapore Shopping Malls<br>
https://en.wikipedia.org/wiki/List_of_shopping_malls_in_Singapore

**HDB information and resale transaction prices**
The site data.gov.sg provides both the hdb information dataset as well as the monthly resale transactions. Since old transaction data does not improve the model only dataset from 2017 is considered for this project.

**Geolocation and point of interests**
In this project, it is hypothesized that distance of hdb flat to nearby amenities such as MRT/LRT stations, schools, and shopping centres will be important, these geo informations are obtained via API from https://developers.onemap.sg/commonapi/search? since this provides free geolocation data unlike google map.

**Workflow Process**  
1. Notebook 1 of 2 : General EDA
2. Notebook 1 of 2 : EDA on Geolocation
3. Notebook 2 of 2 : Data Preprocessing
4. Notebook 2 of 2 : Feature Engineering
5. Notebook 2 of 2 : Create Model
6. Notebook 2 of 2 : Iterative Model tuning