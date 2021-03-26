# (US Flights 2018 Dataset)
## by (Islam M. Saad)

## Dataset
Using US Flights 2018 Dataset - source: https://www.kaggle.com/zernach/2018-airplane-flights
You can find it at Google Drive link:
https://drive.google.com/file/d/1Q67HaB1FZJBQm_u_HhxSHX0mHgpWgUge/view?usp=sharing
This Dataset contains 7.2M records and 28 columns
Due to huge dataset size, We will select subset (random sample) of 10% of dataset 
Variables Descriptions:
=======================
1	DATE
2	DepTime	actual departure time (local, hhmm)
3	CRSDepTime	scheduled departure time (local, hhmm)
4	ArrTime	actual arrival time (local, hhmm)
5	CRSArrTime	scheduled arrival time (local, hhmm)
6	UniqueCarrier	unique carrier code
7	FlightNum	flight number
8	TailNum	plane tail number
9	ActualElapsedTime	in minutes
10	CRSElapsedTime	in minutes
11	AirTime	in minutes
12	ArrDelay	arrival delay, in minutes
13	DepDelay	departure delay, in minutes
14	Origin	origin IATA airport code
15	Dest	destination IATA airport code
16	Distance	in miles
17	TaxiIn	taxi in time, in minutes
18	TaxiOut	taxi out time in minutes
19	Cancelled	was the flight cancelled?
20	CancellationCode	reason for cancellation (A = carrier, B = weather, C = NAS, D = security)
21	Diverted	1 = yes, 0 = no
22	CarrierDelay	in minutes
23	WeatherDelay	in minutes
24	NASDelay	in minutes
25	SecurityDelay	in minutes
26	LateAircraftDelay	in minutes
27	Un-named column will be removed

## Summary of Findings

> * As Numerical Variables, we can find out that the most flights elapsed time in minutes normally distributed around 80-200 and there are outliers then we will use xlimit to elliminate the outliers that leads to right skwed. Moreover, we find out Flights distance average is 630 miles and 75% quartile are 1036 miles and then we xlimit the plot to hide outliers. We provides bar charts for Origin & Destination Airports and US flight Carriers.
> * We find out 'CANCELLED' flights, which are out of our interest then we clean out the selected dataset to include only Non-cancelled Flights. As we have 357 ORIGIN/DEST airports then we will graph the top 20 and then we will focus on top 6 Which are ATL, ORD, DFW, DEN, CLT, LAX Airports. Additionally, we choose Top5 OP_CARRIERS. Additionally, We can conclude that Southwest Airlines is the largest number of flights in 2018 by 18% of the total flights and we can explore that Delta Airlines, American Airlines, SkyWest Airlines, United Airlines took about 45% of flights. Therefore, we can see that Top 5 Airlines carriers took about 63% of US flights in 2018. Then we will focus on Top 5 in later analysis.
> * We can see that SkyWest Airlines provides many flights of distance below 1000 miles and we can see the Top carrier provides 75% of its flights for distance equal or less than 100 miles. Furthermore, we can conclude the carriers which concentrate on large distance flights made small number of flights around US in 2018. and we can see some outliers for greater than 2000 miles flights for Top3 carriers.
> * We can findout Actual Elapsed Time of flight is proportional linearly with Distance in Miles
> * ATL are the most DEST Airport flights lunches by Delta Airlines op_carrier.
> * We can find that linear relationship and postive correlation and also we can conclude that very small delays are the most affected for the majority of flights as we see the high density color(600,000 flights) around zero.
> * We can see that August is the biggest total delay in 2018 that may be because the biggest number of flights were in August. we can see also the same trend in Arrival & Departure total delays. Furthermore, we can see Arrival delays are larger than departure delays alwyas over 2018 months.
> * We can find out that highly correlation between (ARR_DELAY, DEP_DELAY) , (DISTANCE,ACTUAL_ELAPSED_TIME), (ARR/DEP_DELAY, CARRIER_DELAY/LATE_AIRCRAFT_DELAY).
> * We can find out that Delta Airlines & United Airlines made long distant trip that took large Elapsed time as well. That makes sense as Distance & Actual Elapsed Time are postively correlated.
> * We can find out that Arrival Delay & Departure Delay is very small for long average distant trips (more than 2000 Miles). We can also see small distant flight trip took larger delay tahn medium distant trips.
> * e can find out that Delta Airlines made minimum Departure delay at ATL Airport. Furthermore, Delta Airlines & SkyWest Airlines made maximum Departure delay at ORD Airport.


## Key Insights for Presentation

> * We can conclude that we have 239,738 delayed flights due to Arrival delay which is 35.63% of total flights in our sample.
> * We can conclude that we have 232,385 delayed flights due to Departure delay which is 34.54% of total flights in our sample 
> * We can conclude that Southwest Airlines is the largest number of flights in 2018 by 18% of the total flights and we can explore that Delta Airlines, American Airlines, SkyWest Airlines, United Airlines took about 45% of flights. Therefore, we can see that Top 5 Airlines carriers took about 63% of US flights in 2018. Then we will focus on Top 5 in later analysis.
> * We can find that linear relationship and postive correlation and also we can conclude that very small delays are the most affected for the majority of flights as we see the high density color(600,000 flights) around zero.
> * We can see that August is the biggest total delay in 2018 that may be because the biggest number of flights were in August. we can see also the same trend in Arrival & Departure total delays. Furthermore, we can see Arrival delays are larger than departure delays alwyas over 2018 months.
> * We can find out that Arrival Delay & Departure Delay is very small for long average distant trips (more than 2000 Miles). We can also see small distant flight trip took larger delay tahn medium distant trips.