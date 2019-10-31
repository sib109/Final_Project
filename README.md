# Final_Project

## Background
This project explores the causes of cancer. In the course of this project, 6 factors have been explored:
* Obesity
* Physical Activity
* Alcohol Consumption
* Smoking
* Poverty
* Fast Food Availability

## Data Collection
Global Health Data Exchange (GHDx) is a new data catalog for demographic, public health and global health data. It was developed by the Institute for Health Metrics and Evaluation (IHME) at the University of Washington and it complements HealthData.gov data and hosts large health-related datasets and is geared towards providing  innovators and entrepreneurs to access and utilize federal health related datasets.  

* Cancer mortality (number of deaths attributed to cancer per 100K people), Smoking Prevalence (number of smokers per 100 people), Alcohol Prevalence (Heavy (defined as 2 drinks per day) drinking per 100 people) data has been sourced from GHDx website (http://ghdx.healthdata.org/record/ihme-data/united-states-cancer-mortality-rates-county-1980-2014 )

* Obesity (number of people per 100 defined as Obese) and Physical Activity (number of people per 100 with any sort of physical activity) has been sourced from the IMHE website ( http://www.healthdata.org/us-health/data-download )

* Poverty data came from US Government census ( https://www.census.gov/data-tools/demo/saipe/#/?map_geoSelector=aa_c&s_year=2011,2010,2009,2008,2007,2006,2005&map_yearSelector=2011 )

* Fast Food data came from the USDA Economic Research Service (https://www.ers.usda.gov/amber-waves/2010/december/data-feature-compare-your-areas-food-environment-with-the-rest-of-the-country/ )

## Data Cleansing
* Data has been cleaned, merged and made ready for model and Tableau by a mix of Python and Excel codes

* The individual state files combine to 1.12 GB and it could not be uploaded. Only the Alabama file for cancer mortality has been uploaded

## Data Analysis
### Descriptive Analysis

Descriptive analysis was conducted on the data using Tableau. The link to the Tableau Public page is provided below:

https://public.tableau.com/profile/sibasish.sinha#!/vizhome/FinalProject_15720800732710/Map-AlcoholConsumption?publish=yes

### Predictive Analysis

* For the predictive analysis part, first mortality data was checked for spread. Then correlation of the factors was checked. We can see that Mortality is positively correlated with Obesity, Smoking, Poverty, while negatively correlated with Physical Activity, Alcohol Consumption and almost not correlated with Fast Food Consumption

* After reshaping the data, and splitting the dataset into test and train, a multilinear regression model was built. The R2 came to .52, which was less than what was expected considering the factors were handpicked and trustworthy data was used to build the model

*   Or it could simply mean that the factors chosen are not capable of predicting cancer mortality. And there are 100s of cancer varieties, each with their own causes and idiosyncrasies, might be narrowing to a specific type of cancer could make these variables “predictors”


