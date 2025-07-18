# Data-Visualization

# 🏨 Hotel Booking Cancellation Analysis with Apache Superset

This is the final project for the Data Visualization course at Ho Chi Minh City University of Technology and Education. Our team explored the factors influencing hotel booking cancellations by building insightful dashboards using Apache Superset.

---

## 📌 Project Overview

With increasing competition in the hospitality industry, understanding customer behavior—especially booking cancellations—is vital for operational planning and revenue management.

In this project, we:
- Explored and preprocessed a real hotel booking dataset.
- Visualized key cancellation patterns.
- Identified critical insights and proposed practical solutions.
- Used Apache Superset for interactive and intuitive dashboards.

---

## 🎯 Project Objectives

- Analyze hotel booking behavior and cancellation patterns.
- Identify major factors impacting cancellations (lead time, deposit type, booking channel, etc.).
- Apply Apache Superset to create visual storytelling and derive business insights.
- Suggest strategic actions for hotels to minimize cancellations.

---

## 🛠️ Tools & Technologies

| Tool              | Description                                           |
|-------------------|-------------------------------------------------------|
| Python (Pandas)   | Data preprocessing and feature analysis               |
| Apache Superset   | Open-source BI tool for dashboard visualization       |
| Jupyter Notebook  | Used during the data cleaning phase                   |
| Hotel Booking Dataset | Public dataset from [Kaggle](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand) |

---

## 📂 Dataset

- **Source:** Kaggle – Hotel Booking Demand Dataset  
- **Records:** ~119,000 hotel bookings  
- **Columns:** 32 features, including:
  - `hotel`, `is_canceled`, `lead_time`, `arrival_date_*`, `adr`
  - `customer_type`, `deposit_type`, `distribution_channel`
  - `special_requests`, `booking_changes`, and more

---

## 📈 Key Insights

- **Cancellation Rate:** 27.67% overall
  - City Hotel: 30.31%
  - Resort Hotel: 23.54%
- **Deposit Type Anomaly:**
  - 'Non Refund' bookings had a cancellation rate of **94.7%**
- **Lead Time:** Longer lead time correlated with higher cancellation
- **Channel Impact:** TA/TO (Travel Agent/Tour Operator) had the highest cancellation rate
- **Customer Behavior:**
  - New customers tend to cancel more than repeat customers
  - More special requests → lower cancellation likelihood
- **Booking Changes:** Both too few and too many booking changes increased cancellation risk

---

## 📊 Dashboards & Visualizations

We created dashboards using:
- **Heatmaps:** Cancellations by month and hotel type
- **Boxplots:** ADR vs Cancellation
- **Bar Charts:** Cancellation by distribution channel, deposit type
- **Line Charts:** Lead time trends
- **Sunburst / Pie Charts:** Customer type vs Cancellation

All dashboards were built using **Apache Superset**, deployed locally.

---

## ⚙️ How to Run the Project

### 1. Setup Apache Superset

Follow [official setup guide](https://superset.apache.org/docs/installation/installing-superset-from-scratch) to install Superset.

Or use Docker:

```bash
docker-compose -f docker-compose-non-dev.yml up
````

### 2. Prepare Data

Run the provided Jupyter/Python script to clean and export the dataset:

```bash
python preprocess_hotel_bookings.py
```

This will create `cleaned_hotel_bookings.csv`.

### 3. Load Data into Superset

* Upload the cleaned CSV or connect Superset to a database (e.g., SQLite/Postgres).
* Define your dataset schema.
* Start creating charts and dashboards based on key questions (e.g., Why do bookings get canceled? Which customers cancel more?).

### 4. Explore Dashboards

Log in to Superset and explore:

* Hotel type comparison
* Seasonal cancellation trends
* Effects of deposit type, booking channel
* Behavior of customer segments

---

## 👨‍💻 Team Members

| Name               | Student ID | Contribution                        |
| ------------------ | ---------- | ----------------------------------- |
| Trần Tuyên Trường  | 20133108   | Data collection & preprocessing     |
| Lê Quỳnh Nhựt Vinh | 22133066   | Analysis, report writing            |
| Lê Hồ Quốc Huy     | 22133025   | Superset dashboards & system design |

Instructor: **Mr. Lê Quang Thái**

---

## 📚 References

* Hotel Booking Demand Dataset: [https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand)
* Apache Superset: [https://superset.apache.org/](https://superset.apache.org/)

---

## 📌 License

This project is intended for educational and academic use only.

```
