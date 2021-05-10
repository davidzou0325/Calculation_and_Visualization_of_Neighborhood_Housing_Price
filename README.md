# Calculation_and_Visualization_of_Neighborhood_Housing_Price

The main purpose for this tool is to visualize housing data (mainly gross rent and sale price per square foot) in graph using hvplot and MapBox.

Step 1: Import
  By achieving the main purpose, importing different libraries and dependencies are the first step.
  Importing list includes: os, pandas, plotly.express, hvplot.pandas, pathlib and dotenv.
  After importing libraries, test MapBox token to ensure it is working properly. Then import local csv data. 
  
Step 2: Calculate and Plot the Housing Units/year.
  Using groupby and sort_value function to recreate a new data frame. 
  Plotting the new data frame with hvplot function and making x='Year', y='housing_units' with a title='Housing Units in San Francisco from 2010 to 2016'
  
Step 3: Calculate and Plot the Average Sale Prices per Square Foot.
  Using groupby and sort_value function to recreate two new data frames -- 'gross_rent_by_year' and 'prices_square_foot_by_year'. 
  Using hvplot to plot two dataframes seperately, and overlay the graph with new title and labels.
  
Step 4: Compare the Average Sale Prices by Neighborhood.
  Using groupby and sort_value function to recreate two new data frames, drop out unnecessary column. 
  Using groupby and hvplot to plot the graph with different neighborhoods as variables that can be chosen and inspect specific data in that neighborhood.
  Combining two graphs using groupby and hvplot with differnet neighborhood as variable.
  
Step 5: Build an Interactive Neighborhood Map.
  Importing different csv data file with location latitude and lontitude.
  Using groupby and sort_value function to recreate a new data frame. 
  Using concat function to combine two data frames as one piece.
  Dropping NaN value and reframe the index.
  Using plotly.express and MapBox to plot an area heatmap with different gross rent value and sale price/square foot in one graph.
  
Conclusion:
  Based on the graph and data, I would recommend the company to focus on renting return other than sales return since gross return keeps increasing when sales price can be lower than a year before in some cases. Union Square District is a highly recommend area because it has the highest gross rent value among other neighborhoods.
