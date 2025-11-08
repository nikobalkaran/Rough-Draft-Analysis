# Rough-Draft-Analysis
An exploration of commercial and residential property values in Norwalk, CT.
This repository contains data, analytical code, and findings that may support portions of an as-yet-unpublished capstone article for my Master's degree. That article will contain important context and details.

## Data
This analysis uses a compilation of the Net Grand List by Town 2011 to 2024 spreadsheet by the Intergovernmental Policy and Planning found on Connecticut Open Data.

The spreadsheets come from the following sources:

- Name of source:
  - 'Net_Grand_List_by_Town,_2011-2024_20251029.csv': Raw data of the Grand List.

Each of the spreadsheets contains the following columns relevant to the analysis:

- 'GL Year' — The month and year that the data for the list was released.
- 'Town Name' — The towns in Connecticut.
- 'Commercial YoY' - The year-over-year percent for commercial property values.
- 'Residential YoY' - The year-over-year percent for residential property values.
- 

## Methodology

#### Part 1: Cleaning

-Since the original Grand List had all the towns in CT, I decided to separate only Norwalk.
-Upon further examination in Jupyter, I decided to include two other towns to compare to Norwalk: Bridgeport and Stamford.
- Downloaded that new spreadsheet to add to the data folder to analyze in Jupyter Notebook.

The notebook norwalk-office-vacancy.ipynb performs the following analyses:

#### Part 2: More Cleaning and Analysis

- Changed data type of the GL Year column to datetime64.
- Renamed some of the columns to make it easier to work with.
- Removed white space from one of the columns.
- Changed the data types of the Residential, Commercial and Total Grand List columns.
- Calculated year-over-year residential property %.
- Calculated year-over-year commercial property %.
- Calculated how much of the city's total tax base is made up of commercial property value.
- Plotted commercial property year-over-year.
- Plotted residential property year-over-year.


## Outputs

The results from above are saved as: output/norwalk_analysis.csv.

## Running the analysis yourself

You can run the analysis yourself. To do so, you'll need the following installed on your computer:

- Python 3
- The Python libraries specified in requirements.txt

## Licensing

All code in this repository is available under the MIT License. The data file in the output/ directory is available under the Creative Commons Attribution 4.0 International (CC BY 4.0) license. All files in the data/ directory are released into the public domain.

## Feedback / Questions?

Contact Niko Balkaran at niko.balkaran40@journalism.cuny.edu
