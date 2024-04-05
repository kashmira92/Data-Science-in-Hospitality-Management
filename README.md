# Data-Science-in-Hospitality-Management

This project delves into the realm of data science applied to hospitality management, specifically targeting room reservation predictions within a hotel booking system. The dataset provided encompasses a rich array of features ranging from guest demographics to booking details, aiming to forecast the type of room a guest is likely to reserve, thereby facilitating enhanced inventory management, tailored marketing strategies, and improved guest experiences.

## Problem Statement:
The objective is to develop a predictive model capable of accurately forecasting the type of room a guest is likely to reserve (room_type_reserved). By successfully predicting room types, hotels can optimize room inventory management, tailor marketing strategies, enhance guest experiences through personalized services, improve revenue management through dynamic pricing, and boost operational efficiency by anticipating demand for various room types.

## Aim:
To perform multi-class classification on room types that customers are likely to reserve.

## Dataset Attributes:
The dataset comprises various features describing booking details and customer preferences, including the number of adults and children, duration of stay, meal plan preference, requirement for parking space, lead time, market segment, guest history, average price per room, number of special requests, and booking status.
* no_of_adults: The number of adults included in the booking.
* no_of_children: The number of children included in the booking.
* no_of_weekend_nights: The number of weekend nights booked.
* no_of_week_nights: The number of weeknights booked.
* type_of_meal_plan: The type of meal plan selected by the guest.
* required_car_parking_space: Indicates whether the guest required a car parking space.
* room_type_reserved: The type of room reserved by the guest.
* lead_time: The number of days between the booking date and the arrival date.
* arrival_year: The year of arrival.
* arrival_month: The month of arrival.
* arrival_date: The date of arrival.
* market_segment_type: The market segment from which the booking originated.
* repeated_guest: Indicates whether the guest has previously stayed at the hotel.
* no_of_previous_cancellations: The number of previous bookings that were canceled by the guest.
* no_of_previous_bookings_not_canceled: The number of previous bookings not canceled by the guest.
* avg_price_per_room: The average price per room for the booking.
* no_of_special_requests: The number of special requests made by the guest.
* booking_status: Indicates whether the booking was canceled or not.

## Data Pre-processing & Feature Engineering:
The dataset underwent cleaning and preparation for modeling. Relationships between features were analyzed, and appropriate visualization techniques were applied. Feature engineering was performed to enhance the dataset for modeling purposes. SMOTE Sampling Technique was applied due to the high imbalance in the dataset.
![image](https://github.com/kashmira92/Data-Science-in-Hospitality-Management/assets/48323327/d7029639-3c57-4e80-b1e3-448473e8c24e)


## Modeling:
Various classifier models such as SVM, Logistic Regression, KNN, and Random Forest were trained and optimized with hyperparameters to enhance performance. A validation pipeline utilizing 5-fold cross-validation was implemented to assess model performance. Classification accuracy, precision, recall, and F1 score were reported with both macro and weighted averages.

## Evaluation and Reporting:
A model was selected based on expected optimal performance on unseen data, and predictions were provided accordingly. The Random Forest model was chosen due to its superior F1 Score for both weighted and macro averages compared to KNN. External validation was conducted on a separate dataset named 'test.csv', where the label was hidden. The selected model was used to predict the label on 'test.csv', and the predictions were converted into a CSV file named 'submission.csv' using reverse mapping of the labels.
