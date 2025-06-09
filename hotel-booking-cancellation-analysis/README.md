# Hotel Booking Cancellation Analysis

This project was developed as a Data Analytics portfolio piece. It simulates a real-world business case in which a data analyst explores hotel booking data to uncover factors affecting reservation cancellations and builds a machine learning model to predict them.

---

## 📌 Project Overview

The goal of this analysis is to explore a dataset of hotel bookings, identify the main drivers of cancellations, and develop a classification model to predict which bookings are likely to be canceled.  
The dataset includes detailed information on bookings, such as guest demographics, booking channels, reservation dates, and special requests.

**Main questions explored:**
- What percentage of bookings are canceled?
- Which variables are most strongly associated with cancellations?
- How accurately can we predict if a booking will be canceled?

---

## 🧪 Development Process

### Initial Planning
- Defined the objective and success criteria
- Identified relevant features for modeling (lead time, booking changes, room type, market segment, etc.)

### Data Inspection & Cleaning
- Loaded and reviewed 119,390 records
- Checked for missing values and handled them appropriately
- Converted date columns and created new time-based features

### Exploratory Analysis
- Calculated cancellation rates and examined variable distributions
- Explored relationships between features (e.g., lead time and cancellations)
- Visualized patterns and correlations using Seaborn and Matplotlib

### Feature Engineering & Modeling
- Engineered features from date columns
- One-hot encoded categorical variables
- Built and evaluated a logistic regression model to predict cancellations

---

## 📊 Key Insights

-	The cancellation rate is approximately 37% (about 44,000 out of 119,390 bookings).
-	Bookings with higher lead times are strongly associated with cancellations (as shown in the boxplot: median lead time for canceled bookings is much higher than for non-canceled).
-	The logistic regression model achieves an accuracy of 82% and a ROC AUC of 0.89.
-	The model’s recall for canceled bookings is 68%, meaning it identifies most cancellations but misses some, which is typical for imbalanced datasets.


---

## 📁 Project Files

- `Hotel_Booking_Cancellation_Analysis_Portfolio.ipynb`  
  → Jupyter Notebook with all data loading, cleaning, exploration, and modeling

- `hotel_bookings.csv`  
  → Original dataset (from [Kaggle](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand))

---

## 🛠 Tools Used

- Python
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- Jupyter / Google Colab

---

This project demonstrates the full data analysis lifecycle: business understanding, data cleaning, feature engineering, modeling, and insight communication.  
It reflects the practical skills and thinking of a data analyst working with real business data.

---
