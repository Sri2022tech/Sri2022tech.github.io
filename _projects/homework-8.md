---
name: "Homework 8 - Bigfoot Sightings"
tools: [Python, HTML, vega-lite]
description: Two visualizations showing Bigfoot sightings by season and location.
custom_js:
- vega.min
- vega-lite.min
- vega-embed.min
- justcharts
---

# Bigfoot Sightings Analysis
For this assignment, I used the BFRO Bigfoot reports dataset. This dataset helped me create two visualizations using Python and Altair. The purpose of these visualizations is to explore how Bigfoot sightings may be different by season and where they happen across the US. 

# Plot 1: Bigfoot Sightings by Season
The first visualization is a bar chart. The bar chart shows the number of Bigfoot sightings that was reported during each season. I used nominal encoding for the x-axis to represent the season and quantitative encoding for the y-axis to show the number of sightings. I also used different colors for each season to make it easier for comparison. Altair counts the number of reports in each season, I didn't have to manually calculate the totals in Python. From the chart, summer has the most reported sightings. Fall has the second most sightings and winter has the least. 

<vegachart schema-url="{{ site.baseurl }}/plot1.json" style="width: 100%"></vegachart>

# Plot 2: BigFoot Sightings by Location
The second visualization is a scatterplot. The scatterplot shows the locations of the reported Bigfoot sightings across the US. I used quantitative encoding for both axes. The longitude was on the x-axis and the latitude was on the y-axis. I also used nominal encoding for color to show the different seasons. Each season has a different color, which makes it easier to see where the sightings happened during different times of the year. In Python, I removed rows that had missing latitude or longitude values so only sightings with coordinates would appear on the graph. Each point shows a reported Bigfoot sighting. 

<vegachart schema-url="{{ site.baseurl }}/plot2.json" style="width: 100%"></vegachart>

# Interactivity
For the second visualization, I added a dropdown menu. This dropdown menu lets users filter Bigfoot sightings by season. Users can select a specific season or view all the seasons at same time. This makes the plot easier to understand as users can focus on one at a time as well compare where sightings happened during different seasons.

# Data and Analysis
[The Data](https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/bfro_reports_fall2022.csv)
[The Analysis](https://github.com/Sri2022tech/Sri2022tech.github.io/blob/main/Workbook.ipynb)
