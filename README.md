```markdown
# Human Development Indicators Analysis

This repository contains a comprehensive analysis of Human Development Indicators (HDI) for Singapore and Switzerland. The project demonstrates data loading, cleaning, and visualization techniques using the `data.table` package in R, along with the creation of an R package (`HDIAnalysis`) for managing HDI data.

## Project Overview

The project involves the following key steps:
- **Introduction**: Explanation of the Human Development Indicators dataset and its components.
- **Data Preparation**: Loading, cleaning, and merging datasets for Singapore and Switzerland.
- **Data Analysis**: Exploratory data analysis and visualization of key indicators such as Life Expectancy, Education Index, and Carbon Dioxide Emissions.
- **R Package**: Development of an R package (`HDIAnalysis`) to facilitate easy manipulation and analysis of HDI data.

## Getting Started

### Prerequisites

- R (version 4.0 or higher)
- Required R packages: `data.table`, `ggplot2`

### Installation

1. **Clone the repository:**

   ```sh
   git clone https://github.com/your-username/HDI-Analysis.git
   cd HDI-Analysis
   ```

2. **Install the required R packages:**

   ```r
   install.packages(c("data.table", "ggplot2"))
   ```

3. **Install the `HDIAnalysis` package:**

   Navigate to the directory containing the `HDIAnalysis` package and install it using:

   ```r
   devtools::install(".")
   ```

## Data

The datasets used in this project are:
- [HDI Data for Singapore](https://data.humdata.org/dataset/hdro-data-for-singapore)
- [HDI Data for Switzerland](https://data.humdata.org/dataset/hdro-data-for-switzerland)

### File Structure

- `data/`: Contains the HDI CSV files.
- `scripts/`: Contains R scripts for data processing and analysis.
- `vignettes/`: Contains the R package vignettes.
- `HDIAnalysis/`: Contains the R package source code.

## Usage

### Data Analysis

To perform the analysis, run the scripts located in the `scripts/` directory. These scripts will:

1. Load the HDI datasets.
2. Clean and preprocess the data.
3. Merge datasets and perform exploratory data analysis.
4. Generate visualizations of key indicators.

### HDIAnalysis Package

The `HDIAnalysis` package provides functions to:

- **Read HDI Data**: `readHDI(filename)` - Reads and preprocesses HDI data from a CSV file.
- **Print HDI Data**: `print.hdi_data(x)` - Prints summary information of the HDI data.
- **Summarize HDI Data**: `summary.hdi_data(object)` - Provides summary statistics for the HDI data.
- **Plot HDI Data**: `plot.hdi_data(data)` - Creates plots of HDI data over time.

### Example

```r
library(HDIAnalysis)

# Read HDI data for Singapore
singapore_data <- readHDI("data/hdro_indicators_sgp.csv")

# Print summary of the data
print(singapore_data)

# Generate a summary of the data
summary(singapore_data)

# Plot the HDI data
plot(singapore_data)
```
- Replace `https://github.com/your-username/HDI-Analysis.git` with your actual GitHub repository URL.
- Adjust the contact information and any other specific details as needed.
