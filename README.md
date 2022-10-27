# **Tanzanian Water Wells Prediction** 
### Authors: [Abduba Galgalo](https://github.com/Abduba011), [Faith Makokha](https://github.com/faithmaks), [Femi Kamau](https://github.com/ctrl-Karugu), [John Mungai](https://github.com/Johnspes), [Susan Mungai](https://github.com/SueMungai), and [Willy Angole](https://github.com/Willy-Angole)

---

> This project is a part of the [Data Science (DSF-FT) Course](https://moringaschool.com/courses/data-science-course/) at [Moringa School](https://moringaschool.com/). The full project description can be found [here](https://github.com/learn-co-curriculum/dsc-phase-3-project-v2-3).


## Overview
Water makes up about 70% of the earth’s surface and is among the few basic needs common to all living creatures. Unfortunately, 96.5 percent of its coverage makes up oceans, which makes up for some scarcity on land.
Tanzania is one of those countries that have to grapple with the scarcity  of this life saving need. As a  developing nation with a population of over 57,000,000,  it has a hard time meeting the demand for safe drinking water due to limited resources for water extraction. There are already some water pumps available in the country but unfortunately, not all are functional and others need repair.  

The World Health Organization- (WHO), understands that three out of ten people still lack access to clean water, highlighting the critical need for investment to improve water hygiene and accessibility. Water poverty has been considered to drive serious illnesses, high infant mortality rates, poor education, slumped economies and unproductive agricultural conditions in a majority of the regions.


---
---

## 1. Business Understanding
#### Problem Statement
Tanzania is currently failing to meet the potable water requirements for its population.  Despite already building water wells to offset this problem, many are unfortunately non-functional and others are in need of repair. 
As a result,  our stakeholder, WHO, has narrowed down their interest to drilling more water wells and maintaining/ revamping  existing ones within the country, in an effort to ensure availability of quality and quantity drinking water countrywide . 

Our role as the data scientist in this project will be to identify patterns in non-functional wells, with the aim of influencing how new ones are built. Furthermore, using these patterns, we will enable our stakeholder to accurately predict existing water points in need of intervention ensuring the people of Tanzania have access to clean potable water

#### Specific Objectives
* To identify the trends/patterns between both non-functional and functional wells 
* To identify non-functioning wells using a simple analysis, and predict the functionality of a well based on available variables.

#### Research Questions
* How can we apply  Machine Learning and necessary classification methods to predict  functionality  of  wells in Tanzania?
* Are there any common features that are consistent with  functional and non-functional wells?
* Can we identify ways to help build better wells?

#### Success Criteria

##### Business Success Criteria (Review)
 * To ensure that newly constructed wells are of good quality water for the communities.
 * To  correctly identify functionality of a well and determine its viability.
 * To successfully predict the type of wells that dry up and determine the type of wells to build based on the area?
 * To determine working wells in different regions and which ones need repair or improved management.
 * To ensure built wells are  longer lasting/ more viable.

##### Project Success Criteria
Generating a model that will be able to correctly predict the quality status of the wells in Tanzania with an accuracy of 80%.




---
### 2. Data Understanding
#### Overview
In this project we shall use a  dataset containing information about existing water wells in Tanzania  sourced from an ongoing  DrivenData competition.


####  2.1 Data Description
The dataset contains 59,400 records and spans 40 columns. Of these columns, we identified 31 to be categorical, and 9 as numerical.  We were able to further group the columns into the general features being captured. Some of the rows include:

Numerical
* amount_tsh - Total static head (amount water available to waterpoint)
* longitude  -  GPS coordinate
* latitude -  GPS coordinate
* gps_height -  Altitude of the well
* population - Population around the well (those living near it)



Categorical
* extraction_type - The kind of extraction the waterpoint uses
* extraction_type_class - The kind of extraction the waterpoint uses
* extraction_type_group  - The kind of extraction the waterpoint uses
* water_quality -  The quality of the water
* quality_group -   The quality of the water
* quantity - The quantity of water
* quantity_group - The quantity of water
* source - The source of the water
* source_type - The source of the water
* source_class - The source of the water
* waterpoint_type - The kind of waterpoint
* waterpoint_type_group - The kind of waterpoint
* status_group - The condition of the wells (target variable)



---
### 3. Data Preparation

his dataset’s analysis and classification will  help our stakeholders to improve maintenance of the present water wells or give useful information for future wells. 

#### 3.1 Data Selection.

There are a lot of repetitive columns in the dataset, for example. `payment` and `payment_type`, `source` and `source_type` which have the same information. We scrapped the columns and for the sake of preparing our data for modelling purposes. 
We have included columns that contain information about the location and the basin that is closest to the water wells geographically. 

#### 3.2  Data Cleaning.

The data was checked for missing values and a number were found in the columns; `funder`, `installer` , `subvillage`, `scheme_management` and `permit`  the percentage of missing values in the particular columns were a small amount, thus were dropped to ensure completeness of the dataset. 
Checking for validity in the data, the dataset was checked for any duplicated values and outliers. The duplicated records were not dropped as it does not mean that they were similar wells but just built under the same project.
We also chose not to drop the outliers, as it did not display erroneous data but will be further looked into in the analysis section. 
After cleaning the dataset, we need to bring uniformity by formatting and the columns to be  readable and easily interpretable.So we defined functions to make these possible.
Moreover, we verified that the values of various columns are consistent. The names of installers and funders had numerous instances of the same funder and/or installer, but with misspelt names and/or typographical errors.


---

### 4. Modeling

---

### 5. Evaluation 

---

### 6. Deployment

---
---

## Repository Structure

* The repository is structured as follows:

```
├── README.md                            <- The top-level README for reviewers of this project
|
├── .gitignore                           <- The .gitignore file for the project
|
├── LICENSE.md                           <- The license for the project
|
├── index.ipynb                          <- Narrative documentation of analysis in Jupyter Notebook
|
└── data                                 <- Datasets used in the analysis
     ├── credit_default.csv
     |          
     └── data_description.txt            
```

---

## Technologies Used

---
## For More Information

* Please review the full analysis in the [Jupyter Notebook](./index.ipynb) or the [Presentation](/presentation.pdf).


---
---

>## *“Keep your eyes on the stars, and your feet on the ground.”* - Theodore Roosevelt
