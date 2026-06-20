#  UK Road Safety Analysis (2000–2025)

## Project Overview

This project analyzes the UK Department for Transport (DfT) STATS19 Road Safety dataset from 2000–2025 to identify:

* Long-term collision trends
* Accident hotspots
* Environmental risk factors
* Casualty demographics
* Vehicle involvement patterns
* Predictors of accident severity

## Business Questions

### Trend Analysis

* Are road collisions increasing or decreasing?
* Which years recorded the highest casualties?
* Are there seasonal patterns in accidents?

### Geographic Analysis

* Which local authorities experience the highest collision rates?
* How do urban and rural accident patterns compare?
* Where are accident hotspots located?

### Risk Analysis

* Which weather conditions contribute most to accidents?
* Which road surfaces are associated with higher risk?
* How do day and night accidents compare?

### Casualty Analysis

* Which age groups are most affected?
* Who suffers the most casualties (drivers, passengers, pedestrians)?
* What is the distribution of injury severity?

### Vehicle Analysis

* Which vehicle types are most involved in collisions?
* How do motorcycles compare with cars?
* What role do commercial vehicles play?


## Dataset

Source: UK Department for Transport (DfT) STATS19 Dataset

### Datasets Used

| Dataset    | Description                        |
| ---------- | ---------------------------------- |
| Collisions | Accident-level information         |
| Casualties | Casualty demographics and severity |
| Vehicles   | Vehicle and driver information     |


## Data Preparation

### Data Cleaning

* Filtered records between 2000–2025
* Removed invalid observations
* Converted coded variables into descriptive labels
* Standardized date and time fields
* Investigated missing values

### Feature Engineering

Created additional features:

* Month
* Month Number
* Hour
* Day/Night Classification
* Age Bands

## Exploratory Data Analysis

### Collision Trends

**Key Findings**

* Collision volumes generally declined across the study period.
* Certain years experienced significantly higher casualty counts.
* Monthly accident patterns suggest seasonal effects.

  * <img width="451" height="240" alt="image" src="https://github.com/user-attachments/assets/11dab00a-e6d2-4b87-a8dd-5141be53162b" />
*

* <img width="451" height="253" alt="image" src="https://github.com/user-attachments/assets/eae08668-be07-49ab-ad51-87812f7a569b" /> *


### Geographic Analysis

**Key Findings**

* Birmingham and Kent recorded some of the highest collision volumes.
* Urban areas accounted for the majority of accidents.
* Accident hotspots were concentrated around major population centres.

  *<img width="451" height="289" alt="image" src="https://github.com/user-attachments/assets/b3cfb113-0bd4-4935-9254-da25eee7944d" />*

*<img width="451" height="510" alt="image" src="https://github.com/user-attachments/assets/9ea2560f-b826-46f8-9a2b-e78e1a1e92b3" />*


### Risk Factors

**Weather Conditions**

* Most collisions occurred during fine weather conditions.
* Exposure effects likely explain the result.

**Road Surface Conditions**

* Dry roads accounted for the highest collision volumes.
* Wet and icy roads showed elevated risk profiles.

**Day vs Night**

* More accidents occurred during daytime hours.
* Night-time accidents may be associated with greater severity.

*<img width="451" height="209" alt="image" src="https://github.com/user-attachments/assets/be2da938-651b-4f3f-88e4-fe812151e005" />*

*<img width="451" height="337" alt="image" src="https://github.com/user-attachments/assets/6a2d3901-a45a-477b-8de2-52d8f5915b1d" />*


### Casualty Analysis

**Key Findings**

* Individuals aged 26–40 represented the largest casualty group.
* Drivers recorded the highest casualty counts.
* Slight injuries dominated casualty outcomes.

*<img width="451" height="397" alt="image" src="https://github.com/user-attachments/assets/e1f79abc-dab1-4111-be68-5aa2a8fce12f" />*

*<img width="402" height="411" alt="image" src="https://github.com/user-attachments/assets/105b85d4-789f-4c19-866b-e51be9878aed" />*

### Vehicle Analysis

**Key Findings**

* Cars were involved in the majority of collisions.
* Motorcyclists remain a vulnerable road-user group.
* Commercial vehicles contributed to a smaller share of incidents.

*<img width="451" height="190" alt="image" src="https://github.com/user-attachments/assets/50014aec-8428-4853-99c5-d1c196bfc3e7" />*


## 🤖 Predictive Modelling

### Model 1: Collision Severity Prediction

**Target Variable**

* Collision Severity

**Algorithm**

* Random Forest Classifier

**Features**

* Weather Conditions
* Road Surface Conditions
* Road Type
* Junction Control
* Number of Vehicles
* Number of Casualties
* Time Variables


### Model 2: Casualty Severity Prediction

**Target Variable**

* Casualty Severity

**Algorithm**

* Random Forest Classifier

**Features**

* Age
* Gender
* Casualty Class
* Casualty Type


### Model 3: Number of Casualties Prediction

**Target Variable**

* Number of Casualties

**Algorithm**

* Random Forest Regressor

**Features**

* Environmental Conditions
* Road Characteristics
* Vehicle Counts


## 🔍 Key Insights

* Road collisions have generally declined over time.
* Urban areas experience the highest accident volumes.
* Birmingham and Kent emerged as major collision hotspots.
* Weather and road surface conditions influence accident risk.
* Adults aged 26–40 represent the most affected casualty group.
* Drivers account for the largest share of casualties.
* Cars dominate collision involvement.
* Machine learning models can help predict accident severity and casualty outcomes.
  

## 💡 Recommendations

### Road Safety

* Increase enforcement in hotspot locations.
* Target high-risk periods with focused interventions.

### Infrastructure

* Improve road surface maintenance.
* Expand lighting coverage in high-risk areas.

### Public Awareness

* Focus campaigns on high-risk age groups.
* Increase motorcycle safety initiatives.

### Future Work

* Incorporate traffic volume data.
* Use weather history datasets.
* Compare Random Forest with XGBoost and LightGBM.
* Build an interactive road safety dashboard.
* Expand on 2025 data(full data yet to be released).


## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Folium
* Scikit-Learn
* XGBoost

## Author

Hilton Oladipupo

Data Analytics | Machine Learning
