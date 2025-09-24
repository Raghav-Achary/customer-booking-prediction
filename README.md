# Customer Booking Prediction

This project predicts whether a customer will complete a flight booking using machine learning based on booking and flight-related features.

---

## Dataset

The dataset contains customer booking details including:

- Number of passengers
- Sales channel (e.g., Internet)
- Trip type (e.g., RoundTrip)
- Purchase lead time (days before flight)
- Length of stay
- Flight hour and day
- Route and booking origin
- Preferences for extra baggage, preferred seat, and in-flight meals
- Flight duration
- Target variable: `booking_complete` (whether booking was completed)

---

## Project Overview

The project workflow includes:

### 1. Data Exploration & Cleaning
- Loaded and inspected the dataset.
- Checked for missing values and basic statistics.

### 2. Feature Engineering
- Created new features like `is_weekend` (if flight day is Saturday or Sunday).
- Computed `num_add_ons` by summing extra services requested.
- Applied one-hot encoding on categorical variables such as `sales_channel`, `trip_type`, `flight_day`, `route`, and `booking_origin`.

### 3. Modeling
- Split the data into training and test sets.
- Trained a **Random Forest Classifier** to predict booking completion.
- Selected Random Forest due to its ability to provide feature importance.

### 4. Evaluation
- Evaluated model performance using accuracy, classification report, and confusion matrix.
- Performed 5-fold cross-validation to ensure robustness.
- Visualized feature importance to interpret which features contribute most to the predictions.

---

## How to Run

1. Load the dataset `customer_booking.csv`.
2. Run the Jupyter Notebook containing the code (e.g., `task2_british_airways.ipynb`).
3. Follow the steps in the notebook for preprocessing, training, evaluation, and feature importance visualization.

---

## Dependencies

- Python 3.x  
- pandas  
- numpy  
- scikit-learn  
- matplotlib  
- seaborn

---

## Author

Raghav Achary  
[GitHub Profile](https://github.com/Raghav-Achary)

---

Feel free to open issues or suggest improvements!
