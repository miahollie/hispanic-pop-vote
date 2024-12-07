# Analysis of Hispanic/Latino population changes in NJ

This repository contains data, analytic code, and findings that support portions of an article that looks at population changes in New Jersey and how that may have impacted the most recent election, if at all. 

## Data

This analysis uses five spreadsheets.

The spreadsheets come from the following sources:

Census Bureau:
- 2019_acs_nj.csv: cleaned data of the 2019 1-year American Community Survey, filtered for all New Jersey counties.
- 2023_acs_nj.csv: cleaned data of the 2023 1-year American Community Survey, filtered for all New Jersey counties. 
- 2019_acs_us.csv: cleaned data of the 2019 1-year American Community Survey.
- 2023_acs_us.csv: cleaned data of the 2023 1-year American Community Survey. 

Various county boards of elections. Find a full list to their websites here: https://www.nj.gov/state/elections/election-night-results.shtml
- votes_2024.xlsx: cleaned data from various county boards of elections in New Jersey.

Each of the spreadsheets contain, among others, the following columns relevant to the analysis:

- label: county name
- Total population: total number population in the county at the time of the census survey
- Hispanic or Latino (of any race): total number Hispanic or Latino population in the county at the time of the census survey
- Not Hispanic or Latino: total number non-Hispanic or non-Latino population in the county at the time of the census survey
- total_votes: total number of casted votes in the county for the 2024 general election.
- d_votes: total number of casted votes in the county for the Democratic presidential candidate during 2024 general election.
- r_votes: total number of casted votes in the county for the Republican presidential candidate during 2024 general election.

## Methodology

The notebook hispanic-voter-analysis.ipynb performs the following analyses:

#### Part 1: Imports
imports initial sets of datasets and libraries

#### Part 2: Merge Dataframes
Marges dataframes

#### Part 3: Analyze population changes
For each year, finds the percentage of each county's population that is Hispanic/Latino and non-Hispanic/Latino. Does the same for the U.S.-specific data. Then, uses the percent change formula to find how much these populations have changed since the first reporting year (2019).

#### Step 4: Analyze voter data
Analyzes the voter data to figure out who won in each county and by how much. Finds the percentage of votes that went to each major-party candidate, then finds the difference between those percentages.

#### Step 5: Linear Regression
Performs a linear regression and plots it. 

## Running the analysis yourself

You can run the analysis yourself. To do so, you'll need the following installed on your computer:

Python 3 and some of its libraries, including: pandas, statsmodels.api and matplotlib 

## Licensing

All code in this repository is available under the MIT License. The data file in the output/ directory is available under the Creative Commons Attribution 4.0 International (CC BY 4.0) license. All files in the data/ directory are released into the public domain.

## Feedback / Questions?

Contact YOUR NAME HERE at mia.hollie48@journalism.cuny.edu.
