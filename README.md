# GoBike-SystemData-Analysis
## by Victoria Perez Mola

## Introduction
Bay Wheels's trip data Analysis using Jupyter Notebook.


## Dataset
The dataset chosen to perform the analysis is the [Ford GoBike System Data](https://www.lyft.com/bikes/bay-wheels/system-data).
This data set includes information about individual rides made in a bike-sharing system covering the greater San Francisco Bay area.
* Trip Duration (seconds)
* Start Time and Date
* End Time and Date
* Start Station ID
* Start Station Name
* Start Station Latitude
* Start Station Longitude
* End Station ID
* End Station Name
* End Station Latitude
* End Station Longitude
* Bike ID
* User Type (Subscriber or Customer – “Subscriber” = Member or “Customer” = Casual)

### Data Wrangling 
- fields start_time and end_time changed to datetime
- start_station_id and end_station_id changed tocategorical variables
- user_type should changed to category value: Suscriber, Customer
- Creatin of columns to store the start time hour, start time day of the week and start time month

## Summary of Findings
After recolecting the data and performing a data exploration, these are the main findings:

* The majority of the rentals occur at peak times (8am and 5pm) and during weekdays
* During weekends the peak tends to be less pronounced and most rentals take place between 1 and 3 pm
* Although the amount of rentals is not stable along the year, there's no clear seasonal impact on it
* On average people ride 13 min, this varies between weekdays and weekends, being slightly longer over the last ones
* The suscriber demad is high during the weekdays but has a huge decrease during weekends
* The casual customer demand is more stable, yet it increases during weekends. 

In the first part, I'll use Python visualization libraries to systematically explore a dataset, starting from plots of single variables and building up to plots of multiple variables. 

In the second part, I'll produce a short presentation that illustrates interesting properties, trends, and relationships discovered in the dataset. The primary method of conveying the findings will be through transforming your exploratory visualizations from the first part into polished, explanatory visualizations.

## Key Insights for Presentation

There are two clear patterns of behaviour among the users. Subscribers use the system heavily on working days and during peak times.
On the other side, customers have a more steady demand over the week, but it increases during the weekend. 
Combined with the big decrease of the suscriber's demand, the customers represent a great share of the total rides that take place during Saturday and Sunday. 
Customers also tendo to use the bikes along the day, mostly around noon during the weekends rather that two pronounced peaks as seen in the working days. 

While suscribers seem to be using the bikes for work commute, customers use it for leisurepurposes. 