---
layout: page
title: Data
permalink: /Data/
---

[Data Download](https://github.com/CHuanSite/Google-Revenue/tree/master/dataset)

The original data is from Kaggle contest "Google Analytics Customer Revenue Prediction". And also hits part from google analytics API (which is also included in Kaggel version 2 data).

# Raw Data
A brief description of the original data can be found from Kaggle

1. fullVisitorId- A unique identifier for each user of the Google Merchandise Store.

2. channelGrouping - The channel via which the user came to the Store.

3. date - The date on which the user visited the Store.

4. device - The specifications for the device used to access the Store.

5. geoNetwork - This section contains information about the geography of the user.

6. socialEngagementType - Engagement type, either "Socially Engaged" or "Not Socially Engaged".

7. totals - This section contains aggregate values across the session.

8. trafficSource - This section contains information about the Traffic Source from which the session originated.

9. visitId - An identifier for this session. This is part of the value usually stored as the _utmb cookie. This is only unique to the user. For a completely unique ID, you should use a combination of fullVisitorId and visitId.

10. visitNumber - The session number for this user. If this is the first session, then this is set to 1.

11. visitStartTime - The timestamp (expressed as POSIX time).

12.hits - This row and nested fields are populated for any and all types of hits. Provides a record of all page visits.

13. customDimensions - This section contains any user-level or session-level custom dimensions that are set for a session. This is a repeated field and has an entry for each dimension that is set.

14.totals - This set of columns mostly includes high-level aggregate data.

Where the totals and hits are all json object, and we expand it. Totals contain high-level aggregated data, like revenue is in the totals. 

Hits is the detailed web action the visitor have. It will record every website visited and action the visitor done. Therefore the transaction columns are in the hits, which means if you use hits to predict the revenue then you can atucally fully recover those digits. Therefore we remove all columns related directly to transaction. 

There are still lots of other features remian in hits.

time -- millisecond of visiting time for each pages

Product - told you which good are visitor currently viewing, also contain their price and name

page.* - told you the exact web path along the visitor's visiting.

social.* - told you if the visitor have a social network referral and where the referral from.

content* - told you what class of content are visitor viewing

eventInfo* - told you the action visitor took during the whole visiting

And other technical columns not easy to understand. In this version of hits data, it contain multiple rows for one visitor, therefore we need to get some features and summarise it. We do this through a detailed EDA of the hits data only and find some patterns for buyers. Therefore we reduce our hits data according to these patterns. And only use the reduced features and no original data, doing a randomforest already improve result to some extent.

# Summary Data:

time_* - told you some quantiles of page visiting duration

*_count - told you the count of certain action or state the visitor have during whole visiting. Say social_count is for the referral he had. Bags_count is the count of pages related to Bags, and Click_count the count for number of clicking on good pictures the visitor had.

price_* - told you some quantile of good prices the visitor took action on

just.view - a summary statistics telling you if the visitor is just viewing and have no actions.



