# DATA 606 Final Project

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

Dataset: Electric Consumption and Cost  
Publisher: New York City Housing Authority

Source:

https://data.cityofnewyork.us/d/jr24-e7cr

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

## How to Run the Project

Open the project folder in RStudio and render the Quarto document:

```r
quarto::quarto_render("DATA606-Final-Project.qmd")
