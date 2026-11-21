# 🚗 Auto MPG – Exploratory Data Analysis (EDA)

## 📌 Project Overview
This project explores the **Auto MPG dataset** to analyze vehicle fuel efficiency (Miles Per Gallon – MPG) and its relationship with various vehicle specifications. The goal is to perform basic Exploratory Data Analysis (EDA) using Python, NumPy, Pandas, and Matplotlib.

> **Note:** This project focuses on data analysis and visualization only. No machine learning models are trained.

## 📊 Dataset Information
- **Dataset:** Auto MPG
- **Instances:** 398
- **Target Variable:** `mpg`
- **Features:** 7 core features
- **Additional Column:** `car_name` (vehicle identification)

### Features
| Feature | Description |
|---|---|
| `cylinders` | Number of engine cylinders |
| `displacement` | Engine displacement |
| `horsepower` | Engine horsepower |
| `weight` | Vehicle weight |
| `acceleration` | Acceleration performance |
| `model_year` | Model year |
| `origin` | Vehicle origin |
| `car_name` | Car name/identifier |
| `mpg` | Fuel efficiency (target) |

**Dataset Source:** UCI Machine Learning Repository  
**Donor:** R. Quinlan (1993), revised from the CMU StatLib library.

## 🎯 Objectives
- Understand the structure and characteristics of the dataset.
- Analyze MPG statistics and distributions.
- Compare fuel efficiency across cylinder counts and origins.
- Identify the most fuel-efficient vehicles.
- Detect and handle missing values.
- Visualize relationships between vehicle specifications and MPG.

## 🔍 Analysis Performed
1. Load the dataset using Python.
2. Display `head()`, `tail()`, `shape`, `info()` and `describe()`.
3. Check missing values and duplicate rows.
4. Calculate mean, median, minimum and maximum MPG using NumPy.
5. Compare average MPG for 4, 6 and 8-cylinder vehicles.
6. Identify the model year with the highest average MPG.
7. List the 10 most fuel-efficient vehicles.
8. Analyze average MPG by vehicle origin.
9. Use Pandas filtering, sorting, `value_counts()` and `groupby()`.

## 📈 Visualizations
- **Cylinder-count bar chart:** Shows the number of vehicles for each cylinder category.
- **MPG histogram:** Displays the distribution of fuel efficiency.
- **Scatter plots:** Weight vs. MPG and horsepower vs. MPG.
- **Correlation heatmap:** Visualizes relationships among numerical features.
- **Box plots:** Compares MPG across cylinders or origins.

## 💡 Key Findings
- Vehicle weight, displacement, horsepower and cylinder count generally have a negative relationship with MPG.
- Vehicles from newer model years generally demonstrate better fuel efficiency.
- Fuel efficiency varies across vehicle origins and engine configurations.

## ❓ Questions Answered
1. What are the mean, median, minimum and maximum MPG values?
2. How does average MPG compare among 4, 6 and 8-cylinder vehicles?
3. Which model year has the highest average MPG?
4. What are the 10 most fuel-efficient cars?
5. Are there missing values, particularly in horsepower?
6. How does average MPG differ by origin?

## 📝 Observations
- Lighter vehicles generally achieve higher fuel efficiency.
- Four-cylinder vehicles tend to have higher average MPG than vehicles with six or eight cylinders.
- Average MPG generally improves across newer model years in the dataset.

## 🛠️ Tools & Technologies
- Python 3
- Pandas
