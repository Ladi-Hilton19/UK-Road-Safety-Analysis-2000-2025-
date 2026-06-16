# UK Road Safety Analysis (2000–2025)

## Project Overview

Road traffic collisions remain a major public safety challenge in the United Kingdom. Understanding where, when, and why accidents occur is critical for policymakers, transport authorities, and road users.

This project analyzes the UK Department for Transport (DfT) STATS19 Road Safety dataset covering collisions, vehicles, and casualties between 2000 and 2025. The objective is to identify accident trends, geographic hotspots, risk factors, casualty patterns, and vehicle involvement while exploring predictive modelling opportunities.

---

## Business Objectives

The analysis was designed to answer the following key questions:

### Trend Analysis

* Are road collisions increasing or decreasing over time?
* Which years recorded the highest casualty volumes?
* Are there seasonal accident patterns?

### Geographic Analysis

* Which local authorities experience the highest collision rates?
* How do urban and rural accident patterns differ?
* Where are major accident hotspots located?

### Risk Analysis

* Which weather conditions contribute most to collisions?
* Which road surface conditions are associated with severe accidents?
* How do day and night accident patterns differ?

### Casualty Analysis

* Which age groups are most affected?
* How do casualty classes differ?
* What is the distribution of fatal, serious, and slight injuries?

### Vehicle Analysis

* Which vehicle types are most frequently involved?
* How do motorcycles compare with cars?
* What role do commercial vehicles play in collision severity?

---

## Dataset Description

The analysis uses the UK Department for Transport STATS19 Road Safety Open Dataset.

Three core datasets were used:

### Collisions Dataset

Contains accident-level information including:

* Location
* Date and time
* Weather conditions
* Road conditions
* Severity
* Local authority information

### Casualties Dataset

Contains information on:

* Casualty age
* Casualty gender
* Casualty class
* Injury severity

### Vehicles Dataset

Contains information on:

* Vehicle type
* Vehicle manoeuvres
* Driver characteristics
* Vehicle conditions

The datasets were sourced from the DfT Open Data Portal and combined with provisional 2025 records.

---

## Data Preparation

### Data Integration

Historical and provisional datasets were concatenated to create a unified dataset covering 2000–2025.

### Data Cleaning

Key cleaning activities included:

* Filtering records between 2000 and 2025
* Handling missing values
* Creating lookup mappings
* Replacing coded values with descriptive labels
* Converting date fields to datetime format
* Extracting month and hour variables
* Creating day/night indicators

### Feature Engineering

Additional analytical features were created:

* Month
* Month Number
* Hour of Day
* Day/Night Category
* Age Bands
* Accident Hotspot Coordinates

---

# Exploratory Data Analysis

## Trend Analysis

### Road Collisions Over Time

A yearly trend analysis revealed long-term changes in collision frequency across the UK.

The analysis indicates that collision volumes generally declined over the study period, reflecting improvements in vehicle safety, road engineering, and traffic enforcement.

### Casualties by Year

Casualty counts were examined annually to identify years with elevated road safety risks.

### Seasonal Patterns

Monthly analysis revealed recurring seasonal patterns in collision activity, suggesting weather conditions, daylight duration, and travel demand influence accident occurrence.

---

## Geographic Analysis

### Local Authority Analysis

Several local authorities consistently recorded higher collision counts than others.

This may be explained by:

* Higher population density
* Greater traffic volumes
* Urban road complexity

### Urban vs Rural Comparison

Urban areas accounted for the majority of collisions due to greater traffic exposure.

However, rural collisions may exhibit higher severity because of:

* Higher travel speeds
* Longer emergency response times
* Reduced road lighting

### Accident Hotspots

Geospatial analysis using latitude and longitude identified clusters of accidents across major population centres and transport corridors.

Interactive maps and heatmaps were created to visualize accident concentrations.

---

## Risk Analysis

### Weather Conditions

Most collisions occurred during fine weather conditions.

This result reflects exposure rather than danger, since most journeys occur during normal weather conditions.

### Road Surface Conditions

Road surface analysis highlighted relationships between:

* Dry roads
* Wet roads
* Frost or ice conditions

and collision severity outcomes.

### Day vs Night Analysis

Daytime collisions occurred more frequently.

Night-time accidents, however, may warrant further investigation because lower visibility can contribute to greater accident severity.

---

## Casualty Analysis

### Casualties by Age Group

Young adults(26-40) represented one of the most affected groups.

Potential contributing factors include:

* Higher exposure
* Commuting behaviour
* Driving experience

### Casualty Classes

Analysis compared:

* Drivers who had the highest number of casualties.
* Passengers
* Pedestrians

to understand differences in injury outcomes.

### Injury Severity Distribution

Most casualties sustained slight injuries.

Serious and fatal injuries represented a smaller proportion of recorded casualties but remain a significant public safety concern.

---

## Vehicle Analysis

### Vehicle Types Most Frequently Involved

Cars accounted for the majority of vehicle involvement.

This result aligns with their dominance in overall road traffic.

### Motorcycles vs Cars

Motorcycle involvement was analyzed separately due to the elevated vulnerability of riders.

### Commercial Vehicles

Goods vehicles were examined to determine whether their involvement was associated with higher collision severity.

---

# Predictive Modelling

## Objective

To explore whether accident characteristics can be used to predict road safety outcomes.

### Model 1: Collision Severity Prediction

Target Variable:

* Collision Severity

Predictor Variables:

* Weather Conditions
* Road Surface Conditions
* Road Type
* Junction Control
* Urban/Rural Classification
* Time Variables
* Number of Vehicles
* Number of Casualties

Algorithm:

* Random Forest Classifier

### Model 2: Casualty Severity Prediction

Target Variable:

* Casualty Severity

Predictor Variables:

* Age
* Gender
* Casualty Class
* Casualty Type

Algorithm:

* Random Forest Classifier

### Model 3: Number of Casualties Prediction

Target Variable:

* Number of Casualties

Predictor Variables:

* Road Characteristics
* Environmental Conditions
* Vehicle Counts

Algorithm:

* Random Forest Regressor

---

## Model Evaluation

Models were evaluated using:

### Classification Models

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix

### Regression Model

* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)
* R² Score

Feature importance analysis was used to identify the strongest predictors influencing collision outcomes.

---

# Key Findings

1. Road collisions generally decreased over time.
2. Collision activity exhibited seasonal patterns.
3. Urban areas experienced the highest collision volumes.
4. Several local authorities emerged as persistent accident hotspots.
5. Weather and road surface conditions influence accident risk.
6. Young adults represented a significant proportion of casualties.
7. Cars were involved in the majority of recorded collisions.
8. Motorcycle users remain a vulnerable road-user group.
9. Predictive models demonstrated that environmental and road characteristics can help explain accident severity.

---

# Recommendations

### Road Safety Policy

* Prioritize interventions in identified hotspot locations.
* Expand targeted enforcement during high-risk periods.

### Infrastructure

* Improve road surface maintenance.
* Enhance lighting in high-risk locations.

### Public Awareness

* Develop campaigns focused on vulnerable age groups.
* Increase motorcycle safety awareness initiatives.

### Future Analytics

* Incorporate traffic volume data.
* Include weather history datasets.
* Apply advanced machine learning techniques such as XGBoost and LightGBM.
* Develop collision risk forecasting dashboards.

---

# Limitations

* Collision records are based on reported incidents.
* Underreporting may exist for minor accidents.
* Traffic exposure measures were not included.
* Provisional 2025 data may be subject to revision.

---

# Conclusion

This analysis provides a comprehensive overview of UK road safety trends between 2000 and 2025. Through data cleaning, exploratory analysis, geospatial visualization, and predictive modelling, the project identifies key accident patterns and risk factors that can support evidence-based road safety interventions and future transport planning.
