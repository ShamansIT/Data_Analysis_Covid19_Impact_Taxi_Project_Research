# Data Analysis Covid19 Impact Taxi Project Research
The research date project of the impact of the Covid-19 epidemic on the trips of the New York City Taxi and Limousine Service (TLC) for the period 2015-2023.

## Project Scope and Data
The project's scope encompasses analyzing the effects of the Covid-19 epidemic on taxi trips within the New York City Taxi and Limousine Service (TLC) from 2015 to 2023. The dataset selected for analysis was chosen based on its accuracy and comprehensive data content. It includes data for each month throughout the specified period.

## Dataset Details
- Number of Data Files Processed: 328
- Total Data: 124 Gb

### Data Taxi dictionary

[Taxi Trip Records Data](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page)

### Describe Taxi data
Yellow and green taxi trip records include fields capturing pick-up and drop-off dates/times, pick-up and drop-off locations, trip distances, itemized fares, rate types, payment types, and driver-reported passenger counts. The data used in the attached datasets were collected and provided to the NYC Taxi and Limousine Commission (TLC) by technology providers authorized under the Taxicab & Livery Passenger Enhancement Programs (TPEP/LPEP). The trip data was not created by the TLC, and TLC makes no representations as to the accuracy of these data.

For-Hire Vehicle (“FHV”) trip records include fields capturing the dispatching base license number and the pick-up date, time, and taxi zone location ID (shape file below). These records are generated from the FHV Trip Record submissions made by bases. Note: The TLC publishes base trip record data as submitted by the bases, and we cannot guarantee or confirm their accuracy or completeness. Therefore, this may not represent the total amount of trips dispatched by all TLC-licensed bases. The TLC performs routine reviews of the records and takes enforcement actions when necessary to ensure, to the extent possible, complete and accurate information.

### Yellow NYC Taxi Trip Records Dictionary
This document provides a data dictionary for the New York City Taxi Trip Records dataset, specifically focusing on the yellow taxi trips. The dataset is made available by the NYC Taxi and Limousine Commission (TLC).

### Data Yellow NYC Taxi Trip Records Fields
Field Name              | Description                                                                                           
------------------------|-------------------------------------------------------------------------------------------------------
VendorID                | A code indicating the TPEP provider that provided the record. 1= Creative Mobile Technologies, LLC; 2= VeriFone Inc.
tpep_pickup_datetime   | The date and time when the meter was engaged.
tpep_dropoff_datetime  | The date and time when the meter was disengaged.
Passenger_count         | The number of passengers in the vehicle. This is a driver-entered value.
Trip_distance           | The elapsed trip distance in miles reported by the taximeter.
PULocationID            | TLC Taxi Zone in which the taximeter was engaged.
DOLocationID            | TLC Taxi Zone in which the taximeter was disengaged.
RateCodeID              | The final rate code in effect at the end of the trip. 1= Standard rate, 2= JFK, 3= Newark, 4= Nassau or Westchester, 5= Negotiated fare, 6= Group ride.
Store_and_fwd_flag      | This flag indicates whether the trip record was held in vehicle memory before sending to the vendor, aka “store and forward,” because the vehicle did not have a connection to the server. Y= store and forward trip, N= not a store and forward trip.
Payment_type            | A numeric code signifying how the passenger paid for the trip. 1= Credit card, 2= Cash, 3= No charge, 4= Dispute, 5= Unknown, 6= Voided trip.
Fare_amount             | The time-and-distance fare calculated by the meter.
Extra                   | Miscellaneous extras and surcharges. Currently, this only includes the $0.50 and $1 rush hour and overnight charges.
MTA_tax                 | $0.50 MTA tax that is automatically triggered based on the metered rate in use.
Improvement_surcharge   | $0.30 improvement surcharge assessed trips at the flag drop. The improvement surcharge began being levied in 2015.
Tip_amount              | Tip amount – This field is automatically populated for credit card tips. Cash tips are not included.
Tolls_amount            | Total amount of all tolls paid in trip.
Total_amount            | The total amount charged to passengers. Does not include cash tips.
Congestion_Surcharge    | Total amount collected in trip for NYS congestion surcharge.
Airport_fee             | $1.25 for pick up only at LaGuardia and John F. Kennedy Airports.

For more detailed information, refer to the [NYC Taxi Trip Records Yellow Data Dictionary PDF.](https://www.nyc.gov/assets/tlc/downloads/pdf/data_dictionary_trip_records_yellow.pdf)

### Green NYC Taxi Trip Records Dictionary
This document provides a data dictionary for the New York City Taxi Trip Records dataset, specifically focusing on the green taxi trips. The dataset is made available by the NYC Taxi and Limousine Commission (TLC).

### Data Green NYC Taxi Trip Records Fields
Field Name               | Description                                                                                          
------------------------|-----------------------------------------------------------------------------------------------------
VendorID                 | A code indicating the LPEP provider that provided the record. 1= Creative Mobile Technologies, LLC; 2= VeriFone Inc.
lpep_pickup_datetime    | The date and time when the meter was engaged.
lpep_dropoff_datetime   | The date and time when the meter was disengaged.
Passenger_count         | The number of passengers in the vehicle. This is a driver-entered value.
Trip_distance           | The elapsed trip distance in miles reported by the taximeter.
PULocationID            | TLC Taxi Zone in which the taximeter was engaged.
DOLocationID            | TLC Taxi Zone in which the taximeter was disengaged.
RateCodeID              | The final rate code in effect at the end of the trip. 1= Standard rate, 2= JFK, 3= Newark, 4= Nassau or Westchester, 5= Negotiated fare, 6= Group ride.
Store_and_fwd_flag      | This flag indicates whether the trip record was held in vehicle memory before sending to the vendor, aka “store and forward,” because the vehicle did not have a connection to the server. Y= store and forward trip, N= not a store and forward trip.
Payment_type            | A numeric code signifying how the passenger paid for the trip. 1= Credit card, 2= Cash, 3= No charge, 4= Dispute, 5= Unknown, 6= Voided trip.
Fare_amount             | The time-and-distance fare calculated by the meter.
Extra                   | Miscellaneous extras and surcharges. Currently, this only includes the $0.50 and $1 rush hour and overnight charges.
MTA_tax                 | $0.50 MTA tax that is automatically triggered based on the metered rate in use.
Improvement_surcharge   | $0.30 improvement surcharge assessed on hailed trips at the flag drop. The improvement surcharge began being levied in 2015.
Tip_amount              | Tip amount – This field is automatically populated for credit card tips. Cash tips are not included.
Tolls_amount            | Total amount of all tolls paid in trip.
Total_amount            | The total amount charged to passengers. Does not include cash tips.
Trip_type               | A code indicating whether the trip was a street-hail or a dispatch that is automatically assigned based on the metered rate in use but can be altered by the driver. 1= Street-hail, 2= Dispatch.

For more detailed information, refer to the [NYC Taxi Trip Records Green Data Dictionary PDF.](https://www.nyc.gov/assets/tlc/downloads/pdf/data_dictionary_trip_records_green.pdf)

### FHV Trip Records
This document provides a data dictionary for the New York City Taxi Trip Records dataset, specifically focusing on the For-Hire Vehicle (FHV) trips. The dataset is made available by the NYC Taxi and Limousine Commission (TLC).

### Data FHV Trip Records Fields
Field Name                | Description                                                                                          
--------------------------|-------------------------------------------------------------------------------------------------------
dispatching_base_num      | TLC base license number of the base that dispatched the trip.
Pickup_date               | The date of the trip.
locationID                | TLC Taxi Zone in which the trip ended.
PUlocationID              | TLC Taxi Zone in which the trip began.

For more detailed information, refer to the [NYC Taxi Trip Records For-Hire Vehicle (FHV) Data Dictionary PDF.](https://www.nyc.gov/assets/tlc/downloads/pdf/data_dictionary_trip_records_fhv.pdf)


### Convector Taxi data
The files from format **.parquet** have been converted by **parquet_to_csv_convector.py** into **.csv** files for more convenient use and data processing. 
To convert four files that could not be converted due to an error in the conversion stage due to the presence of data corruption, separate **parquet_to_csv_convector_error_protection.py** convector was written, which reads the data line by line into the data frame (DF) exceptions detected errors in the records. Once this operation is complete, the file is saved to **.csv** format with name **output.csv**. The total processing time of one file varies within 35-45 minutes, depending on the hardware capabilities. The list of files converted this way: fhv_tripdata_2017-06, fhv_tripdata_2018-05, fhv_tripdata_2018-06, fhv_tripdata_2018-08.


### COVID-19 Health Data dictionary

[NYC Open Data: COVID-19 Daily Counts of Cases, Hospitalizations, and Deaths](https://data.cityofnewyork.us/Health/COVID-19-Daily-Counts-of-Cases-Hospitalizations-an/rc75-m7u3/about_data)

### Describe COVID-19 Health Data
Daily count of NYC residents who tested positive for SARS-CoV-2, who were hospitalized with COVID-19, and deaths among COVID-19 patients.
Note that this dataset currently pulls from **https://raw.githubusercontent.com/nychealth/coronavirus-data/master/trends/data-by-day.csv** on a daily basis.

| **Dataset Information** |                               |
|-------------------------|-------------------------------|
| **Agency**              | Department of Health and Mental Hygiene (DOHMH) |
| **Update Frequency**    | Daily                         |
| **Automation**          | Yes                           |
| **Date Made Public**    | 5/19/2020                     |



### Data COVID-19 Health

| **Column Name**                 | **Description**                                                                                          | **Type**     |
|---------------------------------|----------------------------------------------------------------------------------------------------------|--------------|
| **date_of_interest**              | Date of COVID-19 diagnosis (i.e., date of specimen collection), hospital admission, or death             | Date & Time  |
| **CASE_COUNT**                    | Count of patients tested who were confirmed to be COVID-19 cases on **date_of_interest**                    | Number       |
| **PROBABLE_CASE_COUNT**           | Count of probable COVID-19 cases on **date_of_interest**                                                   | Number       |
| **HOSPITALIZED_COUNT**            | Count of COVID-19 patients who were hospitalized on **date_of_interest**                                   | Number       |
| **DEATH_COUNT**                   | Count of deaths occurring among confirmed COVID-19 cases on **date_of_interest**                           | Number       |
| **CASE_COUNT_7DAY_AVG**           | 7-day average of confirmed COVID-19 cases                                                                | Number       |
| **ALL_CASE_COUNT_7DAY_AVG**       | 7-day average of all COVID-19 cases (confirmed and probable)                                             | Number       |
| **HOSP_COUNT_7DAY_AVG**           | 7-day average of hospitalized COVID-19 cases                                                             | Number       |
| **DEATH_COUNT_7DAY_AVG**          | 7-day average of deaths among confirmed COVID-19 cases                                                   | Number       |
| **BX_CASE_COUNT**                 | Count of confirmed COVID-19 cases in the Bronx                                                           | Number       |
| **BX_PROBABLE_CASE_COUNT**        | Count of probable COVID-19 cases in the Bronx                                                            | Number       |
| **BX_HOSPITALIZED_COUNT**         | Count of hospitalized COVID-19 cases in the Bronx                                                        | Number       |
| **BX_DEATH_COUNT**                | Count of deaths among confirmed COVID-19 cases in the Bronx                                              | Number       |
| **BX_CASE_COUNT_7DAY_AVG**        | 7-day average of confirmed COVID-19 cases in the Bronx                                                   | Number       |
| **BX_PROBABLE_CASE_COUNT_7DAY_AVG**| 7-day average of probable COVID-19 cases in the Bronx                                                    | Number       |
| **BX_ALL_CASE_COUNT_7DAY_AVG**    | 7-day average of all COVID-19 cases in the Bronx (confirmed and probable)                                 | Number       |
| **BX_HOSPITALIZED_COUNT_7DAY_AVG**| 7-day average of hospitalized COVID-19 cases in the Bronx                                                | Number       |
| **BX_DEATH_COUNT_7DAY_AVG**       | 7-day average of deaths among confirmed COVID-19 cases in the Bronx                                      | Number       |
| **BK_CASE_COUNT**                 | Count of confirmed COVID-19 cases in Brooklyn                                                            | Number       |
| **BK_PROBABLE_CASE_COUNT**        | Count of probable COVID-19 cases in Brooklyn                                                             | Number       |
| **BK_HOSPITALIZED_COUNT**         | Count of hospitalized COVID-19 cases in Brooklyn                                                         | Number       |
| **BK_DEATH_COUNT**                | Count of deaths among confirmed COVID-19 cases in Brooklyn                                               | Number       |
| **BK_CASE_COUNT_7DAY_AVG**        | 7-day average of confirmed COVID-19 cases in Brooklyn                                                    | Number       |
| **BK_PROBABLE_CASE_COUNT_7DAY_AVG**| 7-day average of probable COVID-19 cases in Brooklyn                                                     | Number       |
| **BK_ALL_CASE_COUNT_7DAY_AVG**    | 7-day average of all COVID-19 cases in Brooklyn (confirmed and probable)                                 | Number       |
| **BK_HOSPITALIZED_COUNT_7DAY_AVG**| 7-day average of hospitalized COVID-19 cases in Brooklyn                                                 | Number       |
| **BK_DEATH_COUNT_7DAY_AVG**       | 7-day average of deaths among confirmed COVID-19 cases in Brooklyn                                       | Number       |
| **MN_CASE_COUNT**                 | Count of confirmed COVID-19 cases in Manhattan                                                           | Number       |
| **MN_PROBABLE_CASE_COUNT**        | Count of probable COVID-19 cases in Manhattan                                                            | Number       |
| **MN_HOSPITALIZED_COUNT**         | Count of hospitalized COVID-19 cases in Manhattan                                                        | Number       |
| **MN_DEATH_COUNT**                | Count of deaths among confirmed COVID-19 cases in Manhattan                                              | Number       |
| **MN_CASE_COUNT_7DAY_AVG**        | 7-day average of confirmed COVID-19 cases in Manhattan                                                   | Number       |
| **MN_PROBABLE_CASE_COUNT_7DAY_AVG**| 7-day average of probable COVID-19 cases in Manhattan                                                    | Number       |
| **MN_ALL_CASE_COUNT_7DAY_AVG**    | 7-day average of all COVID-19 cases in Manhattan (confirmed and probable)                                | Number       |
| **MN_HOSPITALIZED_COUNT_7DAY_AVG**| 7-day average of hospitalized COVID-19 cases in Manhattan                                                | Number       |
| **MN_DEATH_COUNT_7DAY_AVG**       | 7-day average of deaths among confirmed COVID-19 cases in Manhattan                                      | Number       |
| **QN_CASE_COUNT**                 | Count of confirmed COVID-19 cases in Queens                                                              | Number       |
| **QN_PROBABLE_CASE_COUNT**        | Count of probable COVID-19 cases in Queens                                                               | Number       |
| **QN_HOSPITALIZED_COUNT**         | Count of hospitalized COVID-19 cases in Queens                                                           | Number       |
| **QN_DEATH_COUNT**                | Count of deaths among confirmed COVID-19 cases in Queens                                                 | Number       |
| **QN_CASE_COUNT_7DAY_AVG**        | 7-day average of confirmed COVID-19 cases in Queens                                                      | Number       |
| **QN_PROBABLE_CASE_COUNT_7DAY_AVG**| 7-day average of probable COVID-19 cases in Queens                                                       | Number       |
| **QN_ALL_CASE_COUNT_7DAY_AVG**    | 7-day average of all COVID-19 cases in Queens (confirmed and probable)                                   | Number       |
| **QN_HOSPITALIZED_COUNT_7DAY_AVG**| 7-day average of hospitalized COVID-19 cases in Queens                                                   | Number       |
| **QN_DEATH_COUNT_7DAY_AVG**       | 7-day average of deaths among confirmed COVID-19 cases in Queens                                         | Number       |
| **SI_CASE_COUNT**                 | Count of confirmed COVID-19 cases in Staten Island                                                       | Number       |
| **SI_PROBABLE_CASE_COUNT**        | Count of probable COVID-19 cases in Staten Island                                                        | Number       |
| **SI_HOSPITALIZED_COUNT**         | Count of hospitalized COVID-19 cases in Staten Island                                                    | Number       |
| **SI_DEATH_COUNT**                | Count of deaths among confirmed COVID-19 cases in Staten Island                                          | Number       |
| **SI_PROBABLE_CASE_COUNT_7DAY_AVG**| 7-day average of probable COVID-19 cases in Staten Island                                                | Number       |
| **SI_CASE_COUNT_7DAY_AVG**        | 7-day average of confirmed COVID-19 cases in Staten Island                                               | Number       |
| **SI_ALL_CASE_COUNT_7DAY_AVG**    | 7-day average of all COVID-19 cases in Staten Island (confirmed and probable)                            | Number       |
| **SI_HOSPITALIZED_COUNT_7DAY_AVG**| 7-day average of hospitalized COVID-19 cases in Staten Island                                            | Number       |
| **SI_DEATH_COUNT_7DAY_AVG**       | 7-day average of deaths among confirmed COVID-19 cases in Staten Island                                  | Number       |
| **INCOMPLETE**                    | Count of incomplete COVID-19 cases                                                                        | Number       |
