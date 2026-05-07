# CHIP705
Python Notebook Final

# CMS Hospital Star Ratings and Patient Outcomes

# Overview
This project examines whether a relationship exist between CMS hospital overall star ratings and patient outcome measures, specifcally 30-day mortality rates across U.S. hospitals. This idea stems from my previous CHIP 721: US Health Care Systems course I took my Fall 2025 semester and an overall focus on Electronic Health Records. This analysis explores how publically reported quality scores align with real patient outcomes derived from hospital EHR submissions.

# Research Question
> Is there a relationship between CMS hospityal overall star ratings and patient outcome measures, specifically 30-day mortality rates, across U.S. hospitals?

# Data Sources
All data derives directly from the Centers for Medicare & Medicaid Services (CMS) via data.cms.gov. The notebook pulls btoh datasets live using the CMS offical CSV download endpoint.

 - https://data.cms.gov/provider-data/dataset/xubh-q36u
 - https://data.cms.gov/provider-data/dataset/ynj2-r877

No manual downloads are required. The notebook pulls btoh datasets live using the CMS offical CSV download endpoint. Both datasets are derived from EHR data submitted by participating hospitals.

# Project Structure
milestone_2.ipynb   # Main Jupyter Notebook with full analysis
README.md           # This file

# Walkthrough
1. Setup & Pre-processing: loads required libraries such as pandas and matplotlib
2. Data Retrieval: Both data is pulled directly from the CMS datasets live from data.cms.gov
3. Explore the Data: Preview column names and structure of each dataset
4. Clean and Filter Data: Isolate the 6  30-day mortality metrics and remove any non numerical or missing data
5. Calculate Average Mortality Rate for Each Hospital: Averages the data of each hospital into a single row per facility
6. Merge Datasets: Combines CMS rating with outcome scores based on Facility ID
7. Descriptive Statistics per Rating: Identified the mean, median, and standard deviation per each CMS star rating
8. Visualizations: Creates 2 visual charts that highlight the relationship between CMS rating and outcomes
9. Summary and Conclusion: Plain-text conclusion that display real numbers directly from data

# How to run
1. Open 'milestone_2.ipynb' in Jupyter Notebook or Visual Studio
2. Run all cells in order from top to bottom
3. The notebook will automatically pull the latest CMD data and generate the corresponding visualizations

# Visualizations
1. Average 30-day Mortality by CMS Star Rating - A bar chart that displays the mortality rate in a 30-day period for each star rating group
2. Mortality rate by condition and CMS Star Rating - A group bar chart that illustrates mortality rates per condition and broken down by star rating
