**Customer Flight Booking Prediction**

This project applies Exploratory Data Analysis (EDA), feature engineering, and machine learning to predict whether a customer completes a flight booking based on their preferences and booking data.

**Dataset**

The dataset (customer_booking.csv) contains customer-level booking information, such as:

    Booking channel

    Travel preferences (extra baggage, seat preference, in-flight meals)

    Route and origin

    Booking completion status (target variable)

    Note: The dataset is read using ISO-8859-1 encoding due to special characters.

**Workflow Overview**

    EDA and Data Cleaning

    Load and inspect the data

    Visualize target distribution

    Check for missing values and data types

**Feature Engineering**

Created new features:

    is_weekend_flight: Flag for weekend travel

    has_preferences: Flag if the user requested any add-ons

    One-hot encoded categorical variables

**Modeling**

    Model used: RandomForestClassifier

    Data split: 80% training / 20% testing

    Evaluated using:

            Accuracy

            Precision

            Recall

            F1-Score

            ROC AUC Score

            5-Fold Cross-Validation

**Feature Importance**

        Visualized top features influencing booking completion

**Evaluation Metrics**

The model was evaluated using multiple metrics and cross-validation:

    Classification Report

    ROC AUC Score

    Cross-Validation Accuracy

    Cross-Validated Precision, Recall, F1, ROC AUC

**Top Feature Importances**

After fitting the model, the top 10 features contributing to the booking prediction were visualized using a horizontal bar plot.

**Tech Stack**

    Python (Pandas, NumPy, Seaborn, Matplotlib)

    Scikit-learn (RandomForestClassifier, metrics, model_selection)

**How to Run**

Clone the repository:

git clone https://github.com/your-username/customer-booking-prediction.git
cd customer-booking-prediction

Install dependencies:

pip install -r requirements.txt

Place the customer_booking.csv file in the project directory.

Run the script:
