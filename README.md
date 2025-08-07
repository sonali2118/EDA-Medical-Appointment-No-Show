# EDA - Medical Appointment No-Show

This project performs **Exploratory Data Analysis (EDA)** on a dataset related to medical appointments in Brazil, to investigate the factors that influence whether a patient shows up for their appointment.

## 📁 Dataset Overview

The dataset contains **110,527** medical appointment records, with the following important columns:

- `PatientId`: Identifier for the patient
- `AppointmentID`: Unique identifier for each appointment
- `Gender`: Male or Female
- `ScheduledDay`: The day the appointment was scheduled
- `AppointmentDay`: The actual appointment day
- `Age`: Age of the patient
- `Neighbourhood`: Location of the hospital
- `Scholarship`: Indicates if the patient is enrolled in Brasilian welfare program
- `Hipertension`, `Diabetes`, `Alcoholism`, `Handcap`: Health conditions
- `SMS_received`: Whether the patient received an SMS reminder
- `No-show`: **Target variable** (`Yes` if patient did not show up)

📌 **Target Variable**: `No-show`

---

## 🎯 Project Objective

The main goal is to understand:
- What factors influence a patient missing their appointment?
- Are there any patterns related to age, gender, day of the week, or health conditions?
- Does receiving an SMS affect attendance?

---

## 🧰 Tools & Libraries

- Python
- pandas
- numpy
- matplotlib
- seaborn
- datetime

---

## 📊 EDA Summary

### ✅ Data Cleaning
- Checked for null/missing values
- Corrected data types (dates, boolean columns)
- Standardized column names

### 📈 Key Visualizations
- Show vs No-show count
- Age distribution
- Impact of SMS reminders
- No-show rate by weekday
- Heatmap of correlation between variables

### 🔍 Key Insights
- Around **20%** of appointments are no-shows.
- Younger patients are more likely to miss appointments.
- Patients with **no SMS reminder** are slightly more likely to miss.
- No-show rates vary by **day of the week**, with Friday having more absentees.
- Health conditions like **hypertension** and **diabetes** reduce the no-show probability slightly.

---

## 📌 Conclusion

EDA helped uncover multiple patterns in the data that can inform healthcare systems:
- Reminders help reduce no-shows.
- Age and day of week are critical factors.
- This dataset can be further used to **build predictive models** to reduce missed appointments.

---

## 🚀 Future Work

- Build a classification model to predict no-shows.
- Use feature engineering to improve model performance.
- Explore deeper temporal patterns (seasonality, holidays).

---

## 📂 How to Run

1. Clone this repo
2. Install required libraries:
   ```bash
   pip install pandas matplotlib seaborn
