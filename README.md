# Household Carbon Footprint & Recycling Behaviour Analysis

This project presents a quantitative data analysis workflow in **R** using a household sustainability survey dataset.  
The analysis focuses on **data cleaning**, **exploratory data analysis (EDA)**, **regression modelling** for household carbon footprint, and **classification modelling** for recycling behaviour.

The project was completed as an academic data analysis assignment and demonstrates an end-to-end statistical workflow, from raw data preparation to model interpretation.

---

## Objectives

- Assess and improve the quality of the household sustainability dataset
- Explore patterns in household energy use, lifestyle choices, and environmental behaviour
- Build a model to explain variation in **carbon footprint**
- Build a model to predict whether a household **recycles regularly**
- Interpret results clearly and connect statistical findings to real-world sustainability behaviour

---

## Dataset Overview

The dataset contains household-level survey responses related to:

- Household size
- Annual energy consumption
- Recycling behaviour
- Public transport use
- Diet type
- Carbon footprint
- Environmental concern score
- Income
- Number of adults
- Home type

Two target variables were analysed:

1. **carbon_footprint** — continuous outcome  
2. **recycles_regularly** — binary outcome

---

## Tools & Technologies

- **Language:** R
- **Environment:** RStudio
- **Libraries:** tidyverse, ggplot2, dplyr, readr, broom, car, MASS, caret *(edit this list to match your actual packages)*
- **Workflow:** Data cleaning, EDA, regression modelling, model diagnostics, interpretation
- **Reporting:** R Markdown

---

## Key Analysis Areas

- Data quality assessment
- Missing values and invalid entries
- Category standardisation
- Exploratory analysis of household and behavioural variables
- Carbon footprint modelling
- Recycling likelihood modelling
- Model diagnostics and interpretation

---

## Project Workflow

### 1. Data Preparation & Cleaning
- Loaded the `.Rda` dataset in R
- Checked variable types, missing values, and invalid records
- Identified data quality issues such as:
  - missing values
  - inconsistent categorical labels
  - invalid numerical values
- Cleaned the dataset using transparent and reproducible R code

### 2. Exploratory Data Analysis (EDA)
- Explored distributions of key variables
- Examined relationships between explanatory variables and both target variables
- Used plots, summary statistics, and tabular analysis to identify informative patterns
- Selected the most useful findings to support later modelling decisions

### 3. Modelling Carbon Footprint
- Built an initial regression model for **carbon_footprint**
- Compared candidate explanatory variables based on EDA and model fit
- Refined the model using diagnostics and model selection
- Interpreted coefficients and assessed weaknesses such as multicollinearity, non-linearity, and residual behaviour

### 4. Modelling Recycling Behaviour
- Built a classification model for **recycles_regularly**
- Used a binary modelling approach suitable for a yes/no target
- Selected predictors based on behavioural and household characteristics
- Evaluated the proposed model and interpreted the main effects on recycling likelihood

---

## Models Used

### Regression Model
Used to analyse the continuous target:

- **Multiple Linear Regression** for `carbon_footprint`

### Classification Model
Used to analyse the binary target:

- **Logistic Regression** for `recycles_regularly`

> Replace this section if you also used alternative models during testing, such as stepwise regression or interaction models.

---

## Example Insights

Some of the analysis focused on how carbon footprint and recycling behaviour may vary with:

- annual energy consumption
- household size
- household income
- environmental concern score
- home type
- use of public transport
- diet type

> Add 3–5 bullet points here with your actual findings from your final project.

Example format:
- Higher annual energy consumption was associated with higher household carbon footprint.
- Environmental concern appeared to be positively associated with regular recycling.
- Some household or property types showed different recycling patterns.

---

## Project Structure

```bash
Household-Carbon-Footprint-Analysis/
┣ data/
┃ ┗ carbon-footprint.Rda
┣ scripts/
┃ ┗ analysis.R            # optional if you have a standalone script
┣ reports/
┃ ┣ submission.Rmd
┃ ┗ supporting.Rmd
┣ outputs/
┃ ┣ plots/
┃ ┗ tables/
┣ README.md
