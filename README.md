# AZ-Pizza-Company-Sales-Report-Documentation

**Documentation Outline**
- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools Used](#tools-used)
- [Data Cleaning and Preparation](#data-cleaning-and-preparation)
- [Data Analysis](#data-analysis)
- [Results and Findings](#results-and-findings)
- [Conclusion and Recommendations](#conclusion-and-recommendations)

## Project Overview
This Data Analysis project aims to get insight from the AZ Pizza Company's Annual Sales data. By analyzing the various parameters in the data set,
I seek to understand sales performance over the mouths of the different categories of pizza product the company produce. 

## Data Sources
The primary source of Data used is pizza_sales.xlsx and this is open source data that was freely downloaded from an open source online data repository site "kaggle"

## Tools Used
- Google
- Power BI
- Power Query Editor

## Data Cleaning and Preparation
The dataset consists of four tables (Pizza sales, Pizzas, Pizza types and Orders) and data cleaning was done for each table.

**Pizza Sales Table**

The cleaning done on this table include
- Promoted Headers: The first row was used as the header
- Change Type: The data type of the columns were change from any to their appropriate data types
- Renamed Columns: The columns were meaningfully renamed

**Pizzas Table**

The cleaning done on this table include
- Promoted Headers: The first row was used as the header
- Change Type: The data type of the columns were change from any to their appropriate data types
- Renamed Columns: The columns were meaningfully renamed

**Pizza Types Table**

The cleaning done on this table include
- Promoted Headers: The first row was used as the header
- Change Type: The data type of the columns were change from any to their appropriate data types
- Renamed Columns: The columns were meaningfully renamed

**Orders Table**

The cleaning done on this table include
- Promoted Headers: The first row was used as the header
- Change Type: The data type of the columns were change from any to their appropriate data types
- Split Columns By Delimiter: The time column that consists of time and date was splitted
- Removed Columns: The columns that were not needed for the analysis were removed  
- Renamed Columns: The columns were meaningfully renamed

## Data Analysis

The dataset only provided quantity sold and the price for each pizza product by size. There was no provision for total sales.

The obtain the total sales, a DAX expression was written as follows:
```
Total Sales = SUMX(pizza_sales, pizza_sales[Quantity] * RELATED(pizzas[Price]))
```



## Results and Findings
![](Data-insight-1.png)
some of the insight drived from the data set are as follows:
- A Total of 44 persons responded spread around 4 African Countries
- There are a Total 33 distinct "Occupations" and 4 distinct "Educational Levels"
- The data shows that about 48% are Females and 52% are Males
- The data also shows that majority of the responses recieved are Singles
- The Age Range are in 5 categories and majority of the responses received are between ages 25 - 29
![](Data-insight-2.png)
![](Data-insight-3.png)
![](Data-insight-4.png)
![](Data-insight-5.png)
![](Data-insight-6.png)

## Conclusion and Recommendations
The data set was transformed using power query editor and loaded into Power BI canva for visualization
and the insight obtained from the data are as follows:
1. About 95% of the students resides in Nigeria
2. Majority of the students are Males and Singles and around the age range of 25-29

It is clear from our analysis from the given dataset that youthful and single Nigerians are very interested in learning new tech skills.
Also it is clear that SkilHarvest Academy has very little presence in other Afrian countries.

## Recommendation
SkilHarvest Academy should increase their advertisments in the other African countries, to give same opportunity to the youths of those countries.
