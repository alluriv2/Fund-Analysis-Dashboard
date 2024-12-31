Motilal Oswal Portfolio Visualization

This project visualizes the Motilal Oswal Flexi Cap Fund Portfolio using treemap charts. The visualization helps to explore the portfolio composition by Holding Type, Sector, and Individual Securities.

Project Details
	•	Author: Vaibhav Alluri
	•	Date: November 25, 2024
	•	Tools Used: R, ggplot2, treemapify, dplyr, and tidyverse
	•	Output Formats: PDF, Word, HTML (via R Markdown)

Files in the Project

1. Project Script
	•	Portfolio_Visualisation.Rmd: The R Markdown file containing the analysis and visualization code.

2. Input Dataset
	•	Motilal_Portfolio.csv: The dataset containing information about the portfolio, including:
	•	Holding.Type: Type of the holding (e.g., Equity, Debt, etc.).
	•	Sector: The sector of each security (e.g., IT, Finance).
	•	Security: Name of the individual security.
	•	Portfolio.Weight: The weight of the security in the portfolio.
	•	Return_3M: 3-month return for the security.

3. Outputs
	•	Rendered document formats:
	•	Motilal_Portfolio.pdf
	•	Motilal_Portfolio.docx
	•	Motilal_Portfolio.html

How to Run

1. Prerequisites

Ensure the following R libraries are installed:

install.packages(c("dplyr", "ggplot2", "readr", "tidyverse", "treemap", "treemapify", "ggfittext"))

2. File Path

Set the file path to the Motilal_Portfolio.csv dataset in the R Markdown script:

file_path <- "/path/to/your/Motilal_Portfolio.csv"
data <- read.csv(file_path)

3. Render the Document
	•	Open the Portfolio_Visualisation.Rmd file in RStudio.
	•	Click Knit to render the report into the desired format (PDF, Word, or HTML).

Visualization Overview

The treemap chart in this project visualizes the portfolio structure based on:
	1.	Holding Type: Primary grouping of securities (e.g., Equity, Debt).
	2.	Sector: Sub-grouping by the industry or sector (e.g., IT, Finance).
	3.	Individual Securities: Drill-down to individual holdings.

Treemap Attributes:
	•	Size (vSize): Represents the weight of the security in the portfolio.
	•	Color (vColor): Represents the Holding Type of the securities.

Example Treemap Structure:

Holding Type
 ├── Sector 1
 │    ├── Security A
 │    ├── Security B
 ├── Sector 2
 │    ├── Security C
 │    ├── Security D

Key Functions Used

1. Data Preparation
	•	Column names are cleaned using make.names.
	•	Numerical values are converted using as.numeric.

2. Visualization
	•	The treemap function from the treemap library is used to create hierarchical treemaps.

Additional Notes
	•	Ensure the dataset is in CSV format and matches the column names expected in the script.
	•	For better font control in treemap labels, adjust the fontsize.labels and fontcolor.labels parameters.

Feel free to modify this README.md based on your specific project needs or additional features. Let me know if you need further help!# Portfolio-Visualisation
