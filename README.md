# Global Economic Report: 1960-2018

### Overview

Using Python and popular libraries such as Pandas, Numpy, Matplotlib and Seaborn, I created a comprehensive data visualization on global economic trends spanning from 1960 to 2018. This project dives deep into GDP growth, population shifts, and development indicators to analyze economic progress and provide insightful projections.

## Steps:

Here's a breakdown of the steps I followed and the insights uncovered:

## 1. Data Collection and Cleaning:
I got the raw data from Maven Analytics containing different tables. 
- Using Pandas, I first merged the tables while keeping only relevant columns. 
- Then I checked the data types and make them appropriate. There was no column for population which would be required in analysis and visualization, but using total GDP and GDP per capita columns, I created population column.
- I cleaned and structured the data to ensure consistency across various economic indicators. I analyzed data using describe and info methods.
  
## 2. Data Analysis and Transformation
With the data prepared, I conducted exploratory data analysis (EDA) using Pandas and NumPy. This step helped reveal patterns and relationships, setting a foundation for insightful visualizations.
E.g. I discovered that the correlation between GDP per capita and HDI is 0.65
For further analysis and creating visuals, I created few tables which could be used.
  1. gdp_pivot table created by pivoting table with Year on index, Regions as columns and sum aggregated values of Total GDP
  2. pop_pivot table created by pivoting table with Year on index, Regions as columns and sum aggregated values of Total Population.
  3. web_hdi_by_region table created by groupby Region and aggregating hdi using mean.

![image](https://github.com/user-attachments/assets/a5c4d221-3c2d-4143-8b0a-e62e171785cd)


With these tables created, I moved to visualization phase.

## 3. Visualization of Trends

To present the findings, I utilized Matplotlib and Seaborn to create a series of visualizations that highlight the evolving global economic landscape.
After creating the visuals separately, I used Matplotlib's gridspec module to bring them together to create a formal report

![Economic Report Project](https://github.com/user-attachments/assets/cd2cf914-a338-4411-ac71-9f88b5314fad)


### - GDP Growth Over Time

Visualizes GDP growth trends from 1960 to 2018, highlighting exponential growth, particularly in East Asia, which has overtaken Western regions thanks to powerhouse economies like China and South Korea. This chart offers a historical overview and projections for potential future leaders in global economic growth.

### - Population Dynamics

A stacked area plot shows how global population grew from 2 billion to 7.5 billion. This helps identify population trends by region, shedding light on emerging regions that could drive economic growth in the coming decades, such as South Asia and Sub-Saharan Africa.

### - Life Expectancy vs Wealth:

Using a scatter plot, I correlated GDP per capita with life expectancy by countries. This provides a visual representation of the impact of economic growth on quality of life, with notable insights such as the life expectancy in developing nations over the past few decades. We can see smaller European countries of high GDP per capita have high life expectancy as well. 

### - Energy Consumption and Economic Development

Analyzes the relationship between electricity consumption per capita and GDP per capita across countries. The chart underscores how higher energy availability supports development, especially in emerging economies, highlighting the importance of infrastructure investment for sustainable growth.

### - Regional HDI Comparison

A bar chart illustrates regional HDI values, making it easier to compare standards of living across continents. This helps pinpoint regions where growth could be accelerated through targeted economic policies and education.


## Conclusion

This report demonstrates the power of data visualization in analyzing and forecasting economic trends, offering clear insights into the links between economic growth, development, and quality of life. The analysis suggests that while East Asia has seen tremendous growth in recent years, future global economic leadership may shift to regions like South Asia and Sub-Saharan Africa as they continue to expand and modernize.

### Key Takeaways:

#### - East Asia’s Economic Ascent: Rapid growth, led by China and South Korea, has redefined global economic power since the 1960s.
#### - Population Growth: South Asia and Sub-Saharan Africa show the largest population increases, indicating potential future economic hotspots.
#### - Energy and Development: Increased access to electricity is a catalyst for economic growth, particularly in emerging markets.
