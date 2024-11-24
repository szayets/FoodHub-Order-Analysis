### FoodHub-Order-Analysis

#### Context
The number of restaurants in New York is increasing day by day. Lots of students and busy professionals rely on those restaurants due to their hectic lifestyles. Online food delivery service is a great option for them. It provides them with good food from their favorite restaurants. A food aggregator company FoodHub offers access to multiple restaurants through a single smartphone app.

The app allows the restaurants to receive a direct online order from a customer. The app assigns a delivery person from the company to pick up the order after it is confirmed by the restaurant. The delivery person then uses the map to reach the restaurant and waits for the food package. Once the food package is handed over to the delivery person, he/she confirms the pick-up in the app and travels to the customer's location to deliver the food. The delivery person confirms the drop-off in the app after delivering the food package to the customer. The customer can rate the order in the app. The food aggregator earns money by collecting a fixed margin of the delivery order from the restaurants.

#### Objective
The food aggregator company has stored the data of the different orders made by the registered customers in their online portal. They want to analyze the data to get a fair idea about the demand of different restaurants which will help them in enhancing their customer experience. Suppose you are hired as a Data Scientist in this company and the Data Science team has shared some of the key questions that need to be answered. Perform the data analysis to find answers to these questions that will help the company to improve the business.

#### Data Description
The data contains the different data related to a food order. The detailed data dictionary is given below.

#### Data Dictionary

- **order_id**: Unique ID of the order
- **customer_id**: ID of the customer who ordered the food
- **restaurant_name**: Name of the restaurant
- **cuisine_type**: Cuisine ordered by the customer
- **cost_of_the_order**: Cost of the order
- **day_of_the_week**: Indicates whether the order is placed on a weekday or weekend (Weekdays are from Monday to Friday and the weekend is Saturday and Sunday)
- **rating**: Rating given by the customer out of 5
- **food_preparation_time**: Time (in minutes) taken by the restaurant to prepare the food. This is calculated by taking the difference between the timestamps of the restaurant's order confirmation and the delivery person's pick-up confirmation.
- **delivery_time**: Time (in minutes) taken by the delivery person to deliver the food package. This is calculated by taking the difference between the timestamps of the delivery person's pick-up confirmation and drop-off information.


#### Installing the libraries with the specified version.

To install the required libraries with the specific versions, run the following command in your terminal:

```bash
!pip install numpy==1.25.2 pandas==1.5.3 matplotlib==3.7.1 seaborn==0.13.1 -q --user

```

#### Conclusions:
After examining the dataset provided, the following observations were made:

* Most popular cuisines are American, Japanese and Italian
* There is nearly three times the number of orders on weekends compared to weekdays.
* The median food preparation time is 25 minutes.
* The median food delivery time is also 25 minutes.
* Delivery times on weekends are typically 6 minutes shorter compared to weekdays.
* Faster order deliveries tend to receive higher ratings.
* Orders with higher costs also tend to receive higher ratings.
* More than one-third of orders are not rated.


#### Recommendations:
* Considering the significant number of orders without ratings, it is advisable to impruve customer feedback requests to gain a better understanding of customer preferences and behavior.
* Since weekends see a surge in orders, it's smart to focus on boosting orders during those days. This might mean adjusting our advertising efforts to promote popular restaurants and cuisines more heavily on weekends.
* To speed up weekday deliveries, recommending restaurants that are closer to customers would be beneficial. This would result in faster food delivery and possibly higher ratings.
* Suggesting the most popular cuisines and restaurants could boost the number of total orders.


