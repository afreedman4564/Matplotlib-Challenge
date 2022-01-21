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

## Calculate summary stats
    - use groupby on drug regimen along with agg to calculate in one df all stats
    - force column rename using .columns and the reset_index using inplace = True to allow overwrite of prior df
    - calculate same statistics for complete file(overall), using similar approach as above
    - combine both drug regimen and overall summary file using append

## Create bar graphs
    - create bar graph using pandas
    - create bar graph using matplotlib.pyplot
    - add formatting for aesthetics
        - title, x-axis, y-axis, footnote, green shading for bars

## Create pie graphs
    - groupby gender and calculate unique Mouse ID by gender
    - Transpose the data table
    - create pie graph with pandas and matplotlib.pyplot

## Quartiles, Outliers and Boxplots
    - creat filtered df with regimens: Capomulin, Ramicane, Infubinol, and Ceftamin
    - use groupby to id the last timepoint for each mouse
    - left merge back to main df to obtain the tumor size
    - create list of drug regimens from df
    - create series of empty lists and use for loop to calculate for each regimen quartiles, iqr and upper and lower bounds
    - use calculated upper and lower bounds to id possible outliers
    - create box plot

## Scatter plots
    - create list with tumor volume and weight
    - create line plot for l509 mouse, trending timepoint and tumor size
    - create scatter plot of weight and avg tumor size for all mice in Capomulin regimen
    - generate identical scatter plot, overlaying regression line and displaying the regression model along with r-squared








