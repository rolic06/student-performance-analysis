• Problem: Predict a vehicle's city-cycle fuel efficiency (mpg) using its physical specs and engine attributes (a regression task) .
• Dataset: 398 instances and 7 core features (cylinders, displacement, horsepower, weight, acceleration, model_year, origin), plus car_name as an ID and mpg as the target (0.1.1).
• Steps:
	1. Load the data and handle missing values in the horsepower column .
	2. Encode categorical features (origin) and drop the unique car_name string .
	3. Split into training and testing sets, then scale numerical features.
	4. Train and evaluate regression models (e.g., Linear Regression, Random Forest).
• Key Findings: Fuel efficiency (mpg) has a strong negative correlation with vehicle weight, displacement, horsepower, and cylinders, while newer model_year vehicles generally achieve higher MPG.
• Charts:
	• Scatter plots: weight vs. mpg and horsepower vs. mpg to show inverse trends.
	• Correlation heatmap: To visualize relationships across all numerical features.
	• Box plots: mpg grouped by cylinders or origin.
• Author: Donated by R. Quinlan (1993), revised from the CMU StatLib library.

How to Run: Install the UCI library and fetch the dataset directly in Python

# code
from ucimlrepo import fetch_ucirepo

auto_mpg = fetch_ucirepo(id=9)
X = auto_mpg.data.features
y = auto_mpg.data.targets
