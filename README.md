# MiltonZouKhalsa__ENV872_EDA_FinalProject

This repository serves as space to develop the final class project required by ENV872 (Environmental Data Analytics) at Duke University.

## Summary

This repository acts as a hub for the project group members to store data and remain coordinated as each member contributes to the goals set forth for the project.  It contains multiple data folders holding processed, raw, and spatial data.  It is also home to the project RMD file containing the bulk of the code written to process our data.  We are using COVID-19 data from 2020 to 2022 collected from the U.S. Census Bureau and the New York Department of Health. Additionally, we are using the state map file that was incorporated in class for ENV872.  The repository also contains the .Rproj project file, .gitignore file, .Rhistory file, license file, and this readme file.

We plan on answering the central question: how well does the population of a county correlate with the occurrence of COVID-19 in New York State?  We will do this by examining three relationships.  First, we will assess the strength of correlation between the predictor variables: population density and the response variable: number of COVID-19 cases across New York State.  Second, we will determine explore the relationship between the variables: density, absolute population,
and settlement types and the response variable: cumulative COVID-19 cases?.  Third, we will answer the question,"What is the correlation between absolute population and population density 
and the number of COVID-19 tests does done? Does the stronger correlated 
relationship vary among settlement types?"

## Investigators

Group Members:
Danlei Zou, GuruBandaa Khalsa, & Sashoy Milton

Contact Information:
gurubandaa.khalsa@duke.edu
sashoy.milton@duke.edu
danlei.zou@duke.edu

Affiliations: Duke University Nicholas School of the Environment

Data Information:
https://www.census.gov/library/stories/state-by-state/new-york-population-change-between-census-decade.html
COVID-19 Variant Data | Department of Health (ny.gov) – (March 1, 2020,  to November 22, 2022)
cb_2018_us_county_20m.shp state FIPS code 36

## Keywords

ENV872, COVID-19, COVID, virus, virus spread, New York, New York State

## Database Information

We acquired our 2020 to 2022 COVID-19 data from the New York Department of Health and population data from the U.S. Census Bureau on November 24th, 2022.  County names did not match between the census data and NY Department of Health data.  We wrangled our data by removing the word "county" from each county in the census data.  In addition to the 62 counties, the NY Health Department broke counties down into smaller sections resulting in more than 62 counties.  Since we only want to work with the original counties, we left-merged the NY health data onto the county data on November 24th, 2022.  We are using the merged version as our main data source.  Additionally on November 24th, 2022, we uploaded the state map file that was incorporated in class for ENV872.  Lastly, we added spatial files and updated the data types and variable types for the combined dataset on November 27th, 2022.

## Folder structure, file formats, and naming conventions 

Our main project folder is named "MiltonZouKhalsa__ENV872_EDA_FinalProject."  Within the folder are the  .gitignore file, .Rhistory file, Data folder, project RMD file named "EDA_Final_Group_Project.RMD", LICENSE file, .Rproj project file named the same as the main project folder, and this README.md file.  We organized our data files within multiple data folders, including "processed, raw, meta-data, and spatial data.These folders are titled, "Processed_Data", "Raw_Data", "Meta_Data" and "Spatial_Files."  The processed,meta-data,raw data folders contain .csv files  The spatial data folder contains a Shapefile.URL file, .cpg file, .dbf file, .prj file, a few .shp files, and a .shx file.  These allow for spatial processing to be conducted.  Our file naming conventions involve descriptive words separated by underscores.

## Metadata

Processed_Data: "Combined_NY_COVID_Pop.csv"
Columns:
"County": New York counties, class factor
"pop2022": population in 2022, class integer
"area_milessquared": area in square miles, class numeral
"density_permilessquared": population density in square miles, class numeral
"sum_new_positives": sum of new positive COVID-19 cases, class numeral
"sum_cumulative_no_of_positives": sum of cumulative number of positive COVID-19 cases, class numeral "sum_total_number_of_tests": sum of total number of COVID-19 tests administered, class numeral
"sum_cumulative_no_of_tests": sum of cumulative number of COVID-19 tests administered, class numeral
"median_test_positive": median number of positive COVID-19 test results, class numeral
"settlement_type": classification of environment ("Urban", "Micropolitan", or "Rural"), class character



## Scripts and code

The "EDA_Final_Group_Project.RMD" file contains code used to import and merge the New York health data with the county data from the United States Census Bureau by left-merging them together.  This created the combined dataset that we used as our main data source.

## Quality assurance/quality control

We assured quality assurance by analyzing our data files carefully before and after downloading them to assure relevance and accuracy.  The datasets were wrangled individually to ensure that column names and variables matched up.  This ensured that our data was accurate when we merged them into a combined dataset.  We also ensured that our project was reproducible by using publicly available datasets and clearly defining our sources.

We assured quality control by having each group member write descriptive messages when committing change to Git.  This ensured that our progress was understood at an incremental level.  This kept everyone on track and in a shared understanding of our progress.  We also had each individual group member double check our data and script files after others updated them.
