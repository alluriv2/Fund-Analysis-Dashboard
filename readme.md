# Mutual Fund Dashboard and Portfolio Visualization

This repository contains two R-based projects for visualizing and analyzing mutual fund data:
	1.	Mutual Fund Dashboard: An interactive Shiny application for portfolio analysis, return calculations, and fund performance visualization.
	2.	Portfolio Visualization Treemap: A static visualization of portfolio holdings using treemaps to display hierarchical data distribution.

Contents
	1.	Mutual_Fund_Dashboard.Rmd
	•	An interactive dashboard built with Shiny and ShinyDashboard.
	•	Visualizes mutual fund data, calculates returns, and tracks NAV performance.
	2.	Portfolio_Visualisation.Rmd
	•	Generates treemaps to represent portfolio composition, sector allocation, and holding types.

Features

1. Mutual Fund Dashboard
	•	Portfolio Overview:
	•	Displays key fund information (e.g., total AUM, inception date).
	•	Visualizes holding type distribution and sector allocation.
	•	Returns Calculator:
	•	Calculates returns for Lumpsum and SIP investments.
	•	Allows dynamic input for investment amounts and durations.
	•	Fund Performance:
	•	NAV trends over time (1 month, 3 months, 1 year, etc.).
	•	NAV comparison across funds.
	•	Risk vs return analysis for portfolio performance.

2. Portfolio Visualization Treemap
	•	Treemap visualizes portfolio hierarchy:
	•	Categorizes by holding type, sector, and individual securities.
	•	Color-coded by holding type with proportional sizing based on portfolio weights.
	•	Displays 3-month returns and portfolio weight distributions.

Technologies Used
	•	R Programming: Core for data manipulation and visualization.
	•	Shiny & ShinyDashboard: For building interactive dashboards.
	•	Treemap & Treemapify: For creating hierarchical treemaps.
	•	ggplot2 & ggfittext: For enhanced static visualizations.
	•	dplyr & tidyr: For data wrangling and preprocessing.

Installation and Usage

1. Clone the Repository

git clone https://github.com/<alluriv2>/<Fund-Analysis-Dashboard>.git
cd <Fund-Analysis-Dashboard>

2. Install Required R Packages

install.packages(c("shiny", "shinydashboard", "ggplot2", "dplyr", "tidyr", "plotly", 
                   "treemap", "treemapify", "ggfittext"))

3. Running the Projects

Mutual Fund Dashboard
	1.	Ensure the required datasets are in the project directory:
	•	Historical_Closing_Prices.csv
	•	Motilal_Portfolio.csv
	2.	Run the app:

shiny::runApp("Mutual_Fund_Dashboard.Rmd")



Portfolio Visualization Treemap
	1.	Update the file path to Motilal_Portfolio.csv in the code if necessary.
	2.	Knit the RMarkdown file Portfolio_Visualisation.Rmd or run the relevant code chunks to generate the treemap.

Datasets
	1.	Historical_Closing_Prices.csv
	•	Contains historical NAV prices.
	•	Required for the dashboard.
	•	Expected columns:
	•	Date
	•	Motilal_Oswal_Flexi_Cap_Fund_Direct_Growth_NAV
	•	Union_Flexi_Cap_Fund_Direct_Growth_NAV.
	2.	Motilal_Portfolio.csv
	•	Contains portfolio composition details.
	•	Required for both the dashboard and treemap visualization.
	•	Expected columns:
	•	Holding.Type
	•	Sector
	•	Portfolio.Weight
	•	Return_3M.

How to Use
	1.	Launch the dashboard for interactive exploration of portfolio data and fund performance.
	2.	Generate treemaps for detailed visual insights into portfolio structure and allocation.

Contributors
	•	Vaibhav Alluri

Acknowledgments

Special thanks to Motilal Oswal and financial datasets for providing the foundation for analysis and visualization.
