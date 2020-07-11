# Linear Regression Project
Just got some contract work with an Ecommerce company based in New York City that sells clothing online but they also have in-store style and clothing advice sessions. Customers come in to the store, have sessions/meetings with a personal stylist, then they can go home and order either on a mobile app or website for the clothes they want.

The company is trying to decide whether to focus their efforts on their mobile app experience or their website. They've hired you on contract to help them figure it out! Let's get started!

(it's fake, don't worry I didn't give you real credit card numbers or emails).

The Data (Ecommerce Customers csv file) has numerical value columns:
- Avg. Session Length: Average session of in-store style advice sessions.
- Time on App: Average time spent on App in minutes
- Time on Website: Average time spent on Website in minutes
- Length of Membership: How many years the customer has been a member.

# Exploratory Data Analysis
To explore and understand the data we explore it using some plots.
eg: Pairplot is used to explore the types of relationship across the data.
	'Length of Membership' is the most correlated feature with 'Yearly Amount Spent'.

	lmplot was plot to show their relationship.


# Training and Testing the Data
Went ahead and split the data into training and testing sets. ** Set a variable X equal to the numerical features of the customers and a variable y equal to the "Yearly Amount Spent" column. **

# Training the Model
Trained the data on the training data 
Created an instance of a LinearRegression() model named lm.

# Predicting Test Data
Created a scatterplot of the real test values versus the predicted values.

# Evaluating the Model 
Evaluated the model performance by calculating the residual sum of squares and the explained variance score (R^2)
Calculated the Mean Absolute Error, Mean Squared Error, and the Root Mean Squared Error.

# Residuals
Explored the residuals to make sure that everything was okay with the data.

# Conclusion of the project 

### Interpreting the coefficients:

- Holding all other features fixed, a 1 unit increase in **Avg. Session Length** is associated with an **increase of 25.98 total dollars spent**.
- Holding all other features fixed, a 1 unit increase in **Time on App** is associated with an **increase of 38.59 total dollars spent**.
- Holding all other features fixed, a 1 unit increase in **Time on Website** is associated with an **increase of 0.19 total dollars spent**.
- Holding all other features fixed, a 1 unit increase in **Length of Membership** is associated with an **increase of 61.27 total dollars spent**.

### Focus more on their mobile app or on their website?

This is tricky, there are two ways to think about this: Develop the Website to catch up to the performance of the mobile app, or develop the app more since that is what is working better. This sort of answer really depends on the other factors going on at the company, probably want to explore the relationship between Length of Membership and the App or the Website before coming to a conclusion!
