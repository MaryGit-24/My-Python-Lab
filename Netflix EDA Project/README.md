🎬 Netflix Exploratory Data Analysis (EDA)
Project Overview

This project focuses on Exploratory Data Analysis (EDA) of a Netflix dataset containing information about movies and TV shows available on the platform.

The goal of the project is to:

Clean and prepare the dataset

Handle missing and inconsistent values

Explore content distribution on Netflix

Analyze movie-related trends such as duration and directors

Visualize insights from the data

Dataset Description

The dataset contains the following columns:

show_id

type (Movie or TV Show)

title

director

cast

country

date_added

release_year

rating

duration

listed_in (genre)

description

Libraries Used

Python

Pandas

NumPy

Matplotlib

Seaborn

Data Loading and Initial Exploration

The dataset was loaded using Pandas.

The first five rows were inspected to understand the structure and content of the data.

Missing values were identified using .isnull().

Data Cleaning and Preparation
Dropping Unnecessary Columns

The show_id column was dropped as it does not contribute meaningful information for analysis.

Checking Data Types

.info() was used to inspect column data types.

.describe() was used to get a statistical summary of numeric columns.

Handling Missing Values

Missing values were handled thoughtfully to preserve data usability:

director → filled with "Not Specified"

cast → filled with "Not Listed"

country → filled with "Not Specified"

Rows with missing values in critical columns were removed:

date_added

rating

duration

After cleaning, all columns contained zero missing values, ensuring consistency for analysis.

Duration Column Cleaning

The duration column contained mixed formats such as:

"90 min"

"1 Season"

"2 Seasons"

To standardize this column:

Text such as "min", "Season", and "Seasons" was removed using string operations.

Extra white spaces were stripped.

The cleaned values were converted to integers.

Rather than performing arithmetic operations on duration, value counts were used to:

Understand how durations and seasons are distributed

Compare frequencies of different duration values

Content Type Distribution

The dataset contains both Movies and TV Shows.

Analysis showed that:

Movies make up approximately 70%

TV Shows make up approximately 30%

Movie-Specific Analysis

A subset containing only Movies was created to allow deeper analysis.

Director Analysis

Director counts were analyzed.

A large number of entries had "Not Specified" as the director.

These were excluded to focus on known directors.

Cleaning Director Names

Movies with multiple directors were split to retain only one director per movie.

The cleaned director data was converted into a DataFrame.

The total number of movies per director was calculated.

Visualization and Insights

Several visualizations were created to explore the dataset, including:

Distribution of Movies vs TV Shows

Top movie directors by number of movies

Duration distribution

Box plots to identify outliers in movie duration

Removing "Not Specified" directors allowed clearer insights into the most active directors on Netflix.

Key Insights

Netflix has a significantly higher number of movies compared to TV shows.

A large portion of director data is missing, which affects director-based analysis.

Movie durations vary widely, with some outliers identified.

Cleaning and standardizing text-based columns is crucial for meaningful analysis.

Conclusion

This project demonstrates a complete EDA workflow, including:

Data inspection

Handling missing values

Data cleaning and transformation

Subsetting data

Visualization and insight generation

It provides a strong foundation for further analysis, such as recommendation systems or content trend modeling.
