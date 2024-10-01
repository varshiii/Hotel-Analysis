# 🏥 **Hospital Analysis using Pandas**
  
**Analyzing hospital bookings, room capacity, and customer behavior**

---

## 📋 **Overview**
This project performs a comprehensive hospital booking analysis using multiple datasets and `Pandas` to uncover trends in **bookings**, **room occupancy**, and **customer ratings**. By leveraging both **dimensional** and **fact tables**, the project dives into understanding **hospital capacity utilization**, booking platforms, customer behavior, and revenue generation.

---

## 🔧 **Features**
- **Data Import and Exploration**: Loading multiple datasets and performing an initial exploration of the data structure.
- **Data Cleaning**: Handling missing values, formatting inconsistencies, and filtering out irrelevant data.
- **Data Transformation**: Creating new features and merging datasets for analysis.
- **Insights Generation**: Exploring key metrics such as booking trends, revenue generation, and customer behavior.

---

## 🛠️ **Tools & Libraries**
- `Pandas` for data manipulation.
- `Matplotlib` for visualizations.
- `Jupyter Notebook` for interactive analysis.

---

## 📊 **Datasets Used**

### 1. **`dim_date.csv`**
   - A dimensional table containing information on:
     - **Dates**, **months**, and **years**
     - **Day types** (Weekend or Weekday)
     - **Week number**

### 2. **`dim_hotels.csv`**
   - A dimensional table containing:
     - **Property ID**, property name
     - **Category**, city

### 3. **`dim_rooms.csv`**
   - A dimensional table containing:
     - **Room ID**, room class

### 4. **`fact_aggregated_bookings.csv`**
   - A fact table containing:
     - **Property ID**, check-in date
     - **Room category**, successful bookings, capacity

### 5. **`fact_bookings.csv`**
   - A fact table containing:
     - **Booking ID**, property ID
     - **Booking date**, check-in and check-out dates
     - Number of guests, room category, booking platform, ratings, booking status
     - **Revenue generated**, revenue realized

---

## 🧑‍💻 **Techniques Used**

### 1. **Data Import and Exploration**
   - Imported the datasets using `Pandas` and explored the structure of each table to understand its role in the analysis.
   - Performed initial **data profiling** to understand data types, missing values, and overall distribution.

### 2. **Data Cleaning**
   - Addressed missing values by **removal** where necessary.
   - Cleaned and reformatted **date columns** to ensure consistency.

### 3. **Data Transformation**
   - Merged the dimensional and fact tables using appropriate joins (e.g., merging `dim_hotels` with `fact_bookings` on **property_id**).
   - Created new features such as **occupancy percentage (occ %)** to analyze room utilization.

### 4. **Insights Generation**
   - Analyzed **successful booking trends** across different time periods (weekday vs. weekend).
   - Visualized **revenue realized** per city and hotel type.
   - Evaluated **customer behavior** based on ratings.

---

## 📝 **Conclusion**
This hospital booking analysis provides valuable insights into how properties can:
- Optimize **room capacity**.
- Better understand **customer preferences**.
- Improve overall **revenue generation**.

The use of **fact and dimensional tables** allows for a more detailed and accurate analysis of booking data. Feel free to explore and adapt this analysis for your own hospital booking data!
