![Alt text](Images/airplane_readme_final.png)
# Aviation Exploration Analysis
## Overview
Our company is making the venture into the airline industry in order to diversify our portfolio. We have been tasked with determining which aircraft carry the lowest risk. The data has been provided in this [Aviation Accident Database 1948-2022](https://www.kaggle.com/datasets/khsamaha/aviation-accident-database-synopses) which is publicly available through [kaggle](https://www.kaggle.com/) datasets.  
## Business Understanding
Requirements and objectives from our new director of aviation is to decide which aircraft our less accident prone and generally safer so that our company can purchase them.
## Data Understanding
### Examining the data with a wider lens
We were given a `.csv` file [Aviation_Data](https://github.com/pyamin1878/Airline_DS_Project/blob/main/Data/Aviation_Data.csv) of raw data from the National Transportation Safety Board [NTSB](https://www.ntsb.gov/Pages/AviationQueryv2.aspx) that we imported into a jupyter notebook with [pandas](https://pandas.pydata.org/) a flexible python tool for data analysis and manipulation. 
### Rows
- Specifies that each incident that occurs with aircraft as an `'accident'` 
### Columns
- The location, region, and event date of where accidents occured
- The specifications of each aircraft including the make, model, engine type, and `n` of engines
- Injuries were listed in columns with subcategories: fatal, nonfatal, minor, and injured
- The last few columns mention flight status as well as weather conditions

There was also a substantial portion of the dataset that contained null values. 
## Data Preparation
In order to prepare the data for analysis and visualization for business recommendations, alot of cleaning and manipulation was required. Creating a subset of the data into relevant columns was the first step. We also had the issue of null values which were replaced with zeros, measures of central tendency such as **mean**, **median**, and **mode**, as well as filling values with 'unknown' and 'N/A' that could not be filled with numerical values like floats and integers. Lastly we used a pandas method [.groupby()](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.groupby.html) to aggregate and transform the data.
## Analysis and Results/Recommendations
### Recommendation 1: Safest Engine 'type' based off fatal vs non fatal injuries
- For the first business recommendation. We have analyzed percentages of fatal vs non fatal injuries according to the engine type of each aircraft in the dataset. The first engine we could recommend based off our data is **turbo fan**. Although this engine type we can recommend should be taken with caution as it is involved with many incidents, **reciprocating** is another engine type we can recommend based on perecenatga of average fatal injuries.  
- We are excluding electric, geared turbofan, and turbo shaft because we have fewer than 12 data points for these 3 types of engines. 
### Recommendation 2: Single Engine Plane has less fatalities but more damage
- There is more damage in a single engine plane based on average percentages in our data, but they are much more cost effective to purchase and maintain. 
- Twin or 2 engine plane has the highest fatal injury rate, but when an incident occurs it has a lower rate of aircraft damage.
### Recommendation 3: Purchasing Airplanes based on make
- The 'make' of the planes that we can recommend purchasing from are Airbus, Boeing, and McDonnell Douglas. These airplane makes have the lowest aircraft damage and the lowest amount of fatalities. 
## Conlusion and Next Steps
We can assert that Boeing and Airbus are the two aviation companies that are making the highest calibre of aircraft for safety. If we are purchasing for chartered flights or private jets it's best to go with single engine airplanes. Otherwise dual engine airplanes would be the best fit for commercial usage.
## Repo Structure
```
├── Data
├── Final Data
├── Images
├── Notebooks
│   ├──
│   ├── 
│   ├── 
├── Final.ipynb
├── README.md
```