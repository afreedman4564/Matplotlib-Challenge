# Matplotlib-Challenge

## Import dependencies with aliases
- matplotlib notebook
- pandas
- numpy
- matplotlib.pyplot

## Read in csv files and perform merge(s)
- use panda read_csv approach

## Perform data intake diagnostics
- look at first few rows
- count records
- calculate null values for each column in each dataframe
**- id duplicate mice-timepoint**
    - calculate a dupkey combining Mouse ID and Timepoint
    - Force Timepoint into str using astype
    - use value_counts to calculate duplicates
    - use loc to filter on those with multiple dupkey
    - reset the index and then rename the columns
    - find the Mouse ID(s) with any duplicate Mouse ID and Timepoint
    - merge back to original mouse combined file and create a new df with all records for the mouse with duplicates
    
**- create df removing
    - use loc to create a clean list without the mouse with duplicates
    - calculate the number of 'clean' unique mice

## Create Summary Stats Table
    - Use groupby regimen and agg function to allow efficient calculation and creation of single df
    - Reset index to clean up the view




