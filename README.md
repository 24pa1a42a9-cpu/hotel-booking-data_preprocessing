# Hotel Booking Data Preprocessing & Quality Improvement Analysis

This project demonstrates end-to-end data preprocessing performed on a real-world hotel booking dataset using Python and Pandas.

## 📌 Project Objective
The main goal of this project is to transform raw hotel reservation data into a clean, structured, and machine-learning-ready dataset.

---

## 🔍 Data Quality Issues Identified Before Cleaning
- Large number of missing values
- Highly incomplete `company` column
- 31,994 duplicate booking records
- Invalid reservations with zero guests
- Extreme outliers in `adr` (Average Daily Rate)

---

## 🛠 Preprocessing Techniques Applied
### ✅ Missing Value Treatment
- Dropped `company` column due to 94% null values
- Filled `agent` null values with `0`
- Filled `country` null values with `"Unknown"`
- Filled `children` null values using median

### ✅ Duplicate Removal
- Removed 31K+ repeated rows

### ✅ Logical Data Validation
- Removed zero guest bookings

### ✅ Outlier Handling
- Applied IQR (Interquartile Range) method on ADR column

### ✅ Feature Engineering
Created new useful columns:
- `total_guests`
- `total_nights`
- `arrival_month_num`
- `is_family`

---

## 📊 Before vs After Cleaning Highlights
| Metric | Before Cleaning | After Cleaning |
|--------|----------------|---------------|
| Total Rows | 119390 | 84715 |
| Total Columns | 32 | 34 |
| Missing Values | 129425 | 0 |
| Duplicate Rows | 31994 | 0 |

---

## 💻 Tools & Libraries Used
- Python
- Pandas
- NumPy
- Matplotlib
- Google Colab

---

## 📁 Repository Files
- `Hotel_Booking_Preprocessing.ipynb` → Complete preprocessing notebook
- `cleaned_hotel_bookings.csv` → Final cleaned dataset

---

## ✅ Final Outcome
The raw hotel booking dataset was successfully converted into a clean, high-quality, and analysis-ready dataset suitable for future machine learning or business analytics tasks.
