# Bike Share Analysis with Ford GoBike Data 
## by Nathania Yuliani

[Ford GoBike](https://www.fordgobike.com/) is a bike share system located in the Bay Area, more specifically in San Francisco, East Bay, and San Jose. With 7,000 bikes distributed across those 3 regions, customers have the feasibility to unlock bikes from one station and return to any other station in the system, making them ideal for one-way trips. The bikes are available for use 24 hours/day, 7 days/week, 365 days/year and riders have access to all bikes in the network when they become a member through a monthly or yearly subscription or purchase a single ride or 24-hour pass.

## Dataset

This project used the Ford GoBike's trip data available in their [website](https://www.fordgobike.com/system-data).

I extracted trip data for the whole year of 2018 and compiled them together into 1 dataframe. Originally the compiled data contained 1,863,721 rows and 16 columns, but after cleaning the data, I ended up with the same number of rows, but only 11 columns.

- Trip Duration (seconds)
- Start Time and Date
- End Time and Date
- Start Station ID
- Start Station Name
- End Station ID
- End Station Name
- Bike ID
- User Type (Subscriber or Customer – “Subscriber” = Member or “Customer” = Casual)
- Member Year of Birth
- Member Gender

## Prerequisites

Before running the codes, you will need to install these:

- Anaconda
- Python (Minimum 3)
- Pandas
- Numpy
- Matplotlib
- Seaborn

## Python Notebook and Scripts

gobike_exploration.ipynb - Main project file, a IPython Notebook that contains the analysis for the project.
gobike_slide_deck.ipynb - This IPython Notebook contains starter cells to help organize the slide deck deliverable.

## Summary of Findings

1. In 2018, the average trip duration that the users took was around 10 minutes. The trips were mostly in Summer season (between June - August) and most trips were taken by males. 85% of the total trips were taken by Subscribers, which are members of the GoBike program. Also, the age group with the most trips was between 30-35 years old.
2. There was no significant difference between the seasons and the trip duration, but there was a low durations in Fall season due to the bad air quality caused by Northern California wildfires in November 2018.
3. The Customers users (casual users) usually took more time in their rides than Subscribers.
4. All gender types (male, female, other) with age range of 10-20 took the longest trip duration in average and surprisingly, in the male and female categories, age range of 50-60 took the second longest trip duration.

## Key Insights for Presentation

For the presentation, I display the influence of variables in question (season of year, user type, user age and gender) on the Users' GoBike trip duration. I start by introducing the duration variable and followed by the main variable in question, season.

Afterwards, I introduce each of the relationship one by one. To start, I use the bar plots of duration and season to show that Summer season does have the longest trip duration. Then, I do violin plots of duration and user type. I'm only looking at
the trip duration of less than 60 minutes here, to focus the analysis. The other two variables, age and gender, are covered afterwards, using bar plots. I've made sure to use different color for each age group to make sure it is clear that they're different between bars.