# Analysis of Statistical Dependency of Distance from Fire Station on Fire Damage

## Overview
This project applies Simple Linear Regression (SLR) to analyze the relationship between the distance of a fire from the fire station and the corresponding damage in thousands of dollars. The analysis leverages data from Mendenhall & Sincich’s textbook *Statistics for Engineering and the Sciences* (2016) and uses the statistical language R for data analysis and visualization.

## File Descriptions
1. **project.Rmd**: Complete R Markdown file that I developed and used to generate the HTML files.
2. **project.bib**: BibTeX bibliographical database file to store my source citations.
3. **project.html**: HTML file generated from project.rmd that displays my project on a web browser in scrollable format.
4. **slidy_project.html**: HTML Slidy file generated from project.rmd that displays my project on a web browser in an accessible power point format.
5. **FIREDAM.csv**: Data set used for the analysis.

## Project Structure
The project is organized into several key sections:
1. **Introduction**: An explanation of the background and context of the study, including the significance of the research and the data used.
2. **Theoretical Basis of SLR**: Explanation of the simple linear regression model and its assumptions.
3. **Data Analysis**: Detailed application of SLR to the dataset, including model fitting and visualization.
   1. *Preliminary Exploration*: Scatter plots and correlation calculations.
   2. *Model Fitting*: Method of Least Squares to fit the SLR model.
   3. *Model Validation*: Residual analysis and checks for errors/assumptions.
   4. *Statistical Tests*: Hypothesis tests, confidence interals, and other potential biases.
4. **Conclusion**: Summary of findings and recommendations.

## Key Findings
- A strong positive correlation was found between fire damage and distance from the fire station, with a correlation coefficient of **0.96**.
- The regression model indicates that for each additional mile from the fire station, the estimated fire damage increases by **$4,919**.
- The model’s goodness-of-fit is validated with an **R-squared value of 0.923**, indicating that 92.3% of the variability in fire damage can be explained by the distance from the fire station.

## Getting Started
To simply view the project on your device, download either of the HTML files and view in your browser. To actually run the analysis in R and reproduce the results, follow these steps:

### Prerequisites
- **RStudio** installed on your local machine.
- Required R libraries:
  - `DT`
  - `s20x`
  - `ggplot2`
  - `rmarkdown`
  - `knitr`

### Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/fire-damage-analysis.git
2. Install necessary R packages if they are not already installed:
    ```bash
   install.packages(c("ggplot2", "DT", "s20x", "rmarkdown", "knitr"))
3. Knit the RmD into desired output format.
   ```bash
   rmarkdown::render("project.Rmd", output_format = "html_document", output_file = "project.html")
   rmarkdown::render("project.Rmd", output_format = "slidy_presentation", output_file = "slidy_project.html")
