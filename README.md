## Project Overview
   This project analyzes publicly available NYPD Shooting Incident Data to identify temporal, geographic, and demographic patterns in gun violence. 
   The project emphasizes data quality, reproducibility, and clear communication, recognizing the sensitive and community-centered nature of violence prevention work.

## Objectives
  Analyze gun violence trends over time to identify periods of elevated risk
  Identify geographic concentrations of shootings to support targeted prevention efforts
  Examine demographic and situational patterns to inform community-centered interventions
  Translate analytical findings into clear, actionable insights for non-technical stakeholders
  Demonstrate an end-to-end analytical workflow suitable for nonprofit program evaluation

## Dataset
Source: NYPD Shooting Incident Data (Open Data NYC)
### Content Includes:
    Date and time of shooting
    Location (borough, precinct, latitude/longitude)
    Victim demographics (age group, sex, race)
    Injury or fatality outcome
All data cleaning and transformations were performed to ensure accuracy, consistency, and reproducibility.

## Methods & Tools:
### Data Cleaning & Validation:
    Handled missing values, standardized date/time fields, validated geographic fields

### Exploratory Data Analysis (EDA):
    Trend analysis, distribution analysis, and comparative breakdowns

### Visualization:
    ggplot2 for clear, publication-ready charts    

### Reproducibility:
    Modular R scripts with documented steps and assumptions

### Key Insights
The analysis reveals clear temporal patterns, geographic clustering, and demographic disparities in gun violence incidents, highlighting opportunities for targeted, evidence-based prevention strategies rather than one-size-fits-all approaches.
   #### These findings demonstrate how structured data analysis can support:
        Strategic allocation of community resources
        Timing and location of intervention programs
        Ongoing program evaluation and impact measurement

### Key Visual Findings
#### 1. Incidents Occurrence Location
![Incidents_Occurrence_Location](https://github.com/ShravaniNK/NYPD-Shooting-Incident-Analysis/blob/b123a15247e54ab204515308e552543aa74f8edb/1.Incident_Occurrence_Barplot.PNG)
      Analysis: From the above plot, most of the incidents took place in Brooklyn and Bronx compared to other 3 places. Also the ratio of males victims is higher than female victims.

#### 2. Victims Age Group
![Victims_Age_Group](https://github.com/ShravaniNK/NYPD-Shooting-Incident-Analysis/blob/dbdb8945c5083cb620f8a89adce1b4be8cd495ce/2.Victims_By_AgeGroup.PNG)
   Analysis: From the above plot, most of the victims are in the age group of 18-45, due to the fact that they are the most active and independent age group to stay out and engage in various activities.Also most of the victims are males.

#### 3.Victims By Race
![Victims_By_Race](https://github.com/ShravaniNK/NYPD-Shooting-Incident-Analysis/blob/dbdb8945c5083cb620f8a89adce1b4be8cd495ce/3.Victims_By_Race.PNG)
   Analysis: From the above plot, we can say that black people are the highest victims, followed by whitehispanic and black hispanic. Racial disparity existence is evident from the plot.

#### 4. Victims By Gender
![Victims_By_Gender](https://github.com/ShravaniNK/NYPD-Shooting-Incident-Analysis/blob/dbdb8945c5083cb620f8a89adce1b4be8cd495ce/4.Victims_By_Gender.PNG)
   Analysis: From the above plot,it is clear that males are the most targetted victims and among them are black race males.Even among the females, even though they are less than males the ratio of black females is high suggesting them as the targetted race.

#### 5. Yearwise Shootings
![Yearwise_Shootings](https://github.com/ShravaniNK/NYPD-Shooting-Incident-Analysis/blob/dbdb8945c5083cb620f8a89adce1b4be8cd495ce/5.Yearwise_Shootings_Barplot.PNG)
   Analysis: From the above plot,we can see that the number of cases declined between 2017-2019, and again increased during covid pandemic.

#### 6. Time Of Incident Occurrence
![Time_Of_Occurrence](https://github.com/ShravaniNK/NYPD-Shooting-Incident-Analysis/blob/e448adc70bbf0faa0409e08f58e2a0365a1a6a69/6.Time_Of_Occurrece.PNG)
   Analysis: 75% of the incidents mostly occured after dark.

## Statistical Modeling: Factors Associated with Fatal Shooting Outcomes
   ### Purpose: 
       To explore whether timing of incidents and victim characteristics are associated with the likelihood that a shooting results in a fatal outcome. This analysis is intended to support population-level understanding and program planning, not individual-level prediction.
   
   ### Model Overview
       A logistic regression model was fitted using NYPD shooting incident data, with the outcome variable indicating whether an incident resulted in a fatality.
       Outcome Variable: 
        STATISTICAL_MURDER_FLAG (Fatal vs. Non-fatal shooting)
       Predictor Variables:
        Time of day (grouped into intervals), 
        Victim age group, 
        Victim sex, 
        Victim race
   
   ### Insights
        Time of day is significantly associated with fatal outcomes, with certain evening and early morning intervals showing higher odds of fatality compared to the reference period.
        Victim age group shows a strong association, with higher odds of fatal outcomes among older age groups relative to younger victims.
        Victim sex was not a statistically significant predictor in this model.
        Race variables were not statistically significant after accounting for other factors, underscoring the importance of interpreting disparities in the context of structural and environmental factors rather than individual characteristics.

## Final Conclusions & Bias Identifications
    From the data we have,it can be concluded that the black males within the age group of 18-45 are mojority of the victims of shooting in the areas of New York. Most of the incidents took place at Brooklyn and Bronx and between 8PM-4AM. 
    It is unclear whether the victims are visitors or residents of Newyork.Also, there is no motive of the incident reported  which can be very useful in reducing the number of incidents in future. 
    To have a more clear understanding about the magnitude of gun violence, the given data which has lots of missing entries that can introduce bias should be filled.
    Appropriate measures such as increased patrol, awareness of gun violence  should be taken to reduce the number of race related shootings. 


