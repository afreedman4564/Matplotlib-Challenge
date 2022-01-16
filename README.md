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


