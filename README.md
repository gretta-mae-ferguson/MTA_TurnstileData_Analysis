# MTA_TurnstileData_Analysis

Exploratory Data Analysis: New York City Subway Traffic and Demographic
We hit the ground running in our first week at the Metis Data Science Bootcamp!
We had a pretty tight timeframe for our first project! It was assigned on Monday, with a due date of Friday.

We were given a scenario in which a ficticious non-profit company WomenTechWomenYes (WTWY) had asked us to perform some  EDA to explore MTA turnstile data in NTC. WTWY want to send out volunteer teams out to subway stations to promote their summer gala to increase increase their brand awareness, participation, and potentially increase donations.They are also interested in collecting email addresse.The deliverable for this scenario was to provide recommendations on where to send WTWY's volunteer teams.

Our Approach
Our strategy to provide valuable recommendations involved finding the top subway stations with respect to foot traffic, and then verifying that the population in the surrounding areas held demographics that could place them in WTWY's target audience.

**Need to complete**
In order to do this, we used data from the NYC MTA to analyze pedestrian traffic acros the NYC subway system. We also incorporated census data from the American Community Survey to analyze demographics,tech data and...

Data
Turnstile Usage Data - Spring2018 data
The dataset we used for station traffic involved records for the months March 2018 to May 2018, and can be found here. This source also provides a useful overview of the data, as well as a data dictionary.

This dataset contained the following:

C/A, Unit and SCP: Unique identifiers for turnstiles
Station, Linename and Divison: Information for each station
Date, Time, Desc: temporal data and notes for each sample
Entries and Exits: Number of pedestrians entering and exiting subway stations

Data Cleaning!

We encountered the following issues:

The samples were on an individual turnstile level, rather than for individual stations
The samples  cumulative across time
Some turnstiles were defective, meaning they'd reset randomly, subtract values and sometimes send the same record twice

We addressed the issues as follows:

Aggregating individual turnstile traffic for each station
Aistributing traffic across days of the week  per station
Filtering for outliers ( discarding negative values and values above a certain limit)

MTA Turnstile Data Findings
After making our data relatively clean, we analyzed the top stations by traffic.We calculated an absolute total for subway users by adding the number of entrances and exits for each station together, to get an absolute total.

We found that the top stations were in central Midtown Manhattan, and were all major hubs. The top 20 stations according to our analysis are shown below:

Top 20 Stations, 2016

Once we had an idea of our top performers, we decided to zoom in and look at traffic at each of the top 4 stations. They had very similar distributions:


Each of the top stations has a spike in subway users on Tuesday and Thursday. W observed that this was consistent across all of the stations in the subway system. This either points to an actual spike in traffic, or (more likely) some further data cleaning that we should do.

Since we were working on a very tight timeframe, we decided to use our daya as it is.

Our observations from the graph are as follows:

spikes occur on Tuesdays and Thursdays
dips occur on weekends





We would have done the following if we had a little more time:

As I said earlier, this project was done on a pretty tight timeframe, and there was a lot more that we could have done!

A few things that would be next steps in this analysis are:

dig a bit deeper in terms of outliers
investigate the March spike,
look into the missing records in June,
try different filter values
analyze traffic data for temporal trends
seasonal
weekday/weekend
time of day
create a demographic 'scorecard' for each station, so that we can better prioritize our recommendations
