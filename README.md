# Ford GoBike: Insights on Users' Behaviour
### by Ana Júlia Bellini

Ford GoBike is a bike-sharing system covering the San Francisco Bay Area metropolitan region.

This project aims **to explore and visualise data** from trips made by customers of this system during February 2019, looking for patterns and insights into user behaviour while putting into practice the teachings of Chapter 5 of Udacity's Data Analyst Nanodegree regarding data visualisation.

## Dataset

Our original dataset consisted of about **180k trips recorded in February 2019 around the greater San Francisco Bay area**, including start and end times, member's gender, birth year, user type, and other attributes. After the preliminary wrangling step, around 8k records were discarded due to missing data or filtered-out members based on their birth year (only members born after 1922 remained). I also ran a Feature Engineering process, creating variables with information on the start hour, weekday, member's age and generation.

I started analysing the distribution of trip durations, where we found outliers related to trips lasting more than one hour. From this point onwards, much of the exploration focused on understanding the users' behaviour in these two scenarios.

## Summary of Findings

In the big picture, we have some interesting findings:

- About 99% of the trips lasted less than an hour, with an average of 11 minutes.
- Most of the trips were made by subscribers on workdays (from Monday to Friday), especially during rush hours, suggesting users prefer using Ford GoBike services for their commuting needs.
- There's a prevalence of Millennials, born between 1984 and 1986.
- 74% of the trips were made by clients who identify as male, 23% were by females, and only 2% of the trips were by non-binary users.
- In 90% of the trips, the clients needed another means of transportation, and every trip with a bike marked as the single mean was made by subscribers.
- All trips spread across San Francisco, Berkeley, Oakland, San Jose, and nearby areas. Out of the five most popular start stations, three of them are public transport stations, and two of the most popular end stations, Market St and Ferry Building, are famous San Francisco tourist attractions.
- The younger the client, the later they like to go out on a bike ride, and the lower the average duration.
- The older the clients, the more they prefer subscriptions over one-time use.

When we took a closer look at the longer trips (1+ hour), we found different characteristics:

- 75% lasted between 1 and 3 hours, and most of them happened on weekends, during the afternoon.
- Customers had a stronger presence on longer trips, especially on the weekends, suggesting several people enjoy GoBike services more as weekend plans. Most of these customers are Millennials or Gen Z-ers.
- 75% of customers' long trips started before 3 pm, while more subscribers went out usually after 3 pm.

Out of these findings, our presentation will focus on the effects of weekdays, generations, and user types over start hours and trip duration.

## Key Insights for Presentation

We learned Ford GoBike was broadly used for commuting purposes by its subscribers, while also being an option for weekend plans, especially for customers on longer trips.

We also found out the older the member, the sooner they prefer to leave for their bike rides, and the more they preferred subscriptions over one-time use. Focusing on engaging younger users could be a great opportunity to grow Ford GoBike's market presence.

Our exploration clearly showed us how members' ages, user types and weekdays can greatly impact when the trips start and how long they last, so the idea is to focus our presentation on conveying these aspects.

When plotting this information for the public, I chose neutral colours to try and keep colourblind people from misunderstanding the conveyed message. I also took special care with titles and labels, seeking the highest data-ink ratio possible and allowing the public to focus on what really matters. Some of our plots have additional filters as well, to make the data even easier to read and interpret, such as members' ages being limited to 60 years old.

## References

- [Folium 0.12.1 documentation](https://python-visualization.github.io/folium/)
- [Interactive Maps, a tutorial from a Kaggle course](https://www.kaggle.com/alexisbcook/interactive-maps)
- [seaborn documentation (used for methods like `despine` and others)](http://seaborn.pydata.org/)
- [pandas documentation](https://pandas.pydata.org/docs/)
- [Generations by birth year](https://www.beresfordresearch.com/age-range-by-generation/)
- [Converting seconds into minutes](https://www.geeksforgeeks.org/python-program-to-convert-seconds-into-hours-minutes-and-seconds/)
- [Getting day names](https://www.geeksforgeeks.org/python-pandas-series-dt-day_name/)
- [Matplotlib documentation](https://matplotlib.org/stable/index.html)
- [Removing labels from subplots](https://stackoverflow.com/questions/25124143/matplotlib-subplots-get-rid-of-tick-labels-altogether)
- [Annotations on seaborn's countplot](https://stackoverflow.com/questions/63745343/annotate-percentage-of-group-within-a-seaborn-countplot)
- [Calculating correlations between dates and numeric variables](https://stackoverflow.com/questions/48242555/correllation-pandas-between-date-and-integer-timeseries)