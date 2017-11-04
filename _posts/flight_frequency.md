---
layout: post
title: "Flight Frequency Graph"
date: 2017-11-03
---

As part of an assignment in Exploratory Data Analytics and Visualization course I created an [flight FREQUENCY GRAPH](https://shubhstiws.github.io/flight_frequency.svg)

## Situation:

Sun Country airlines, a unique player in the airline carrier industry has endured the threats of intense competition from large national brands. Started in 1983 as a charter carrier, it has expanded its business to offer scheduled flight services to various destinations. By 2014, Sun Country had survived bankruptcies, multiple economic recessions, threats of mergers and was now stable and profitable.

You can access the full case [here](https://carlsonschool.umn.edu/news/sun-country-airlines-engages-business-analytics-students-decode-data)

## Intuition:

In an earlier post I made a network graph to see all possible routes Sun Country was operating on but that graph did not give a picture of the number of bookings across various airports. For that we can visualize a flight frequency graph

## Interactions:

Unfortunately this offers no interactions, I will try to make it interactive in future.

## Caveats:

1. This is similar to the social network graph but instead of friends we have airports serving as dots

2. The thickness and color of lines denote the booking frequency among different routes ( A brighter yellow means high bookings and a dull orange means less bookings, similarly a thick line means higher bookings and a thin line means low bookings)

3. Lines crossing out denote flights to Alaska and Hawaii

4. This is a US only graph which means that all network lines originate and terminate in US only

5. This graph is constructed on the COMPLETE dataset and not the sampled dataset

## Insights:

1. Sun Country covers the entire nation of US as any major airline would

2. There is high traffic between major connecting hubs like major cities in East and West coast as well as the SOuth

3. Minneapolis is the airport with most number of bookings. Most people either start or end their journey in Minneapolis

4. There are substantial bookings in Denver and Hawaii

## Limitations:

1. The network diagrams are good at visualizing the connections between airports however we also need to quantitatively visualize them to discover some patterns between number of bookings and the amount spend on bookings

2. A lot of numbers on these graphs will make them hard to read hence we can make heatmaps for them

## Sources:

http://kateto.net/network-visualization
https://cran.r-project.org/web/packages/visNetwork/vignettes/Introduction-to-visNetwork.html
http://fontawesome.io/icon/plane/
https://datastorm-open.github.io/visNetwork/layout.html
