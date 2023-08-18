# Investigate-Business-Hotel-using-Data-Visualization
Source : [Kagle](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand)

# Predict Customer Personality Marketing Campaign Clustering
**Column Description**
- `hotel` = Hotel (H1 = Resort Hotel or H2 = City Hotel)
- `is_canceled` = Value indicating if the booking was canceled (1) or not (0)
- `lead_time` = Number of days that elapsed between the entering date of the booking into the PMS and the arrival date
- `arrival_date_year` = Customer’s marital status
- `arrival_date_month` = Month of arrival date
- `arrival_date_week_number` = Week number of year for arrival date
- `arrival_date_day_of_month` = Day of arrival date
- `stays_in_weekend_nights` = Number of weekend nights (Saturday or Sunday) the guest stayed or booked to stay at the hotel
- `stays_in_weekdays_nights` = Number of week nights (Monday to Friday) the guest stayed or booked to stay at the hotel
- `adults` = Number of adults
- `children` = Number of children
- `babies` = Number of babies
- `meal` = Type of meal booked. Categories are presented in standard hospitality meal packages: Undefined/SC – no meal
- `country` = Country of origin. Categories are represented in the ISO 3155–3:2013 format
- `market_segment` = Market segment designation. In categories, the term “TA” means “Travel Agents” and “TO” means “Tour Operators”
- `distribution_channel` = Booking distribution channel. The term “TA” means “Travel Agents” and “TO” means “Tour Operators”
- `is_repeated_guest` = Value indicating if the booking name was from a repeated guest (1) or not (0)
- `previous_cancellations` = Number of previous bookings that were cancelled by the customer prior to the current booking
- `previous_bookings_not_canceled` = Number of previous bookings not cancelled by the customer prior to the current booking
- `reserved_room_type` = Code of room type reserved. Code is presented instead of designation for anonymity reasons.
- `assigned_room_type` = Code for the type of room assigned to the booking. Sometimes the assigned room type differs from the reserved room type due
- `booking_changes` = Number of changes/amendments made to the booking from the moment the booking was entered on the PMS
- `deposit_type` = Indication on if the customer made a deposit to guarantee the booking. This variable can assume three categories: No
- `agent` = ID of the travel agency that made the booking
- `company` = ID of the company/entity that made the booking or responsible for paying the booking. ID is presented instead of designation for
- `days_in_waiting_list` = Number of days the booking was in the waiting list before it was confirmed to the customer
- `customer_type` = Type of booking, assuming one of four categories: Contract - when the booking has an allotment or other type of
- `adr` = Average Daily Rate as defined by dividing the sum of all lodging transactions by the total number of staying nights
- `required_car_parking_spaces` = Number of car parking spaces required by the customer
- `total_of_special_requests` = Number of special requests made by the customer (e.g. twin bed or high floor)
- `reservation_status` = Reservation last status, assuming one of three categories: Canceled – booking was canceled by the customer; Check-Out
- `reservation_status_date` = Date at which the last status was set. This variable can be used in conjunction with the ReservationStatus to
  
## Problem Statement
A hotel company has a large number of cancellations every year. So the company wants to know the factors that affect the number of cancellations

## Objective
Analyze the factors that influence the number of bookings and the number of hotel cancellations, such as the influence of season on interest in hotel bookings, the effect of long holidays on interest in booking, etc

# Quick Result 
## Comparison of The Number of Hotel bookings Per Year
<img src="https://github.com/JodhiKrisantus/Investigate-Business-Hotel-using-Data-Visualization/blob/master/Assets/Comparison%20of%20the%20number%20of%20hotel%20bookings%20per%20year.png">

- Every year, customers tend to book hotels with a preference for city hotels compared to resort hotels. This could indicate that the location of the hotel plays an important role in the customer's decision to book a room. Maybe city hotels offer easier access to downtown, tourist attractions, businesses, or other public facilities, so that they are more in demand by tourists or business people.
- There were no hotel bookings in March - August in 2017. And there were no hotel bookings from November - February in 2019. Whereas in 2018 there was consistency in hotel bookings throughout the month.

## Number of Hotel Bookings Per Month
<img src="https://github.com/JodhiKrisantus/Investigate-Business-Hotel-using-Data-Visualization/blob/master/Assets/Number%20of%20hotel%20bookings%20per%20month.png">

- Overall, the total number of hotel bookings for 3 years occurred mostly in October. However, the average hotel booking per month is in July.
- The difference between the total number of hotel bookings and the average hotel booking per month shows: In October, hotels consistently get bookings every year, even though the number of bookings is not as many as in July. In July, hotels get the most average bookings, even though every year in July there are not necessarily hotel bookings.

## Relationship Between Seasons and Total Hotel Bookings
<img src="https://github.com/JodhiKrisantus/Investigate-Business-Hotel-using-Data-Visualization/blob/master/Assets/Relationship%20Between%20Seasons%20and%20Total%20Hotel%20Bookings.png">

- The rainy season makes customers less interested in booking hotels, perhaps due to the unfavorable weather factor for traveling/vacationing.
- The average number of hotel bookings increases during the holiday season, namely Eid (June) and Christmas (December). However, the increase is not so significant when compared to hotel bookings on weekdays / workdays.
- 
## Cancelled Booking to Stay Duration Ratio
<img src="https://github.com/JodhiKrisantus/Investigate-Business-Hotel-using-Data-Visualization/blob/master/Assets/Cancelled%20Booking%20to%20Stay%20Duration%20Ratio2.png">

- The total ratio of hotel booking cancellations is dominated by customers who book hotels on a monthly basis. This suggests that customers who book hotels for periods longer than 30 days tend to have higher cancellation rates. The reasons behind this may be various, such as changes in travel plans or other factors that cause them to cancel or change the duration of their stay.
- The lowest hotel booking cancellations were dominated by customers who booked hotels on a daily basis (0-6 days). Customers with daily bookings may be taking short business trips or short vacations, so their decision to book a hotel seems more certain.

<img src="https://github.com/JodhiKrisantus/Investigate-Business-Hotel-using-Data-Visualization/blob/master/Assets/Cancelled%20Booking%20to%20Stay%20Duration%20Ratio.png">

- The cancellation ratio for hotel bookings generally comes from city hotel types compared to resort hotels
- City hotels are often the first choice for business customers or those traveling for work purposes. Business and work travel plans can be very dynamic, so the cancellation rate at city hotels may be higher due to the possibility of sudden schedule changes. On the other hand, resort hotels are usually the choice for vacations or breaks, which tend to have more stable and consistent plans, so cancellations tend to be lower.

## Booking Lead Time vs. Cancelled Bookings Correlation
<img src="https://github.com/JodhiKrisantus/Investigate-Business-Hotel-using-Data-Visualization/blob/master/Assets/Booking%20Lead%20Time%20vs.%20Cancelled%20Bookings%20Correlation.png">

- The number of cancellations is affected by the distance between the order and the check-in time at the hotel. The longer the order interval, the greater the possibility for customers to cancel. Factors that may cause the long distance between orders can make customers more flexible in rearranging booking schedules.
- On average, the cancel booking ratio is dominated by customers with city hotel preferences.
