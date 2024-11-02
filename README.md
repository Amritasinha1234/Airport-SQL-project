# Airport-SQL-project

![logo](https://github.com/Amritasinha1234/Airport-SQL-project/blob/main/images.jpeg?raw=true)


The SQL project will analyze the Airport Data to identify the key factors such as airport operations by examining total passenger numbers and trends per route, average passengers per flight.

## objective
The SQL project will analyze the Airport Data to identify the key factors such as airport operations by examining total passenger numbers and trends per route, average passengers per flight, flight frequency. It will compare passenger numbers across origin cities, access available seats, and identify popular destination airports. Additionally, the project will explore correlations between city population and passenger counts, as well as the impact of population size on flight frequency.

## Business Problems and Solutions

## Problem Statement 1 :
 The objective is to calculate the total number of passengers for each pair of origin and destination airports.
 ```sql
SELECT 
    Origin_airport,
    Destination_airport,
    SUM(Passengers) AS Total_Passengers
FROM
    airports2
GROUP BY Origin_airport , Destination_airport
ORDER BY Origin_airport , Destination_airport;
```
