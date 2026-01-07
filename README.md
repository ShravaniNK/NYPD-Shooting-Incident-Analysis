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

## Key Insights
The analysis reveals clear temporal patterns, geographic clustering, and demographic disparities in gun violence incidents—highlighting opportunities for targeted, evidence-based prevention strategies rather than one-size-fits-all approaches.
### These findings demonstrate how structured data analysis can support:
    Strategic allocation of community resources
    Timing and location of intervention programs
    Ongoing program evaluation and impact measurement

### Incidents occurrence Location


This chart shows clear seasonal spikes during summer months, suggesting opportunities for timed prevention and outreach efforts.  
## Statistical Modeling: Factors Associated with Fatal Shooting Outcomes
   ### Purpose: To explore whether timing of incidents and victim characteristics are associated with the likelihood that a shooting results in a fatal outcome. This analysis is intended to support population-level understanding and program planning, not individual-level prediction.
   ### Model Overview
      A logistic regression model was fitted using NYPD shooting incident data, with the outcome variable indicating whether an incident resulted in a fatality.
     Outcome Variable: STATISTICAL_MURDER_FLAG (Fatal vs. Non-fatal shooting)
     Predictor Variables:Time of day (grouped into intervals), Victim age group, Victim sex, Victim race
The model estimates associations, not causation, and results are interpreted in the context of public-interest and equity-focused analysis.

## Key Findings
   Time of day is significantly associated with fatal outcomes, with certain evening and early morning intervals showing higher odds of fatality compared to the reference period.
   Victim age group shows a strong association, with higher odds of fatal outcomes among older age groups relative to younger victims.
   Victim sex was not a statistically significant predictor in this model.
   Race variables were not statistically significant after accounting for other factors, underscoring the importance of interpreting disparities in the context of structural and environmental factors rather than individual characteristics.
