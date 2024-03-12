# Hotel_Booking_Analysis_EDA
# Obejctive
The City Hotel and Resort Hotel have seen significant cancellation rates in recent years. As a result, every hotel is currently dealing with a variety of problems, such as decreased sales and poor accommodations. Therefore, reducing cancellation rates is the main objective for both hotels in order to boost their revenue-generating efficiency and for us to provide business assistance to solve this issue.
The primary topics of this research are the analysis of hotel booking cancellations along with other elements that don't affect their business or annual revenue generating.
# Tools Used
- Jupyter Notebook
- Python Programming Language
# About Dataset
This dataset contains 119390 observations for a City Hotel and a Resort Hotel. Each observation represents a hotel booking between the 1st of July 2015 and 31st of August 2017, including booking that effectively arrived and booking that were canceled.

Since this is hotel real data, all data elements pertaining hotel or costumer identification were deleted.
Four Columns, 'name', 'email', 'phone number' and 'credit_card' have been artificially created and added to the dataset.

We are given a hotel bookings dataset. This dataset contains booking information for a city hotel and a resort hotel. It contains the following features.

- hotel: Name of hotel ( City or Resort)
- is_canceled: Whether the booking is canceled or not (0 for no canceled and 1 for canceled)
- lead_time: time (in days) between booking transaction and actual arrival.
- arrival_date_year: Year of arrival
- arrival_date_month: month of arrival
- arrival_date_week_number: week number of arrival date.
- arrival_date_day_of_month: Day of month of arrival date
- stays_in_weekend_nights: No. of weekend nights spent in a hotel
- stays_in_week_nights: No. of weeknights spent in a hotel
- adults: No. of adults in single booking record.
- children: No. of children in single booking record.
- babies: No. of babies in single booking record. 
- meal: Type of meal chosen 
- country: Country of origin of customers (as mentioned by them)
- market_segment: What segment via booking was made and for what purpose.
- distribution_channel: Via which medium booking was made.
- is_repeated_guest: Whether the customer has made any booking before(0 for No and 1 for 
                     Yes)
- previous_cancellations: No. of previous canceled bookings.
- previous_bookings_not_canceled: No. of previous non-canceled bookings.
- reserved_room_type: Room type reserved by a customer.
- assigned_room_type: Room type assigned to the customer.
- booking_changes: No. of booking changes done by customers
- deposit_type: Type of deposit at the time of making a booking (No deposit/ Refundable/ No refund)
- agent: Id of agent for booking
- company: Id of the company making a booking
- days_in_waiting_list: No. of days on waiting list.
- customer_type: Type of customer(Transient, Group, etc.)
- adr: Average Daily rate.
- required_car_parking_spaces: No. of car parking asked in booking
- total_of_special_requests: total no. of special request.
- reservation_status: Whether a customer has checked out or canceled,or not showed 
- reservation_status_date: Date of making reservation status.

--------Total number of rows in data: 119390
--------Total number of columns: 32
# Steps
- Data Import: I imported and processed raw data from CSV files into Jupyter Notebook using pandas Library.
- Data Cleaning and Transformation: I cleaned the data to verify its correctness and consistency, which included standardising formats and fixing mistakes. 
1) Removing Duplicate rows
2) Handling null values
3) Converting columns to appropriate data types
4) Removing outliers
5) Creating new columns

- Exploratory Data Analysis : Performed EDA and tried answering the following questions:
1) What are the variables that affect hotel reservatiin cancellation?
2) How can we make hotel reservations cancellations better?
3) How will hotels be assisted in making pricing and promotional decision?

Mainly performed using Matplotlib and Seaborn library and the following graph and plots had been used:

- Bar Plot.
- Histogram.
- Scatter Plot.
- Pie Chart.
- Line Plot.
- Heatmap.
- Box Plot

# Hypothesis
1) More cancellations occur when prices are higher.
2) When there is a longer waiting list, customers tend to cancel more frequently.
3) The majority of clients are coming from offline travel agents to make their reservations.

# Analysis and Findings 
![Reservation status](https://github.com/shobkro/Hotel_Booking_Analysis_EDA/assets/39133098/2b24c11f-9b10-4ae9-87d5-f3789ba419e5)

The percentage of cancelled and non-canceled bookings is displayed in the accompanying bar graph. It is clear that a sizable portion of bookings have not yet been cancelled. 37% of customers still cancel their reservations, which significantly lowers the hotel's profits.

![Reservation status in different hotel](https://github.com/shobkro/Hotel_Booking_Analysis_EDA/assets/39133098/2d8181c2-97ea-402d-a182-01ade6cb2d39)

City hotels have more reservations than resort hotels. There's a chance that resort hotels cost more than city hotels.

![Average Daily Rate in city and resort hotel](https://github.com/shobkro/Hotel_Booking_Analysis_EDA/assets/39133098/b1df938e-8673-46a7-a1f1-3a9cf319f89c)

The accompanying line graph illustrates how the average daily prices for a city hotel can be cheaper than that of a resort hotel on certain days and considerably less on others. It goes without saying that resort hotel rates may increase on weekends and holidays.

![Reservation status per month](https://github.com/shobkro/Hotel_Booking_Analysis_EDA/assets/39133098/0bea3b23-b59d-44b6-8681-855c1bd54cdc)

In order to examine the months with the highest and lowest reservation levels based on reservation status, we have created a grouped bar graph. It is evident that August has the highest number of confirmed reservations as well as the highest number of cancelled reservations. On the other hand, January has the highest number of cancelled bookings.

Let's now examine which country has the largest number of cancelled reservations. Portugal is the nation with the most cancellations overall.

![Top 10 countries with reservation cancelled](https://github.com/shobkro/Hotel_Booking_Analysis_EDA/assets/39133098/f37e4b5b-0a03-4566-8d3f-768bc07ca274)

Let's investigate the region where visitors are arriving at the hotels and submitting their bookings. Does it originate from online or offline travel agents, groups, or direct? Approximately 46% of the customers are from online travel agents, while 27% are from organisations. Just 4% of customers make direct hotel reservations by going there.

![Average Daily Rate](https://github.com/shobkro/Hotel_Booking_Analysis_EDA/assets/39133098/bd329507-9490-4cc4-a77d-e99ff3080def)

Reservations are cancelled when the average daily cost is greater than when they are not cancelled, as the graph illustrates. It amply supports previous study, which states that a greater price corresponds with a larger failure rate.

# Suggestions 
1) The rate of cancellations increases as prices rise. Hotels should improve their pricing tactics and attempt to reduce the costs of particular hotels based on locations in order to minimise reservation cancellations. Additionally, they can give their customers certain discounts.
2) Due to the fact that resort hotels have a greater cancellation to non-cancellation ratio than city hotels. In consideration of this, hotels have to give a fair room rate reduction on weekends and holidays.
3) Since January is the month with the greatest cancellation rate, hotels can initiate campaigns or marketing with a modest budget to boost income.
4) To lower the cancellation rate, they might also improve the quality of their accommodations and services, particularly in Portugal.
