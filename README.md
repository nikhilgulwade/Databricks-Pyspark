# Flight Data analysis in Pyspark

Below are the reports we created -

● Total number of flights by airline and airport on a monthly basis
● On-time percentage of each airline for the year 2015
● Airlines with the largest number of delays
● Cancellation reasons by airport
● Delay reasons by airport
● Airline with the most unique routes

#Data Dictionary -

#Airlines Data Set

Data Entity Airlines
File Name airlines.csv (single data file)
Description Airline codes and names
Airline Data Set Data Structure
Column Name Data Type Description
IATA_CODE String Airline Identifier/Code
AIRLINE String Airline name


#Airports Data Set

Data Entity Airports
Location airports.csv (single data file)
Description Airport codes, names, and locations
Airport Data Set Data Structure
Column Name Data Type Description
IATA_CODE String Airport identifier/Code
AIRPORT String Airport name
CITY String City where the airport is located
STATE String State where the airport is located
COUNTRY String The country where the airport is located
LATITUDE Number Latitude of the airport
LONGITUDE Number Longitude of the airport


#Flights Data Set

Data Entity Flights
Location flights/partition-x.csv (multiple files)
Description Flight Records
Flight Data Set Data Structure
Column Name Data Type Description
YEAR Number Year of the flight
MONTH Number The month of the flight
DAY Number The day of the flight
DAY_OF_WEEK Number Day of the week of the flight
AIRLINE String Airline identifier
FLIGHT_NUMBER String Flight identifier
TAIL_NUMBER String Aircraft identifier
ORIGIN_AIRPORT String Starting airport
DESTINATION_AIRPORT String Destination airport
SCHEDULED_DEPARTURE String Planned departure time
DEPARTURE_TIME String Wheels uptime
DEPARTURE_DELAY Number Total delay on departure
TAXI_OUT Number The time duration elapsed between departure
from the origin airport gate and wheels off
WHEELS_OFF String The time point that the aircraft's wheels leave
the ground
SCHEDULED_TIME Number Planned time amount needed for the flight trip
ELAPSED_TIME Number Total trip time
AIR_TIME Number The time duration between wheels_off and
wheels_on time
DISTANCE Number The distance between two airports
WHEELS_ON Number The time point that the aircraft's wheels touch
on the ground
TAXI_IN Number The time duration elapsed between wheels-on
and gate arrival at the destination airport
SCHEDULED_ARRIVAL Number Planned arrival time
ARRIVAL_TIME String Time of arrival
ARRIVAL_DELAY String Arrival time - Scheduled Arrival
DIVERTED Number Aircraft was diverted
CANCELLED Number Aircraft was canceled
CANCELLATION_REASON String Reason for Cancellation of flight: A -
Airline/Carrier; B - Weather; C - National Air
System; D - Security
AIR_SYSTEM_DELAY Number Delay caused by the air system
SECURITY_DELAY Number Delay caused by security
AIRLINE_DELAY Number Delay caused by the airline
LATE_AIRCRAFT_DELAY Number Delay caused by the aircraft
WEATHER_DELAY Number Delay caused by weather
