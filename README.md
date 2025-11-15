# BIOSTAT721_Project2Project 2
This respository contains all code, data, and documentation for Project 2 in BIOSTAT 721: Statistical Programming in R. It explores the association between various air pollutants and sickle cell disease (SCD) in Durham County, North Carolina, using EPA pollutant data and health system utilization data. 

## Project Overview
Sickle cell disease (SCD) is characterized by misshapen red blood cells that can obstruct blood flow, leading to pain, infection, anemia, and stroke. There is some evidence that exposure to air pollution aggravates vaso-occlusion and pain in SCD patients.

This project analyzes daily air pollutant measurements from EPA air monitors at RDU Airtport (2018-2020) and prepares the exposure data for exploratory analysis. 

The final output includes:

- A custom R function `processdata()` to clean and process the pollutant data
- Two exploratory plots summarizing pollutant concentration patterns over time
- A well-documented R Markdown report knitted to a Word document

## Repository Structure
```{r}
BIOSTAT721_Project2/
├── data/                # Raw CSV files for 2018, 2019, 2020
├── scripts/             # R scripts (functions, code for plot)
├── Project2_Report.Rmd  # Main report (final submission)
├── Project2_Report.docx # Knitted Word output
└── README.md            # This file
```
## Data Processing Function

