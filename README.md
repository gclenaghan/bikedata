a3-nkullman-gclenagh
===============

## Team Members

1. Nick Kullman nkullman@uw.edu
2. Graham Clenaghan clenagh@math.washington.edu

## Bike Activity on the Fremont Bridge

### Visualization
- Visualization shows records of cyclist counts across the Fremont Bridge.
- Records from each calendar day are mapped to two lines on the visualization showing northbound and southbound counts at each hour.
- Sliding brushes allow the viewer to select a subset of daily records according to specific values of the following:
  - Max temperature
  - Daily precipitation
  - Day of the year
- Viewers can choose between weekdays/weekends through use of a radio button.
- Visualization reports number of days currently shown in gray area beneath the bank of controls.
- Emphasized lines show hourly counts for all days in the viz aggregated by date for each direction of cyclist traffic.
- Hovering over a non-aggregate line displays the day's date, maximum temperature, and amount of precipitation

### Dataset
- Two primary data sources for this assignment:
  1. Fremont Bridge bicycle count data from the City of Seattle[(https://data.seattle.gov/)](https://data.seattle.gov/)
  2. Weather data from [WeatherUnderground](http://www.wunderground.com/)
- Bike data are hourly counts of cyclists heading NB and SB on both sides of the Fremont Bridge in Seattle, WA from October 2012 - April 2015.
- Weather data are daily aggregates of a number of meteorological variables over the same time span.
- Datasets were merged, pared down, and modified. Tuples in the final dataset following format:
|""|"Date"|"Time"|"Direction"|"CyclistCount"|"IsWeekday"|"Max_TemperatureF"|"PrecipitationIn"|"daynum"|
|----|----|----|----|----|----|----|----|----|
|1|2012-10-02|0|"NB"|0|TRUE|63|0|275|
 
<!--- (Put a brief description of your final interactive visualization application and your dataset here.) --->


## Running Instructions

<!--- Put your running instructions here. (Tell us how to run your visualization.) --->

You can access our visualization at [http://cse512-15s.github.io/a3-nkullman-gclenagh/](http://cse512-15s.github.io/a3-nkullman-gclenagh/) or download this repository and run `python -m SimpleHTTPServer 9000` and access this from http://localhost:9000/.

Within the visualization, you have the following interactivity controls at your disposal:
- A brush to select a range of maximum daily temperatures
- A brush to select a range of daily precipitation amounts
- A brush to select a range of calendar days
- A radio button to select only weekdays or weekends
Any time a selection is made with these controls, the visualization is updated to show only those days matching the criteria


## Story Board

Put either your storyboard content or a [link to your storyboard pdf file](storyboard.pdf?raw=true) here. Just like A2, you can use any software to create a *reasonable* pdf storyboard.


### Changes between Storyboard and the Final Implementation

A paragraph explaining changes between the storyboard and the final implementation.


## Development Process

Include:
- Breakdown of how the work was split among the group members. 
- A commentary on the development process, including answers to the following questions: 
  - Roughly how much time did you spend developing your application?
  - What aspects took the most time?