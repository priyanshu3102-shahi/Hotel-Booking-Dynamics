# 🏨 Hotel Booking Analysis & Prediction  

## 📌 Project Overview  
This project focuses on analyzing hotel booking data to understand guest behavior, booking trends, and cancellation patterns.  
Using machine learning, the project predicts booking cancellations while also providing insights into high-risk customers, seasonal trends, and country-specific booking dynamics.  

----------------------------------------------------------------------------------------------------------------------

## 📂 Dataset Overview  
- **Rows:** 119,391  
- **Columns:** 32  
- **Dataset:** Hotel Booking Dataset  

### Key Features:
- **country:** Country of origin of the guest.  
- **market_segment:** Market segment designation.  
- **distribution_channel:** Booking distribution channel.  
- **is_repeated_guest:** Whether the guest is a repeated guest (1) or not (0).  
- **previous_cancellations:** Number of previous cancellations by the guest.  
- **previous_bookings_not_canceled:** Number of previous bookings not canceled.  
- **reserved_room_type / assigned_room_type:** Codes for reserved and assigned rooms.  
- **booking_changes:** Number of changes made to the booking.  
- **deposit_type:** Type of deposit made for the booking.  
- **agent / company:** ID of the travel agency or company that made the booking.  
- **days_in_waiting_list:** Number of days the booking was on the waiting list.  
- **customer_type:** Type of customer.  
- **adr:** Average daily rate for the stay.  
- **required_car_parking_spaces:** Number of car parking spaces required.  
- **total_of_special_requests:** Number of special requests made.  
- **reservation_status:** Final status of the reservation.  
- **reservation_status_date:** Date of the last status change.  

----------------------------------------------------------------------------------------------------------------------

## 🧹 Data Cleaning & Preprocessing  
- **Missing Data Handling:** Impute or remove missing values in `children`, `country`, and `agent`.  
- **Outlier Detection:** Handle anomalies in `adr` and `lead_time`.  
- **Data Type Conversion:** Ensure correct data types for all columns.  

----------------------------------------------------------------------------------------------------------------------

## 🔍 Exploratory Data Analysis (EDA)  
- **High-Risk Customers:** Identify customers with multiple past cancellations.  
- **Most Frequent Guests:** Track repeated guest bookings.  
- **Seasonal Booking Trends:** Discover peak booking months and demand patterns.  

----------------------------------------------------------------------------------------------------------------------

## 🔗 Joins & Multi-Table Queries  
- **Hotel-Specific Cancellation Rate:** Cancellation analysis per hotel type.  
- **Country-Wise Cancellations:** Identify countries with high cancellation rates.  

----------------------------------------------------------------------------------------------------------------------

## 🤖 Model Building  
- **Data Split:** 80% training, 20% testing.  
- **Models Tested:**  
  - Logistic Regression  
  - Decision Tree  
  - Random Forest  
  - Gradient Boosting Machines  
  - Support Vector Machines  

- **Hyperparameter Tuning:** Grid Search / Random Search.  

**Target Variable:** `reservation_status` (canceled vs. not canceled).  

----------------------------------------------------------------------------------------------------------------------

## 🛠️ Tools & Libraries  
- **Language:** Python  
- **Libraries:** pandas, numpy, scikit-learn, seaborn, matplotlib  

----------------------------------------------------------------------------------------------------------------------

## 📁 Repository Structure  

```bash
Hotel-Booking-Analysis/
│
├── data/
│   └── hotel_bookings.csv        # Dataset file
│
├── notebook/
│   └── hotel_booking_analysis.ipynb   # Jupyter notebook with code
│
└── README.md                     # Project documentation
