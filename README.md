# Bike-share-dataset-analysis

In this case study I investigate the user habits of a bike-sharing application.

## Dataset description

This bike-share program features more than 5,800 bicycles and 600
docking stations. Until now, the program’s marketing strategy relied on building general awareness and appealing to
broad consumer segments. One approach that helped make these things possible was the
flexibility of its pricing plans: single-ride passes, full-day passes, and annual memberships.
Customers who purchase single-ride or full-day passes are referred to as casual riders.
Customers who purchase annual memberships are members.

The program's finance analysts have concluded that annual members are much more profitable
than casual riders. Rather than creating a marketing campaign that targets all-new customers, the managers believes
there is a solid opportunity to convert casual riders into members.

For this, the manager has set a clear goal: Design marketing strategies aimed at converting casual riders into
annual members.

### Data Source

[Doc: link to the original dataset.](https://divvy-tripdata.s3.amazonaws.com/index.html)

## Goal

For this time, I investiage the data from one aspect: How do annual members and casual riders use shared bikes differently?

I have set up the following series of questions:
- 1 Are there more member or casual riders?
- 2 What type of bikes do member and casual riders use?
- 3 Location analysis - Do the user habits of member and casual riders differ by location?
    - Most important start and end locations for member and casual riders
- 4 Time trend analysis - Are there time trend in the bike usage? Is yes, do the member and casual rider habits differs?
    - Monthly period
    - Weekly period
        - Calculate the average for users by day_of_week
        - Calculate the average for users by weekdays and weekend days
- 5 Ride length analysis
    - Calculate the average ride_length for member and casual riders
    - Do the member and casual ride lengths differs?

## Implementation

I've implemented the entire analysis in Python.

## Key findings and conclusion

- Overview analysis
    - There are more member riders than casual riders
- Bicycle type analysis
    - Members chooses electric and classic bikes in equal ratio
    - Casual riders more likely to choose electric bikes
    - Docked type bikes are not significant
- Location analysis
    - No clear separation between the start and end locations of the different groups
    - No straightforward trend
    - The central places are more frequented, there are more rides
- Monthly time trend analysis
    - There are time trend but that do not provide useful information
    - Ride number increases in summer
    - The change between the member-casual riders is nearly equal
- Ride length analysis
    - Average ride length: 
    - Casual rider's ride length is 8 minutes longer than member riders
    - The member's ride length is consistent during a week, while casual's ride length is higher around the weekend
- Weekly time trend analysis
    - The total number of rides during a week is nearly constant
    - The member rides decreases at the end of a week, while the casual rides increases at the end of a week and it peeks at saturdays. The member rides peeks at wednesday and thursday.
    - The number of member riders on weekdays is twice as high as the number of casual riders
    - The number of member and casual riders are nearly the same at weekends


