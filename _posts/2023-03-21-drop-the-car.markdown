---
layout: post
title:  "Should you drop the car? (Assignment 2)"
date:   2023-03-14 09:53:27 +0100
categories: jekyll update
time-series-plot: /assets/time-series.png
folium: /assets/folium2.html
bokeh: /assets/bokeh.html

---

## The Soaring Tide of Theft in San Francisco: A Data-Driven Deep Dive

### Unraveling the Disturbing Trend of Rising Thefts in the Golden Gate City

The enchanting city of San Francisco, known for its iconic Golden Gate Bridge, vibrant culture, and booming tech scene, is grappling with a disturbing trend: a sharp rise in thefts. A data-driven inquery reveals the extent of this crisis, offering a vivid snapshot of the situation through a series of static and interactive plots.

The data used in this article is provided by the San Francisco Police Departmen (SFPD), and consists of all the reported crimes ranging from 2008 to 2018, and contains details about the crime such as location, type of crime and time of incident.

### A Troubling Timeline - The Escalating Number of Thefts

The first plot in our exploration is a timeseries visualization, which tracks the daily number of thefts in San Francisco in the 10-year period between 2008 and 2018. The graph paints a startling picture, as it shows a consistent upward trend in incidents of theft.

![timeseries]({{ page.time-series-plot}}){:width="100%"}


### Hotspots of Crime - A 24-Hour Heatmap of Theft Incidents

To provide a geographical perspective on theft occurrences in San Francisco, we have created an interactive heatmap that shows where most thefts are committed. This map not only displays the city's crime hotspots but also illustrates the fluctuation of the number of occurences throughout the 24 hours of the day, revealing fascinating temporal insights into the theft problem in San Francisco. 

<iframe src="{{page.folium}}" width="100%" height="600px" frameborder="0">
    Sorry, your browser doesn't support iframes.
</iframe>

From the heatmap, it becomes inceasingly clear that most thefts are comitted later in the day and night, as illustrated by the hotspots occuring later in the day. Additionally, the map also illustrates where the most theft is being comitted. From the map, downtown seems to be the area which is worst affected, which is to be expected, as this is also where the density of people is highest.

### Comparing Apples to Apples - An Interactive plot of Crime Trends

Our final plot is an interactive timeseries that allows readers to compare the rise in theft with other types of crime in San Francisco. The illustration offers an wide array of different crimes, enabling users to put the theft epidemic into context and understand its significance in relation to other criminal activities. It also aims to highlight how crime in particular, has seen a steep increase compared to other types of crime in San Francisco.

To compare different types of crime, simply click on the type of crimes in the legend you want to compare. You can deselect types of crime by clicking on them again.

<iframe src="{{page.bokeh}}" width="100%" height="600px" frameborder="0">
    Sorry, your browser doesn't support iframes.
</iframe>

## Conclusion

In summary, our data-driven exploration of theft in San Francisco brings to light the alarming increase of the city's crime problem, as well as an overview of where the theft is being comitted. By providing a timeseries plot of theft incidents, a 24-hour heatmap of crime activity, and an interactive comparison of various crime types, we aim to provide readers with a multifaceted understanding of the theft crisis in the Golden Gate City. It is our hope that this information will spur a constructive dialogue among policymakers, law enforcement officials, and citizens, leading to effective solutions for addressing the city's theft epidemic.
