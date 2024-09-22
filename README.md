# Tourism Migration Forecasting to Greece

## Overview
This project focuses on predicting the number of tourists migrating to Greece from 2007 to 2016 using time series analysis and forecasting techniques. The goal is to provide insights into seasonal trends and assist stakeholders in planning for tourism-related activities.

## Technologies Used
- R
- Libraries: `forecast`, `fpp3`, `ggplot2`, `dplyr`, `lubridate`, `tsibble`, etc.

## Dataset
The dataset contains monthly records of tourists visiting Greece over a specified period. It includes:
- **Nombre**: The number of tourists per month.

## Project Structure
- `data/`: Directory containing the dataset (`Book1.xlsx`).
- `scripts/`: R scripts for data analysis and forecasting.
- `results/`: Visualizations and output of the forecasting models.

## Installation
1. Ensure R and RStudio are installed on your machine.
2. Install the necessary R packages using the following command:
   ```R
   install.packages(c("readxl", "fpp3", "forecast", "ggplot2", "dplyr", "lubridate", "tsibble"))
## Usage

1. **Load the data and create a time series object:**
   ```R
   library(readxl)
   library(fpp3)

   # Load data
   data <- read_excel("data/Book1.xlsx")
   ts_data <- ts(data$Nombre, start = c(2007, 1), frequency = 12)
#Conclusion
This project demonstrates the application of time series analysis to forecast tourism trends, providing valuable insights for decision-making in the tourism sector.
