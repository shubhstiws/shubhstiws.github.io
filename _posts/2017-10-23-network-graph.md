---
layout: post
title: "Shubhankar Tiwari network graph"
date: 2017-10-23
---

As part of an assignment in Exploratory Data Analytics and Visualization course I created an [interactive network graph] https://shubhstiws.github.io/SC_network.html)

#Situation:

Sun Country airlines, a unique player in the airline carrier industry has endured the threats of intense competition from large national brands. Started in 18983 as a charter carrier, it has expanded its business to offer scheduled flight services to various destinations. By 2014, Sun Country had survived bankruptcies, multiple economic recessions, threats of mergers and was now stable and profitable.

You can access the full case [here] (https://carlsonschool.umn.edu/news/sun-country-airlines-engages-business-analytics-students-decode-data)

#Intuition:

The origins and destination have a huge amount of categorical variables (airport codes) and plotting them in a bar graph would be a mess. To visualize the connections between the airports I made a network diagram:

1. The Network diagram is constructed for all connections between airports on the COMPLETE dataset and not the sampled dataset

2. The nodes denote a unique airport ( includes US and non US airports where ever SunCountry operates)

3. The links are connections between airports (if the raw data contained a row with a passenger booking a flight between two airports it appears as a link in the network diagram)

4. There is no directional inforation in the links, there is weight information ( the total number of flights bookings and the total amount spend on a particular link but visualizing that would make this graph more dense and hard to comprehend, seperate heatmaps are dedicated for that down below in the analysis )

5. The color denotes the country of operation, all US airports are blue color and have an inclined airplane as an icon

#Interactions:

1. Clicks on a particular airport reveal all the networked airports with it

2. Hovering on an airport reveals the airport Name

3. Dragging a particular node reveals all the connections and is quite FUN to play

4. A drop down box lets you select a particular country and view all its networked airports

5. The standard PAN and ZOOM buttons are available to move the chart around ( this can also be accomplished by mouse actions and scroll to zoom)

6. A reset button is available to zoom to the default level

#Insights:

1. Most of the Sub Country network is concentrated in Minneapolis but it has connections all over US

2. Major connecting airports are Denver and Dallas

3. Sun Country also has operation is 10 other countries apart from US (PR and VI counted as part of the union)

However this graph does not give us a picture of the number of bookings across various airports. For that we can visualize a flight frequency graph
