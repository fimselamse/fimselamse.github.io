---
layout: post
title:  "On Crash Course to find the Crash Cause?: Evaluating the success of the Zero Initiative in NYC. (Final Project)"
date:   2023-05-04 23:55:00 +0100
categories: jekyll update
time-series-plot: /assets/time-series-collisions.svg
vehicle-type-2013: /assets/bar-chart-vehicle-type-2013.svg
crash-cause-2013: /assets/bar-chart-crash-cause-2013.svg
deaths-2013: /assets/injuries-by-type-2013.svg
injuries-2013: /assets/deaths-by-type-2013.svg
folium-map-2013: /assets/folium-map-2013.html
crashes-by-borough-2013: /assets/bar-chart-crashes-by-borough-2013.svg
collision-development-2022: /assets/collision-development-2022.svg
collision-regression: /assets/collision-regression.html
intersection-map: /assets/intersections-map.jpg

---

### Vision Zero: A Journey Towards Safer Streets or a Road to Nowhere?

In 2014, New York City embarked on an ambitious plan to eliminate traffic-related fatalities and serious injuries, launching the Vision Zero Initiative [@somecitation]. With a combination of engineering, enforcement, and education strategies, the goal was to redesign streets, modify traffic patterns, and encourage safer behavior among road users. Almost a decade later, the question remains: Has Vision Zero made a significant impact on traffic safety in the city that never sleeps?

In this investigative article, we delve into the data to assess the success or failure of the Vision Zero initiative. We will examine the changes implemented throughout the city, analyze accident statistics, and discuss the lessons learned as we attempt to determine whether Vision Zero has steered New York City towards a safer future.

The data used in this article is provided by the City of New York, and is composed of every police reported vehicle collision since June 2012. As such, the dataset does have it's limitations, and there may be additional colisions that were not reported.


### Status Quo 2013: How bad was it?
<!-- Show status of vehicle collissions as of 2013 -->
To understand whether the Vision Zero Initiative has been successful, we need to set a baseline. So how bad was the situation in 2013, such that it mandated a city-wide traffic safety intervention?

In 2013 the number of vehicle colisions in the City of New York amounted to a staggering 203.734 crashes, resulting in 55123 injured and the death of 297 people. Tragically, the fatalities are often bystanders. 

![Crashes by Vehicle Type]({{ page.deaths-2013 }}){:width="50%"}![Crashes by Vehicle Type]({{ page.injuries-2013 }}){:width="50%"}

As highlighted by the graph above, the most servere victims are often not involved or to blame for the car crash at all.

So who are causing these crashes and why do they happen?

<img src="{{ page.vehicle-type-2013 }}" alt="timeseries" style="display: block; margin: auto; width: 100%;" />

The graph above presents a top 10 breakdown of number of vehicle crashes in 2013 by type, including fatalities and serious injuries involving pedestrians, cyclists, and vehicle occupants. The figures reveal that personal sedans and SUVs constitue the vast majority of accidents, which makes sense given they make up the majority of vehicles on the streets. However this figure does not tell us what is causing all of these crashes.

<img src="{{ page.crash-cause-2013 }}" alt="timeseries" style="display: block; margin: auto; width: 100%;" />

This graph depicts the top 10 causes of crashes as noted in the police report of the crash. Curiously,  the cause has been reported as 'unspecified' in the majority of cases, presumably making it more difficult to address the issue at hand.

Lastly, lets take a look at where these collisions are happening.

<iframe src="{{page.folium-map-2013}}" width="100%" height="600px" frameborder="0">
    Sorry, your browser doesn't support iframes.
</iframe>

The heatmap above represents the most common locations of crashes in 2013. Zoom in to get a more precise look at where the crashes are happening. It's apparent from the heatmap that down/midt-town Manhattan is where the majority of crashes happen, painting a clear picture of where resources for the initiative should be allocated.

<img src="{{ page.crashes-by-borough-2013 }}" alt="timeseries" style="display: block; margin: auto; width: 100%;" />

However, looking at a bar chart, we see that it is actually Brooklyn where most of the crashes happen. The concentration is simply higher in Manhattan, making it pop out on a heatmap.

### Progress at a glimpse?
<!-- Show development of crashes -->

<img src="{{ page.time-series-plot }}" alt="timeseries" style="display: block; margin: auto; width: 100%;" />


### Initiatives taken
<!-- Highlight some of the different measures taken by the initiative -->

Now that we have a clearer understanding of the state of vehicle collisions in 2013, as well as insights on the causes and worst affected areas, we can start looking into the different iniatives taken by the Vision Zero project.

The Initiatives focuses on 4 main aspects of road safety: Engineering, Education, Enforcement, and Legislation.

#### Engineering
The engineering aspect focuses on enhancing road safety by implementing targeted engineering and design improvements, prioritizing high-risk areas such as intersections and major streets, and addressing the specific needs of vulnerable populations like older pedestrians and children.

The majority of traffic related accidents happen at intersections. In January 2022 the city undertook efforts to mitigate this by implementing a number of safety-measures such as signal changes, turn calming treatments, raised crosswalks, and other engineering modifications. Below is a map displaying where changes were implemented. These efforts were finalized in end of October 2022.
[cite https://www.nyc.gov/content/visionzero/pages/engineering]

<img src="{{ page.intersection-map }}" alt="timeseries" style="display: block; margin: auto; width: 70%;" />

Let's look at whether a drop in injuries and accidents were seen in this period.

<img src="{{ page.collision-development-2022 }}" alt="timeseries" style="display: block; margin: auto; width: 100%;" />

The graph above shows the development of monthly crashes since January 2022. It's apparent from the graph that the number of collisions have gone down since the intersection changes commenced. It's worth noting that the increase in collisions between March and June 2022 can be explained by a degree of seasonality, because there are generally more cars and people on the streets during the summer months. Even when taking this into consideration, there is a significant drop in collisions between March 2022 and March 2023 of about 10%.

<iframe src="{{page.collision-regression}}" width="100%" height="600px" frameborder="0">
    Sorry, your browser doesn't support iframes.
</iframe>

The graph above shows the development of weekly vehicle crashes if the decrease continues at this rate.

Another key part of these intersection changes was to protect pedestrians better in the case of a vehicle crash.



Given the noticeable decrease in vehicle accidents during and after the commencement of this initiative, it's fair to say that it has been successful.


### What worked and what didn't?
<!-- Go into details about each inititive taken -->


# References
<!-- Some bib -->