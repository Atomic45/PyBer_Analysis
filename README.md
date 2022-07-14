# PyBer_Analysis

## Overview of the Analysis
The purpose of the Pyber Analysis is to outline the ride-sharing data by city type to present to V.Isualize for decision making strategies. The analysis will include total number of rides, drivers and average fares by the following city types:

- Urban
- Suburban
- and Rural

This analysis will include plotting a multi-line chart to give visualization of the total fares for each week by city type. 

## Results
The project began with reviewing the total of rides, drivers, and fares for each city type as shown below. This shows that the Urban city type had the most rides, drivers and total fare amount. 
![image](https://user-images.githubusercontent.com/30300621/178994134-7522740d-c74d-4196-8bdf-76158f839991.png)

The dataframes created led to the following table showing the items listed above and includes the Average Fare per Ride, and Average Fare per Driver. 
![image](https://user-images.githubusercontent.com/30300621/178994733-5f438bf4-39a2-4ad8-9922-cd5f83e987c5.png)

The next steps include using the groupby() function to include the date information, such as time stamps and types of date format. The pivot() functoin was used to get the total fares for each city type by the date as shown below. 
![image](https://user-images.githubusercontent.com/30300621/178995699-ebe3d862-339e-42d8-9efa-bfa666aa6661.png)

The pivot and loc function were used together to filter the date range 01/01/2019 to 4/29/2019. This is necessary for the next steps that inlcude the resample() function to make the datatype for the index to datetime as shown below. 
![image](https://user-images.githubusercontent.com/30300621/178997006-43edcbcc-04b8-412d-9152-4927ad3be2ae.png)

With the resample() function, a new DataFrame is created, which provides the sum of the fares for each week. 
![image](https://user-images.githubusercontent.com/30300621/178997323-df2fdeac-36cc-481a-9a54-0e1dcd475f82.png)

With the analysis complete, the results can be plotted by using the object oriented interface method. A multi-line chart is created to show all 3 city types with the fare amount for each month. The line graph for each city types shows data from 01/01/2019 to 04/29/2019, with an angle point for each week. 

- The Urban city type shows the most Fare amounts. 
- The Suburban city type shows comes in at 2nd for most Fare amounts
- The Rural city type shows the least Fare amounts. 

![image](https://user-images.githubusercontent.com/30300621/178999347-51558f7a-7908-492c-905f-7a1fcc8fdea6.png)


## Summary
There is a statement summarizing three business recommendations to the CEO for addressing any disparities among the city types
