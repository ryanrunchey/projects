FACTORS INFLUENCING SOLAR PV CAPACITY BY ZIP CODE
By Ryan Runchey

----------------------------------------------------------------------------------------------------------------



# Outline

1. Obtain/Munge Raw Data for Initial Exploratory Data Analysis and Pickle Output
    1. Californiadgstats: NEM Currently Interconnected Data Set
    2. CDXTECH: Zip Code Demographic Data
    3. Google Project Sunroof: Zip Code solar potential data
2. Merge Data Sources to Machine Learning DataFrame
3. Linear Regression Modeling
4. Slide Show Presentation .pdf

----------------------------------------------------------------------------------------------------------------



Presentation

* solarpv_presentation.pdf

----------------------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------------------


Workflow

1. solarpv_01_nem_connections.ipynb

    * Opens, explores, cleans, and outputs the California Net Metering Customers Solar PV installations file into "01_df_capacity.pkl". 


2. solarpv_02_zip_code_demographics.ipynb
    
    * Opens, cleans, filters, and outputs the CDXTECH Zip Code demographic data into "02_df_zip.pkl".


3. solarpv_03_solar_insolation.ipynb

    * Opens, cleans, filters, and outputs the Google Project SunRoof solar insolation data into "03_df_solar_ca.pkl".


4. solarpv_04_ml_dataframe.ipynb

    * Merges files 1,2,3 in order to create the machine learning dataframe into "04_df_ml.pkl".


5. solarpv_05_regression.ipynb

    * Opens "04_df_ml.pkl" file and performs machine learning modeling.

----------------------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------------------



# Citations for data sources

* California Distributed Generation Statistics
    * NEM Currently Interconnected Data Set
    * https://www.californiadgstats.ca.gov/download/interconnection_nem_pv_projects/


* CDX Tech
    * Free Demographic Data Reports by Zip Code
    * https://www.cdxtech.com/tools/demographicdata/


* Google Project Sunroof
    * Solar Potential by Postal Code
    * https://bigquery.cloud.google.com/table/bigquery-public-data:sunroof_solar.solar_potential_by_postal_code


# Researched but not used

* California Open Data Portal
    * ZIP Code List
    * https://data.ca.gov/dataset/county-and-zip-code-references/resource/c3527a9a-81c3-48aa-8ba5-022fc8fc753f#{}


* National Solar Radiation Database (NSRDB)
    * Pulling Avg. Annual Insolation by Zip Code
    * https://nsrdb.nrel.gov/content/pulling-avg-annual-insolation-zip-code
    * https://nsrdb.nrel.gov/forums/support-forum
    * https://nsrdb.nrel.gov/download-instructions
    

* United States Internal Revenue Service (IRS)
    * SOI Tax Stats - Individual Income Tax Statistics - 2015 ZIP Code Data (SOI)
    * https://www.irs.gov/statistics/soi-tax-stats-individual-income-tax-statistics-2015-zip-code-data-soi


* National Renewable Energy Laboratory (NREL)
    * Solar Data: These datasets detail the solar resource available in the United States
    * https://www.nrel.gov/gis/data-solar.html


* United States Census Bureau
    * https://www2.census.gov/geo/tiger/TIGER2017/STATE/
    * https://www2.census.gov/geo/tiger/TIGER2017/ZCTA5/
