# Ford Go Bike Data Exploration
## by Robert Kimani Chege


## Dataset

This data includes information about approximately 183,000 individual bike rides made in a bike-sharing system covering the greater San Francisco Bay area. The dataset consists of properties of the individual bike rides ranging from trip duration in seconds, trip start stations, end stations, usertpes, bike-shares involved among others. The dataset can be downloaded from [here](https://video.udacity-data.com/topher/2020/October/5f91cf38_201902-fordgobike-tripdata/201902-fordgobike-tripdata.csv).<br>
Some of the steps in my data exploration process include:
- Wrangling my dataframe, this included dropping rows with missing values, changing data types start and end time for the trips to datetime, extracting age of members, dropping columns with invalid ages that is above 95 years and dropping columns unnecessary for my analysis.
- Univariate explorations. Here I focused on the distribution of trip duration, member age, user types, genders, bike shares and common start and end stations.
- Bivariate explorations. Here, I focused on relationships such as age with trip duration, gender with trip duration, user type with trip duration, bike shares with trip duration, bike share with age, user type with age, user type with bike share and user type with gender.
- Multivariate explorations. Here, I focused on the distribution of user types, bike shares and gender in the correlation of trip duration with age and the distribution of user types and bike shares in the realtionship of age with trip duration.

## Summary of Findings
From my exploration, I found out that trips taking long durations are less frequent with the most frequent trips being averagely 500 seconds. Participants in these bike trips are mostly between 20 to 45 years with the highest number being in their mid 30's. It's interesting that the most common start staions are also the most common end stations. Among the user types, subsribers are the majority being approximately 90% and the rest are customers. Majority are of the male gender, followed by female then the other genders. 90% of the members do not share their bikes, however it's interesting that they also spend the longest time in their trips. Those sharing their bikes are only subscribers and likely to be in the age bracket 20 to 30 years. The other gender has a record of longer trip durations as compared to the male and female genders.<br>
To arrive at my summary findings I employed plots from univariate to bivariate to multivariate. I plan to bring the more conclusive bivariate and multivariate explorations to my explanatory presentation.

## Key Insights for Presentation

My key insights for presentation include:
- Customers are not involved in bike sharing for all the trips. I will show this using a count plots showing number of customers and subscribers for both bike share categories.
- Majority of the members sharing their bikes are inclined towards short duration trips. This is shown in a correlation between trip duration and member age for both bike share levels.
- Across all genders those not involved in bike sharing have the longest durations. It is also key to note that the other gender averagely spends more time in their trips, followed by females then males.It is also important to note that among the male and female genders, there's an almost equal level in trip duration for both bike share levels while for the other gender those who do not share bikes take significantly more time in their trips. I use seaborn's pointplot function to demonstrate this.
- Across all genders customers spend quite a significant amount of time in their trips. The trend of the other gender having the longest durations, followed by female then male is also evident. I also demonstrate this using seaborn's pointplot function.
