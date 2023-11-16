![Alt text](Images/airplane_readme_final.png)
# Aviation Exploration Analysis
## Overview
- Our company is making the venture into the airline industry in order to diversify our portfolio. We have been tasked with determining which aircraft carry the lowest risk. The data has been provided in this [Aviation Accident Database 1948-2022](https://www.kaggle.com/datasets/khsamaha/aviation-accident-database-synopses) which is publicly available through [kaggle](https://www.kaggle.com/) datasets.  
## Business Understanding
- Requirements and Objectives from our new director of aviation is to decide which aircraft our less accident prone and generally safer so that our company can purchase them
## Data Understanding
### Examining the data with a wider lens
We were given a `.csv` file of raw data from the National Transportation Safety Board [NTSB](https://www.ntsb.gov/Pages/AviationQueryv2.aspx) that we imported into a jupyter notebook
#### Rows
- Specifies that each incident that occurs with aircraft as an `'accident'` 
##### Columns
- The location and region of where accidents occured
- The specifications of each aircraft including the make, model, engine type, and # engines
- Total Injuries
- Flight Status as well as weather conditions on that day.
## Data Preparation (Can be really short in README)
## Analysis and Results/Recommendations
### Recommendation 1: Safest Engine 'type' based off fatal vs non fatal injuries
- For the first business recommendation. We have analyzed percentages of fatal vs non fatal injuries according to the engine type of each aircraft in the dataset. The first engine we could recommend based off our data is **turbo fan**. The although this next recommendation should be taken with caution as it is involved with many incidents, **reciprocating** is another engine type we can recommend based on perecenatga of average fatal injuries.  
- We are excluding electric, geared turbofan, and turbo shaft because we have fewer than 12 data points for these 3 types of engines. 
### Recommendation 2: Single Engine Plane has less fatalities but more damage
- More damage in a single engine plane, but cheaper to purchase and maintain
- Cost effective 
- Twin or 2 engine plane has the highest fatal injury rate, but when an incident occurs it has a lower rate of aircraft damage
### Final Recommendation: Purchasing Airplanes based on make
- The 'make' of the planes that we can recommend purchasing from are Airbus, Boeing, and McDonnell Douglas. These airplane makes have the lowest aircraft damage and the lowest amount of fatalities. 
## Conlusion and Next Steps
## Repo Structure
```
├── Data
├── Images
├── Notebooks
│   ├──
│   ├── 
│   ├── 
├── Final.ipynb
├── README.md
```