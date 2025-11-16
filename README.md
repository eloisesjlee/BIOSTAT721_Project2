# BIOSTAT 721: Project2
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
├── data               # Contains raw CSV files for 2018, 2019, 2020
├── Project2.Rmd       # Main Rmarkdown file with codes
├── Project2.docx      # Knitted Word output
└── README.md          # This file
```
## Data Processing Function
The custom R function `processdata()` does the following to each of `AQ_2018.csv`, `AQ_2019.csv`, `AQ_2020.csv`:

- Rename pollutant variables (clean, short, readable names)
- Parses dates correctly
- Average multiple measurements per day
- Removes duplicate rows
- Identifies negative pollutant concentrations and sets them to zero
- Returns a clean, tidy data frame for each year

## Plots
The project produces two required plots:
### Plot 1: Monthly Average CO and O3 Concentration (2018-2020 Combined)
- X-axis: month
- Y-axis: pollutant concentration
- Displays monthly averages across all 3 years with 95% confidence interval error bars

### Plot 2: Monthly PM2.5 Concentration by Year
- X-axis: month
- Y-axis: PM2.5 concentration
- `geom_line()` chosen to best convey patterns over time

## Author
**Eloise Lee**  
Master of Biostatistics, Duke University  
BIOSTAT721 - Fall 2025
