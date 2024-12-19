# Hotel_Booking_data:

This dataset provides detailed information about bookings made at both a city hotel and a resort hotel. It includes data such as booking dates, length of stay, guest composition (adults, children, and babies), and features like parking availability. To protect privacy, all personally identifiable information has been removed.

I will use Postgres SQL to store the data into a warehouse try to create a star schema with dimension tables for customers, agents and company. 


Using Python, we will perform an exploratory analysis of this dataset to uncover meaningful patterns and insights.

I have tried to answer the following questions:

1. Which Country has the highest bookings?
2. What is the seasonality of booking by Month of the Year?
3. Which Hotel Type has highest number of bookings?
4. What is the average revenue per booking for a City Hotel VS a Resort Hotel?
5. How does the revenue differ by the room type for different hotels?




I have finally built a predictive model to findout if the booking will be cancelled. 

In this step, I have
1. Perform the Feature Engineering to make new features
2. Perform the Data Selection to select only relevant features
3. Split the data (Train Test Split)
4. Model the data (Fit the Data)
5. And finally Evaluate our model on Accuracy and ROC_AUC_score.

Findings:

1. City Hotels have higher booking than Resort Hotel.
2. The Bookings go up in the middle of the year and is relatively low during start and end of the year.
3. We see that the "Corporate" bookings go up towards the end of the year and reduces around mid of the year
4. Direct Bookings fall during mid of the year.
5. The majority booking are from "Transient" and "Transient - Party" Customer Type.
6. Most Guests are from the country PRT


From the Model:
1. The model has an accuracy score of ~0.77 AND and AUC score of 0.86
2. The lead_time, total_of_special_requests and previous_cancellelations are the most important factors in determining if the booking will be cancelled or not. 
