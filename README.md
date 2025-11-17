Table of Contents Introduction Dependencies Data Description Data Preprocessing Feature Engineering Model Training and Evaluation Results Usage Conclusion Introduction This notebook is designed to predict airfares based on historical data. The dataset contains features like airline, date of journey, source, destination, route, departure and arrival times, duration, and the total number of stops. Several regression models, including Linear Regression, Decision Tree, and Random Forest, are used to train the prediction model.

Dependencies To run this notebook, you need the following Python libraries:

pandas numpy matplotlib seaborn scikit-learn You can install the required libraries using the following command:

sh Copy code pip install pandas numpy matplotlib seaborn scikit-learn Data Description The dataset used in this notebook contains the following columns:

Airline: The airline company Date_of_Journey: The date of the journey Source: The source airport Destination: The destination airport Route: The route taken by the flight Dep_Time: Departure time Arrival_Time: Arrival time Duration: Duration of the flight Total_Stops: Total number of stops between source and destination Price: The price of the ticket (target variable) Data Preprocessing Data preprocessing steps include:

Handling missing values Converting date columns to datetime objects Extracting useful features from the date columns (e.g., day, month, year) Converting categorical variables into numerical ones using techniques like one-hot encoding and label encoding Feature Engineering Feature engineering involves:

Extracting additional features from existing columns, such as extracting hours and minutes from the Duration column. Creating new features that might help improve the model's performance. Model Training and Evaluation Several regression models are trained and evaluated, including:

Linear Regression Decision Tree Regression Random Forest Regression Model evaluation metrics include:

Mean Absolute Error (MAE) Mean Squared Error (MSE) Root Mean Squared Error (RMSE) R-squared score (R²) Results The results of each model are compared based on the evaluation metrics. Visualizations are created to show the performance of the models and the importance of various features.
