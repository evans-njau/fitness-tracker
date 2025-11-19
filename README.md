📊 Fitness Data Analysis Notebook

This project analyzes a randomly generated fitness dataset to explore user activity patterns, clean timestamp information, extract new time-based features, and visualize trends. The analysis is performed entirely in Python using Pandas, NumPy, Matplotlib, and Plotly.

📁 Project Overview

The notebook performs the following tasks:

1. Data Loading

Reads the dataset from random_fitness_dataset.csv.

Displays the first few rows for a quick preview.

2. Data Exploration

Uses:

info() to inspect data types and structure

describe() for statistical summary

Null value checks using:

isna().values.any()

isnull().sum()

3. Data Cleaning

Converts the time_stamp column into a valid datetime format.

Handles CSV inconsistencies.

Ensures clean and usable timestamps for feature extraction.

4. Feature Engineering

New features are created from the timestamp column:

date — Extracted date

month — Month name

day — Day of the week

hour — Extracted hour value

These features make the dataset easier to analyze and visualize.

📈 Visualizations (Depending on Notebook)

Although not fully visible from the preview, the imports suggest the notebook supports:

Matplotlib static plots

Plotly interactive charts

These help uncover trends such as:

Daily workout patterns

Monthly activity variations

Hourly fitness behavior

🛠️ Technologies Used
Library	Purpose
Pandas	Data loading, cleaning, and manipulation
NumPy	Numerical computations
Matplotlib	Static visualizations
Plotly	Interactive visualizations
datetime	Timestamp transformation
