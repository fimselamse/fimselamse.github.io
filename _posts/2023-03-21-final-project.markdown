---
layout: post
title:  "On Crash Course to find the Crash Cause?: Evaluating the success of the Zero Initiative in NYC. (Final Project)"
date:   2023-05-04 23:55:00 +0100
categories: jekyll update
time-series-plot: /assets/time-series-collisions.html
vehicle-type-2013: /assets/bar-chart-vehicle-type-2013.html
crash-cause-2013: /assets/bar-chart-crash-cause-2013.html
deaths-2013: /assets/injuries-by-type-2013.svg
injuries-2013: /assets/deaths-by-type-2013.svg
crashes-by-borough-2013: /assets/bar-chart-crashes-by-borough-2013.html
collision-development-2022: /assets/collision-development-2022.html
collision-regression: /assets/collision-regression.html
injuries-development-2022: /assets/injuries-development-2022.html
deaths-by-year: /assets/deaths-by-year.html
total-injuries-by-year: /assets/total-injuries-by-year.html
total-deaths-by-year: /assets/total-deaths-by-year.html
total-deaths-by-year-type: /assets/total-deaths-by-year-type.html
fatal-crashes-by-year: /assets/fatal-crashes-by-year.html

folium-map-2013: /assets/folium-map-2013.html
folium-map-2022: /assets/folium-map-2022.html



intersection-map: /assets/intersections-map.jpg

---

### Vision Zero: A Journey Towards Safer Streets or a Road to Nowhere?

In 2014, New York City embarked on an ambitious plan to eliminate traffic-related fatalities and serious injuries, launching the Vision Zero Initiative [@somecitation]. With a combination of engineering, enforcement, and education strategies, the goal was to redesign streets, modify traffic patterns, and encourage safer behavior among road users. Almost a decade later, the question remains: Has Vision Zero made a significant impact on traffic safety in the city that never sleeps?

In this investigative article, we delve into the data to assess the success or failure of the Vision Zero initiative. We will examine the changes implemented throughout the city, analyze accident statistics, and discuss the lessons learned as we attempt to determine whether Vision Zero has steered New York City towards a safer future.

The data used in this article is provided by the City of New York, and is composed of every police reported vehicle collision since June 2012 as well as all related personal injuries and fatalities. As such, the dataset does have it's limitations, and there may be additional colisions that were not reported.

Almost all of the graphs in this post are interactive, either by letting the reader hover over graphs to get accurate readings or by letting them pick and choose what to see in a graph.

### Status Quo 2013: How bad was it?
In order to gage whether the Vision Zero Initiative has been successful, we first need to set a baseline. So how bad was the situation in 2013, such that it mandated a city-wide traffic safety intervention?

In 2013 the number of vehicle colisions in the City of New York amounted to a staggering 203.734 crashes, resulting in 55123 injured and the death of 297 people. 

![Crashes by Vehicle Type]({{ page.deaths-2013 }}){:width="50%"}![Crashes by Vehicle Type]({{ page.injuries-2013 }}){:width="50%"}

As highlighted by the graph above, the most servere victims are often not involved or to blame for the car crash at all. So who are causing these crashes and why do they happen?

<iframe src="{{page.vehicle-type-2013}}" width="100%" height="600px" frameborder="0">
    Sorry, your browser doesn't support iframes.
</iframe>

The graph above presents a top 10 breakdown of vehicle crashes in 2013 by type of vehicle, including fatalities and serious injuries involving pedestrians, cyclists, and vehicle occupants. The figures reveal that personal sedans and SUVs cause the vast majority of accidents, which makes sense given they make up the bulk of vehicles on the streets. However this figure does not tell us what is causing all of these crashes.

<iframe src="{{page.crash-cause-2013}}" width="100%" height="600px" frameborder="0">
    Sorry, your browser doesn't support iframes.
</iframe>

This graph depicts the top 10 causes of crashes as noted in the police report of the crash. Curiously, the cause is often been reported as 'unspecified', making it more difficult to address the issue at hand. Lastly, lets take a look at where these collisions are happening.

<iframe src="{{page.folium-map-2013}}" width="100%"  height="600px" frameborder="0">
    Sorry, your browser doesn't support iframes.
</iframe>

The heatmap above highlight the most concentrated areas of crashes in 2013. Zoom in to get a more precise look at where the crashes are happening. It's apparent from the heatmap that the highest concentration of crashes is down/midt-town Manhattan, painting a clear picture of where resources for the initiative should be allocated.

<iframe src="{{page.crashes-by-borough-2013}}" width="100%" height="600px" frameborder="0">
    Sorry, your browser doesn't support iframes.
</iframe>

However, looking at a bar chart we see that it is actually Brooklyn where most of the crashes happen. The concentration is simply higher in Manhattan, making it pop out on a heatmap.

### What measures are being taken?
Now that we have a clearer understanding of the state of vehicle collisions in 2013, as well as insights on the causes and worst affected areas, we can start looking into some of the initiatives taken by the Vision Zero project and what effect they had in practice. The Initiative focuses on 4 main aspects of road safety: Engineering, Education, Enforcement, and Legislation. In this section we will be looking at two of the major efforts made to reduce traffic accidents and serious injuries/fatalities caused by them.

#### Engineering Initiatives
The engineering aspect focuses on enhancing road safety by implementing targeted engineering and design improvements, prioritizing high-risk areas such as intersections and major streets, as well as addressing the specific needs of vulnerable populations like older pedestrians and children. Between 2014 and 2023 the City of New York has completed over 1000 street improvement projects. [cite https://www.nyc.gov/html/dot/downloads/pdf/safety-treatment-evaluation-2005-2018.pdf]. 

<iframe src="{{page.time-series-plot}}" width="100%" height="600px" frameborder="0">
    Sorry, your browser doesn't support iframes.
</iframe>

The graph above illustrates the development of monthly crashes since 2013. We see that the number of crashes rose in the initial period following beginning of the project, followed by a steep drop coinciding with the beginning of the covid-19 pandemic where the state of New York entered a lockdown [cite https://www.governor.ny.gov/news/governor-cuomo-signs-new-york-state-pause-executive-order]. Interestingly, the number of monthly crashes remained low even after the the lockdown ceased, which may be as a result of some of the measures taken by Vision Zero. Additionally, we also see a high degree of seasonality in the data, with a yearly maximum in May/June and a yearly minimum in February.

The majority of traffic related accidents happen at intersections. In January 2022 the city announced efforts to mitigate this by implementing a number of safety-measures such as signal changes, turn calming treatments, raised crosswalks, and other engineering modifications. These efforts were finalized in end of October 2022. Below is a map displaying where changes were implemented. 
[cite https://www.nyc.gov/content/visionzero/pages/engineering]

<img src="{{ page.intersection-map }}" alt="timeseries" style="display: block; margin: auto; width: 70%;" />

Let's take a look at whether these changes have had a noticeable effect since they commenced.

<iframe src="{{page.collision-development-2022}}" width="100%" height="420px" frameborder="0">
    Sorry, your browser doesn't support iframes.
</iframe>

The graph above shows the development of monthly crashes since January 2022. It's apparent from the graph that the number of collisions have gone down since the intersection changes commenced. The increase in collisions between March and June 2022 can be explained by a degree of seasonality, since there are generally more cars and people on the streets during the summer months. Even when taking this into consideration, there is roughly a 10% drop in collisions between March 2022 and March 2023.

<iframe src="{{page.collision-regression}}" width="100%" height="420px" frameborder="0">
    Sorry, your browser doesn't support iframes.
</iframe>

The graph above shows the weekly number crashes and the predicted development of weekly crashes if this trend continues. Based on these predictions, we can expect to see roughly another 15% drop in traffic accidents before the end of 2023 if the trend continues.

Another key part of the intersection alterations was to protect pedestrians and reduce the number of injuries and fatalities in the case of a crash.

<iframe src="{{page.injuries-development-2022}}" width="100%" height="420px" frameborder="0">
    Sorry, your browser doesn't support iframes.
</iframe>

Looking at the graph above it becomes clear that the efforts to reduce pedestrian injuries have been unsuccessful or have yet to take effect as a result of the changed made to intersection made in 2022. Without too much speculation, one can imagine that introducing a lot of changes to intersection might take some getting used to for the natives of NYC. So while the number of crashes have gone down, the number of injuries have stalled or even seen an increase!

In a press release, the New York City Department of Transportation (NYC DOT) praised the Vision Zero Initiative for reducing the number of fatalities by 6.3% from 2021 to 2022 for the first time in three years [cite https://www.nyc.gov/html/dot/html/pr2023/vision-zero-fatalities-dropped-2022.shtml]. While this is true for the overall number of fatalities, pedestrian fatalities actually saw a slight increase in this period as seen by the graph below.

<iframe src="{{page.deaths-by-year}}" width="100%" height="420px" frameborder="0">
    Sorry, your browser doesn't support iframes.
</iframe>

Given the noticeable decrease in vehicle accidents since the commencement of intersection engineering initiative, its *safe* to say it has been a success. However, it is too early to give praise for reducing fatalities and injuries, as the efforts missed the mark on this front.

#### Legislative
The Vision Zero Initiative has also made large efforts to pass legislations promoting road safety. Key highlights include the introduction of a 25 mph default speed limit in New York City (S7892/A10144 of 2014), meant to double pedestrian survival chances in collisions and reduce the likelihood of serious crashes. The speed camera program, initially established in 2013, was expanded in 2019 (S4331/A6449) to cover 750 school zones and extended operational hours to between 6 AM and 10 PM within a quarter-mile of a school building. Finally, in 2022, the Speed Camera 24/7 Extension (S5602/A10438) removed all restrictions on speed camera operating hours, allowing them to function around the clock throughout the year [cite https://www.nyc.gov/content/visionzero/pages/legislation].

One goal of legislation S7892/A10144 was to reduce the number of serious injuries as a result of a vehicle crash by reducing the city-wide speed limit from 30mph to 25mph. While the data provided by NYC DOT does not specify the severity of injuries sustained, any injuries resulting in death are pretty serious.
<iframe src="{{page.total-deaths-by-year-type}}" width="100%" height="420px" frameborder="0">
    Sorry, your browser doesn't support iframes.
</iframe>
This graph displays the total number of deaths caused by vehicle collisions by year and type of road user. From the graph, we see a significant and sustained drop in predestrian fatalities from 2014 onwards. The bill containing this mandate passed in 2014, coniciding with the drop fatalities. Despite this, there was not a noticeable drop in fatalities bicyclists or vehicle occupants, the latter even seeing an increase.  

The second goal of this legislation was to reduce the likelihood of serious crashes.
<iframe src="{{page.fatal-crashes-by-year}}" width="100%" height="420px" frameborder="0">
    Sorry, your browser doesn't support iframes.
</iframe>
However, looking at the number of fatal crashes since the bill passed, we see that although there was an immediate drop in 2014, it has failed to sustain this level since then.    

# Where do we stand today?
We have looked at a couple of the specific efforts made to increase road-safety and seen what direct effects they had, but those were just a few pieces of a much larger puzzle. So where does the City of New York stand today compared to a decade ago?

We saw from our analysis that since 2013 the overall number of crashes has gone down by 50% from 203734 in 2013 to only 100466. The number of pedestrian fatalities have also gone down, while the same number among vehicle occupants remained stable, sometimes even seeing an increase. Lastly, we saw  

If we compare the heatmap from 2013 to that of 2022, the difference becomes clear.
<iframe src="{{page.folium-map-2022}}" width="100%" height="600px" frameborder="0">
    Sorry, your browser doesn't support iframes.
</iframe>


# Where do we go from here?


# References
<!-- Some bib -->