
# Mutual Fund Dashboard and Portfolio Visualization

This repository contains two R-based projects for visualizing and analyzing mutual fund data:

1. **Mutual Fund Dashboard**: An interactive Shiny application for portfolio analysis, return calculations, and fund performance visualization.
2. **Portfolio Visualization Treemap**: A static visualization of portfolio holdings using treemaps to display hierarchical data distribution.

## Contents

1. **Mutual_Fund_Dashboard.Rmd**
   - An interactive dashboard built with Shiny and ShinyDashboard.
   - Visualizes mutual fund data, calculates returns, and tracks NAV performance.
   
2. **Portfolio_Visualisation.Rmd**
   - Generates treemaps to represent portfolio composition, sector allocation, and holding types.

## Features

### 1. Mutual Fund Dashboard
- **Portfolio Overview**:
   - Displays key fund information (e.g., total AUM, inception date).
   - Visualizes holding type distribution and sector allocation.
  
- **Returns Calculator**:
   - Calculates returns for Lumpsum and SIP investments.
   - Allows dynamic input for investment amounts and durations.
  
- **Fund Performance**:
   - NAV trends over time (1 month, 3 months, 1 year, etc.).
   - NAV comparison across funds.
   - Risk vs return analysis for portfolio performance.

### 2. Portfolio Visualization Treemap
- Treemap visualizes portfolio hierarchy:
   - Categorizes by holding type, sector, and individual securities.
   - Color-coded by holding type with proportional sizing based on portfolio weights.
   - Displays 3-month returns and portfolio weight distributions.

## Technologies Used
- **R Programming**: Core for data manipulation and visualization.
- **Shiny & ShinyDashboard**: For building interactive dashboards.
- **Treemap & Treemapify**: For creating hierarchical treemaps.
- **ggplot2 & ggfittext**: For enhanced static visualizations.
- **dplyr & tidyr**: For data wrangling and preprocessing.

## Installation and Usage

### 1. Clone the Repository
Clone the repository to your local machine:
```bash
git clone https://github.com/alluriv2/Fund-Analysis-Dashboard.git
cd Fund-Analysis-Dashboard
```

### 2. Install Required R Packages
Make sure you have the necessary R packages installed by running the following command in your R console:
```r
install.packages(c("shiny", "shinydashboard", "ggplot2", "dplyr", "tidyr", "plotly", 
                   "treemap", "treemapify", "ggfittext"))
```

### 3. Running the Projects

#### Mutual Fund Dashboard
1. Ensure the following required datasets are in the project directory:
   - `Historical_Closing_Prices.csv`: Contains historical NAV prices (required for the dashboard).
   - `Motilal_Portfolio.csv`: Contains portfolio composition details (required for both the dashboard and treemap).

2. Launch the dashboard using the following command in R:
```r
shiny::runApp("Mutual_Fund_Dashboard.Rmd")
```

#### Portfolio Visualization Treemap
1. Make sure to update the file path for `Motilal_Portfolio.csv` in the code if necessary.

2. Knit the `Portfolio_Visualisation.Rmd` file in RStudio or run the relevant code chunks to generate the treemap.

   - To knit the file:
     - Open the file `Portfolio_Visualisation.Rmd` in RStudio.
     - Click the "Knit" button in RStudio to generate the treemap.

### 4. Datasets

- **`Historical_Closing_Prices.csv`**
   - Contains historical NAV prices for mutual funds.
   - Expected columns:
     - `Date`
     - `Motilal_Oswal_Flexi_Cap_Fund_Direct_Growth_NAV`
     - `Union_Flexi_Cap_Fund_Direct_Growth_NAV`

- **`Motilal_Portfolio.csv`**
   - Contains portfolio composition details.
   - Expected columns:
     - `Holding.Type`
     - `Sector`
     - `Portfolio.Weight`
     - `Return_3M`

### 5. How to Use

- **Mutual Fund Dashboard**: 
   - Launch the dashboard for interactive exploration of portfolio data and fund performance.
   - Visualize portfolio performance and track NAV trends over time.
   - Calculate returns for different investment types (Lumpsum and SIP).
   
- **Portfolio Visualization Treemap**: 
   - Generate the treemaps to visualize portfolio structure, holding types, sector allocation, and returns.
   - The treemaps provide detailed insights into portfolio composition, categorized by holding type, sector, and individual securities.

## Contributors
- Vaibhav Alluri

## Acknowledgments

Special thanks to Motilal Oswal and financial datasets for providing the foundation for analysis and visualization.

