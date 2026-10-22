DATA 606 Final Project

## NYCHA Electricity Consumption and Cost

This project analyzes electricity consumption and electricity costs among New York City Housing Authority (NYCHA) developments.

The analysis compares electricity records across the five New York City boroughs:

- Bronx
- Brooklyn
- Manhattan
- Queens
- Staten Island

## Research Question

How is electricity consumption associated with electricity cost among NYCHA housing developments in New York City, and how does this relationship vary across boroughs?

## Dataset

The dataset contains monthly electricity billing records for NYCHA developments.

The main variables include:

- Development name
- Borough
- Revenue month
- Electricity consumption
- Current electricity charges
- KWH charges

Electricity consumption is reported in kilowatt-hours in the original dataset and converted to megawatt-hours (MWh) for visualization.

Electricity costs are reported in U.S. dollars (USD).

## Data Source

The data were obtained from NYC Open Data.

**Dataset:** Electric Consumption and Cost  
**Publisher:** New York City Housing Authority  
**Source:** [NYC Open Data — Electric Consumption and Cost](https://data.cityofnewyork.us/d/jr24-e7cr)

## Methods

The project uses R and Quarto to:

- Import the original CSV file.
- Clean and prepare the variables.
- Convert electricity and cost fields to numeric values.
- Remove invalid or missing records when necessary.
- Calculate summary statistics.
- Compare electricity consumption and cost by borough.
- Create scatter plots and boxplots.
- Display electricity consumption in MWh.
- Display electricity cost in USD.

## Files

- `DATA606-Final-Project.qmd` — Quarto source file.
- `DATA606-Final-Project.html` — Rendered HTML report.
- `Data/` — Dataset folder.
- `Data/Electric_Consumption_And_Cost_(2010_-_Sep_2025)_20261018.csv` — Original dataset.
- `DATA 606 Data Project Proposal.pdf` — Proposal document.

## Published Report

The published proposal is available on RPubs:

[View the DATA 606 NYCHA Electricity Project](https://rpubs.com/howtwo3/data606-nycha-electricity-project)

## How to Run the Project

Open the project folder in RStudio and render the Quarto document:

```r
quarto::quarto_render("DATA606-Final-Project.qmd")
```

The required R packages are:

```r
install.packages(c(
  "readr",
  "dplyr",
  "tidyr",
  "ggplot2",
  "knitr",
  "scales"
))
```

## Study Type

This is an observational study. The researcher did not assign electricity consumption, costs, boroughs, or billing periods.

The results describe the observed NYCHA records and do not establish causation.

## Limitations

The analysis does not include all factors that may affect electricity consumption and cost, such as:

- Building size
- Occupancy
- Weather
- Utility rate changes
- Building efficiency
- Type of equipment
- Billing adjustments

Therefore, the findings cannot be generalized to every building in New York City.

## AI Use

ChatGPT was used to help interpret the assignment requirements, organize the project, improve the English writing, and review the R code.

The data preparation, calculations, tables, visualizations, and conclusions were reviewed by the author.

## Author

Patricio Romero

DATA 606
