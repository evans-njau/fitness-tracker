# Fitness Tracker Data Analysis
## Overview 
This Jupyter Notebook contains a comprehensive data analysis of fitness tracking data. The project explores various aspects of user fitness activities, including calories burned, steps taken, sleep patterns, and how these metrics relate to different demographic factors and activity types.

## Dataset Information
The dataset contains 200 records with the following columns:

record_id: Unique identifier for each record

timestamp: Date and time of the activity record

user_id: Unique identifier for each user

age: User's age

gender: User's gender (Male, Female, Other)

activity_type: Type of physical activity (Cycling, Strength Training, Swimming, Yoga, HIIT, Walking, Running)

duration_min: Duration of activity in minutes

calories_burned: Calories burned during the activity

heart_rate_avg: Average heart rate during activity

steps: Number of steps taken

sleep_hours: Hours of sleep

weight_kg: User's weight in kilograms

# Key Features
## Data Preprocessing
Checked for null values (none found in the original dataset)

Converted timestamp to datetime format

Extracted additional time features:

Date

Month name

Day of week

Hour of day

## Feature Engineering
Season Classification: Categorized months into seasons (Summer, Autumn, Spring)

Week Time Classification: Classified days as weekday or weekend

Generation Analysis: Calculated birth year and categorized users into generations:

Baby Boomers (born 1946-1964)

Generation X (born 1965-1980)

Millennials (Gen Y) (born 1981-1996)

Generation Z (born 1997-2012)

Generation Alpha (born 2012+)

# Key Insights
## Activity Analysis
HIIT burns the most calories on average (320.63 calories)

Cycling burns the least calories on average (250.48 calories)

Thursday is the most popular day for training (34 records)

August is the most active month (43 records)

## Seasonal Patterns
Summer has the highest activity levels (109 records)

Autumn follows with 52 records

Spring has the least activity (39 records)

##Demographic Insights
Generation X takes the most steps on average (15,687.96 steps)

Generation Z takes the fewest steps on average (12,776.08 steps)

## Time-based Analysis
Weekend vs Weekday: Weekends show higher average steps (15,518.27) but lower average calories burned (272.10) compared to weekdays

## Files
Fitness_tracker.ipynb: Main analysis notebook

random_fitness_dataset.csv: Original dataset

cleaned_fitness_data.csv: Processed dataset with additional features

## Technologies Used
Python

Pandas (Data manipulation)

NumPy (Numerical operations)

Matplotlib & Plotly (Visualization)

## Usage
The notebook demonstrates:

Data loading and inspection

Data cleaning and transformation

Exploratory data analysis

Feature engineering

Statistical summaries and insights

### This analysis provides valuable insights for fitness professionals, health researchers, and anyone interested in understanding fitness patterns across different demographics and time periods.
