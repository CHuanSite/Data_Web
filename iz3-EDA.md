---
layout: page
title: EDA
permalink: /EDA/
---
There are in fact two different types of data: **Raw Data** and **Summary Data**. To do EDA on the data, we do seperately on the **Raw Data** and **Summary Data**

#  Raw Data
Here we explore the browser distribution. 
Most of the visitors used chrome browser. The most used browsers are chrome, safari, firefox. 

<p align="center">
  <img src="{{site.url}}{{site.baseurl}}/assets/1.png" width="600" />
</p>

Here we explore the device category distribution. 
The most used device is desktop. 
<p align="center">
  <img src="{{site.url}}{{site.baseurl}}/assets/2.png" width="600" /> 
</p>

Here we explore the device operating system. 
Most of the visitors used Mac. The most used operating systems are Mac, Windows, IOS, Android.  
<p align="center">
  <img src="{{site.url}}{{site.baseurl}}/assets/3.png" width="600" /> 
</p>

Now we check these features correlation.
The most frequent combiniation of the visits is using Chrome browser from Mac. 
<p align="center">
  <img src="{{site.url}}{{site.baseurl}}/assets/4-1.png" width="600" /> 
</p>
The most frequent combiniation of the visits is using Chrome browser on desktop. 
<p align="center">
  <img src="{{site.url}}{{site.baseurl}}/assets/4-2.png" width="600" /> 
</p>

The state with the largest number of visit is California, and the state with the second largest visit is New York. 
<p align="center">
  <img src="{{site.url}}{{site.baseurl}}/assets/5-1.png" width="600" /> 
</p>
Consistent with the number of visit, the state with the highest transaction revenue is California, and the state with the second highest transaction revenue is New York. 
<p align="center">
  <img src="{{site.url}}{{site.baseurl}}/assets/5-2.png" width="600" /> 
</p>
Now we show the distribution of visit per state, considering only visits with non-zero transactions. 
The total numbers in each state are smaller, and the top 2 states with largest number of visits are California and New York. 
<p align="center">
  <img src="{{site.url}}{{site.baseurl}}/assets/5-3.png" width="600" />
</p>
We plot the time series for transaction revenues. 
April has the highest revenue.
<p align="center">
  <img src="{{site.url}}{{site.baseurl}}/assets/6-1.png" width="600" />
</p>
Revenue is higher in weekdays than weekends.
<p align="center">
  <img src="{{site.url}}{{site.baseurl}}/assets/6-2.png" width="600" />
</p>

#  Summary Data

Based on [Random Forest](https://en.wikipedia.org/wiki/Random_forest), we obtain the feature importance of the data

<p align="center">
<img src="{{site.url}}{{site.baseurl}}/assets/feature_importance.png" width="1000" />
</p>



