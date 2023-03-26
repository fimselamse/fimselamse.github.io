---
layout: post
title:  "Should you drop the car? (Assignment 2)"
date:   2023-03-14 09:53:27 +0100
categories: jekyll update
time-series-plot: /assets/images/time-series.png
folium: /assets/folium2.html

---

Need another good reason to go carless in the city? While San Francisco has one of the highest rates of car breakins in the world, many people still opt for the car rather than use one of the citys public transportation options. If this is you, I have bad new for you - it's only getting worse.

### Background

Using data on crime in San Francisco provided by the San Francisco Police Department (SFPD), I seek to make a case for going green in the Capital of NorCal. The dataset covers all reported crimes between 2003 and 2017 in the San Francisco area. While the entire police reports are not available to the public, this data includes things such at location, time, and type of crime, allowing us to dig into the statistics of crime in San Francisco.

### Why should I leave the car altogether and not simply use it less?
Using your car less is a perfectly valid way to reduce your carbon footprint, however, as you will see, this is not the only point I'm trying to make in this blog post. The real reason why you should drop the car is because of the increasing car thefts and break-ins.

![timeseries]({{ page.time-series-plot}}){:width="100%"}

### Where to park your car??

Here is a map that might help you determine where to park.

<!-- {% include folium.html %} -->
<iframe src="{{page.folium}}" width="100%" height="600px" frameborder="0">
    Sorry, your browser doesn't support iframes.
</iframe>

### Development of theft patterns

Here is an interactive plot that shows how the 24-hour crime cycle has developed over the years.

{% include bokeh.html %}{:width="100%"}