# Proptech-Real-Estate-
# Housing Rental Analysis for San Francisco

In this challenge, your job is to use your data visualization skills, including aggregation, interactive visualizations, and geospatial analysis, to find properties in the San Francisco market that are viable investment opportunities.

## Instructions

Use the `san_francisco_housing.ipynb` notebook to visualize and analyze the real-estate data.

Note that this assignment requires you to create a visualization by using `hvPlot` and `GeoViews`. Additionally, you need to read the `sfo_neighborhoods_census_data.csv` file from the Resources folder into the notebook and create the DataFrame that you’ll use in the analysis.

The main task in this Challenge is to visualize and analyze the real-estate data in your Jupyter notebook. Use the `san_francisco_housing.ipynb` notebook to complete the following tasks:

1. Calculate and plot the housing units per year.

2. Calculate and plot the average prices per square foot.

3. Compare the average prices by neighborhood.

4. Build an interactive neighborhood map.

5. Compose your data story.

## Calculate and Plot the Housing Units per Year

For this part of the assignment, use numerical and visual aggregation to calculate the number of housing units per year, and then visualize the results as a bar chart. To do so, complete the following steps:

1. Use the `groupby` function to group the data by year. Aggregate the results by the mean of the groups.

2. Use the `hvplot` function to plot the `housing_units_by_year` DataFrame as a bar chart. Make the x-axis represent the year and the y-axis represent the housing_units.

3. Style and format the line plot to ensure a professionally styled visualization.

Answer the following question:

- What’s the overall trend in housing units over the period that you’re analyzing?

## Calculate and Plot the Average Sale Prices per Square Foot

For this part of the assignment, use numerical and visual aggregation to calculate the average prices per square foot, and then visualize the results as a bar chart. To do so, complete the following steps:

1. Group the data by year, and then average the results. What’s the lowest gross rent that’s reported for the years that the DataFrame includes?

2. Create a new DataFrame named `prices_square_foot_by_year` by filtering out the “housing_units” column. The new DataFrame should include the averages per year for only the sale price per square foot and the gross rent.

3. Use `hvPlot` to plot the `prices_square_foot_by_year` DataFrame as a line plot.

4. Style and format the line plot to ensure a professionally styled visualization.

Use both the `prices_square_foot_by_year` DataFrame and interactive plots to answer the following questions:

- Did any year experience a drop in the average sale price per square foot compared to the previous year?
- If so, did the gross rent increase or decrease during that year?

## Compare the Average Sale Prices by Neighborhood

For this part of the assignment, use interactive visualizations and widgets to explore the average sale price per square foot by neighborhood. To do so, complete the following steps:

1. Create a new DataFrame that groups the original DataFrame by year and neighborhood. Aggregate the results by the mean of the groups.

2. Filter out the “housing_units” column to create a DataFrame that includes only the sale_price_sqr_foot and gross_rent averages per year.

3. Create an interactive line plot with `hvPlot` that visualizes both sale_price_sqr_foot and gross_rent. Set the x-axis parameter to the year (`x="year"`). Use the `groupby` parameter to create an interactive widget for neighborhood.

