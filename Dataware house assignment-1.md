Design Data Warehouses For Given Below Products:
Note : While designing any Data Warehouse make sure to cover given below points.
a. Design Fact & Dimension tables
b. Create meaningful Primary & Foreign keys
c. Try to follow Star/SnowFlake Schema Design
d. Try to write few SQL queries to generate insightful business metrics (This is the critical
point because you need to understand the Data & Business both)

1. Design a Data Warehouse for IPL Cricket Tournament (Asked in Flipkart Interview for
Senior Data Engineer role)

a. Fact Table: Match Fact Table

Columns: match_id (Primary Key), date, venue, team1, team2, result, winning_team, player_of_the_match, stadium_id, etc.
b. Dimension Tables:

Team Dimension Table:
Columns: team_id (Primary Key), team_name, home_city, coach, captain, etc.
Player Dimension Table:
Columns: player_id (Primary Key), player_name, nationality, role, batting_style, bowling_style, team_id (Foreign Key), etc.
Venue Dimension Table:
Columns: stadium_id (Primary Key), stadium_name, city, capacity, etc.
Date Dimension Table:
Columns: date_id (Primary Key), date, day, month, year, etc.
c. Primary & Foreign Keys:

match_id will be the Primary Key in the Match Fact Table.
team_id will be the Primary Key in the Team Dimension Table.
player_id will be the Primary Key in the Player Dimension Table.
stadium_id will be the Primary Key in the Venue Dimension Table.
date_id will be the Primary Key in the Date Dimension Table.
Foreign Keys will establish relationships between the Fact and Dimension Tables.
d. Star Schema Design:

The Fact Table (Match Fact Table) is at the center, connected to various Dimension Tables (Team, Player, Venue, Date) through Primary and Foreign Keys.
e. SQL Queries for Business Metrics:

i) Total matches played in a specific season.


Total matches won by each team.
Total runs scored by a player in a season.
Average runs scored per match by a team.
Player with the most number of sixes in a season.

ii)Average runs scored per match in a specific season:

SELECT season, AVG(runs_scored) AS average_runs_per_match
FROM FactTable
GROUP BY season;

iii) Highest individual score by a player in a specific season:

SELECT season, player_name, MAX(individual_score) AS highest_score
FROM FactTable
GROUP BY season, player_name;

iv)Total wickets taken by each bowler in a specific season:

SELECT bowler_name, COUNT(wickets_taken) AS total_wickets
FROM FactTable
WHERE season = 'specific_season'
GROUP BY bowler_name;

v)Player with the most Player of the Match awards in a specific season:

SELECT player_name, COUNT(player_of_match) AS total_player_of_match
FROM FactTable
WHERE season = 'specific_season'
GROUP BY player_name;

2. Design a Data Warehouse for Food delivery app like Swiggy, Zomato (Asked in Grab
for Data Engineer role)

a. Fact Table: Order Fact Table

Columns: order_id (Primary Key), customer_id (Foreign Key), restaurant_id (Foreign Key), delivery_partner_id (Foreign Key), order_date, order_time, order_status, payment_method, etc.
b. Dimension Tables:

Customer Dimension Table:
Columns: customer_id (Primary Key), customer_name, phone_number, email, address, etc.
Restaurant Dimension Table:
Columns: restaurant_id (Primary Key), restaurant_name, cuisine_type, city, address, etc.
Delivery Partner Dimension Table:
Columns: delivery_partner_id (Primary Key), partner_name, vehicle_type, contact_number, etc.
Date Dimension Table:
Columns: date_id (Primary Key), date, day, month, year, etc.
c. Primary & Foreign Keys:

order_id will be the Primary Key in the Order Fact Table.
customer_id will be the Primary Key in the Customer Dimension Table.
restaurant_id will be the Primary Key in the Restaurant Dimension Table.
delivery_partner_id will be the Primary Key in the Delivery Partner Dimension Table.
date_id will be the Primary Key in the Date Dimension Table.
Foreign Keys will establish relationships between the Fact and Dimension Tables.
d. Star Schema Design:

The Fact Table (Order Fact Table) is at the center, connected to various Dimension Tables (Customer, Restaurant, Delivery Partner, Date) through Primary and Foreign Keys.
e. SQL Queries for Business Metrics:

i)Total number of orders placed in a specific city.
SELECT city, COUNT(order_id) AS total_orders
FROM FactTable
GROUP BY city;

ii) Average order value in a specific city:
SELECT city, AVG(order_value) AS average_order_value
FROM FactTable
GROUP BY city;

iii)Most popular cuisines ordered in a specific city:

SELECT city, cuisine_type, COUNT(order_id) AS total_orders
FROM FactTable
GROUP BY city, cuisine_type;

iv)Customer with the highest number of orders:

SELECT customer_id, COUNT(order_id) AS total_orders
FROM FactTable
GROUP BY customer_id;

v)Order cancellation rate in a specific city:

SELECT city, (COUNT(order_cancelled) / COUNT(order_id)) * 100 AS cancellation_rate
FROM FactTable
GROUP BY city;



3. Design a Data Warehouse for cab ride service like Uber, Lyft (Asked in Google for Data
Engineer role)

a. Fact Table: Ride Fact Table

Columns: ride_id (Primary Key), customer_id (Foreign Key), driver_id (Foreign Key), start_location, end_location, ride_date, ride_time, fare_amount, distance, duration, etc.
b. Dimension Tables:

Customer Dimension Table:
Columns: customer_id (Primary Key), customer_name, phone_number, email, etc.
Driver Dimension Table:
Columns: driver_id (Primary Key), driver_name, phone_number, license_number, etc.
Location Dimension Table:
Columns: location_id (Primary Key), location_name, latitude, longitude, etc.
Date Dimension Table:
Columns: date_id (Primary Key), date, day, month, year, etc.
c. Primary & Foreign Keys:

ride_id will be the Primary Key in the Ride Fact Table.
customer_id will be the Primary Key in the Customer Dimension Table.
driver_id will be the Primary Key in the Driver Dimension Table.
location_id will be the Primary Key in the Location Dimension Table.
date_id will be the Primary Key in the Date Dimension Table.
Foreign Keys will establish relationships between the Fact and Dimension Tables.
d. Star Schema Design:

The Fact Table (Ride Fact Table) is at the center, connected to various Dimension Tables (Customer, Driver, Location, Date) through Primary and Foreign Keys.
e. SQL Queries for Business Metrics:

i) Total number of rides completed in a specific city.

SELECT city, (COUNT(order_cancelled) / COUNT(order_id)) * 100 AS cancellation_rate
FROM FactTable
GROUP BY city;

ii) Average fare amount per ride.

SELECT AVG(fare_amount) AS average_fare
FROM FactTable;

iii) Most frequently visited locations by customers.
SELECT customer_id, location, COUNT(ride_id) AS ride_count
FROM FactTable
GROUP BY customer_id, location;

iv) Driver with the highest number of rides.
SELECT driver_id, COUNT(ride_id) AS ride_count
FROM FactTable
GROUP BY driver_id;

v) Total revenue generated per day.
SELECT DATE(ride_date) AS ride_date, SUM(f

4. Design a Data Warehouse for Restaurent table booking app like Dineout (Asked in
McKinsey for Consultant Data Engineer role)

a. Fact Table: Reservation Fact Table

Columns: reservation_id (Primary Key), customer_id (Foreign Key), restaurant_id (Foreign Key), reservation_date, reservation_time, party_size, status, etc.
b. Dimension Tables:

Customer Dimension Table:
Columns: customer_id (Primary Key), customer_name, phone_number, email, etc.
Restaurant Dimension Table:
Columns: restaurant_id (Primary Key), restaurant_name, cuisine_type, city, address, etc.
Date Dimension Table:
Columns: date_id (Primary Key), date, day, month, year, etc.
c. Primary & Foreign Keys:

reservation_id will be the Primary Key in the Reservation Fact Table.
customer_id will be the Primary Key in the Customer Dimension Table.
restaurant_id will be the Primary Key in the Restaurant Dimension Table.
date_id will be the Primary Key in the Date Dimension Table.
Foreign Keys will establish relationships between the Fact and Dimension Tables.
d. Star Schema Design:

The Fact Table (Reservation Fact Table) is at the center, connected to various Dimension Tables (Customer, Restaurant, Date) through Primary and Foreign Keys.
e. SQL Queries for Business Metrics:

i) Total number of reservations made in a specific city.
SELECT city, COUNT(reservation_id) AS total_reservations
FROM FactTable
GROUP BY city;

ii) Average party size per reservation.
SELECT city, AVG(party_size) AS average_party_size
FROM FactTable
GROUP BY city;

iii) Popular cuisine types in a city.

SELECT city, cuisine_type, COUNT(reservation_id) AS total_reservations
FROM FactTable
GROUP BY city, cuisine_type;

Customer with the highest number of reservations.
iv) SELECT customer_id, COUNT(reservation_id) AS total_reservations
FROM FactTable
GROUP BY customer_id;

v) Reservation status distribution.

SELECT status, COUNT(reservation_id) AS reservation_count
FROM FactTable
GROUP BY status;


5. Design a Data Warehouse for Covid Vaccination Application (Asked in Livsapce for
Data Engineer role)

a. Fact Table: Vaccination Fact Table

Columns: vaccination_id (Primary Key), patient_id (Foreign Key), vaccine_id (Foreign Key), vaccination_date, vaccination_time, location, dose_number, side_effects, etc.
b. Dimension Tables:

Patient Dimension Table:
Columns: patient_id (Primary Key), patient_name, age, gender, contact_number, address, etc.
Vaccine Dimension Table:
Columns: vaccine_id (Primary Key), vaccine_name, manufacturer, dosage_interval, etc.
Location Dimension Table:
Columns: location_id (Primary Key), location_name, city, address, etc.
Date Dimension Table:
Columns: date_id (Primary Key), date, day, month, year, etc.
c. Primary & Foreign Keys:

vaccination_id will be the Primary Key in the Vaccination Fact Table.
patient_id will be the Primary Key in the Patient Dimension Table.
vaccine_id will be the Primary Key in the Vaccine Dimension Table.
location_id will be the Primary Key in the Location Dimension Table.
date_id will be the Primary Key in the Date Dimension Table.
Foreign Keys will establish relationships between the Fact and Dimension Tables.
d. Star Schema Design:

The Fact Table (Vaccination Fact Table) is at the center, connected to various Dimension Tables (Patient, Vaccine, Location, Date) through Primary and Foreign Keys.
e. SQL Queries for Business Metrics:

i) Total number of vaccinations administered in a specific location.
SELECT location, COUNT(vaccination_id) AS total_vaccinations
FROM FactTable
GROUP BY location;

ii) Vaccination rate per day/week/month.
SELECT DATE(vaccination_date) AS vaccination_date, COUNT(vaccination_id) AS daily_vaccinations
FROM FactTable
GROUP BY DATE(vaccination_date)
ORDER BY DATE(vaccination_date);

iii) Popular vaccines used.
SELECT vaccine_id, COUNT(vaccination_id) AS vaccine_count
FROM FactTable
GROUP BY vaccine_id;

iv) Patient demographics (age, gender) for vaccinations.

SELECT age_group, gender, COUNT(vaccination_id) AS vaccination_count
FROM FactTable
GROUP BY age_group, gender;

v) Adverse reactions to vaccines reported.
SELECT side_effects, COUNT(vaccination_id) AS side_effects_count
FROM FactTable
GROUP BY side_effects;

