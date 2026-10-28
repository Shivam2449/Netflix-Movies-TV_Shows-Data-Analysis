# 🎬 Netflix Content Insights & Exploratory Data Analysis

**An Exploratory Data Analytics Project using Python**

## 📌 Project Overview

This project analyze Netflix's Movies and TV Shows to uncover meaningful patterns in its content library. By analyzing content categories, release years, genres, ratings, and country-related information, the project provides a better understanding of the platform's content distribution.

## 🎯 Project Objectives

* Understand the structure and characteristics of the Netflix dataset.
* Detect and handle missing values to improve data quality.
* Examine the distribution of Movies and TV Shows.
* Analyze content trends based on release years, genres, and ratings.
* Explore the relationship between a title's release year and its addition to Netflix.
* Present analytical findings through clear and meaningful charts.

## 🛠️ Skills & Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Data Cleaning and Preprocessing
* Exploratory Data Analysis (EDA)
* Data Visualization

## 📂 Dataset Information

**Dataset Name:** Netflix Movies and TV Shows Dataset
**File Name:** `netflix_titles.csv`
**Total Records:** 8,807
**Total Features:** 12
**Analysis Type:** Exploratory Data Analysis (No target variable)

### Key Attributes

* **Content Identification:** Title name and content type (Movie or TV Show).
* **Production Details:** Director, cast members, and country of production.
* **Release Information:** Original release year and date added to Netflix.
* **Content Classification:** Ratings and genre categories.
* **Duration Details:** Movie runtime and number of seasons for TV Shows.
* **Analysis Focus:** `type`, `release_year`, `rating`, and `date_added` are key attributes used to explore content distribution and trends.

## 🔍 Project Workflow

### 1️⃣ Data Loading & Initial Inspection

* Loaded the CSV file into a Pandas DataFrame.
* Checked the number of rows and columns.
* Examined data types and dataset information.
* Generated descriptive statistics for numerical columns.

### 2️⃣ Data Cleaning & Preprocessing

* Identified missing values across the dataset.
* Calculated the percentage of missing values in each column.
* Reviewed numerical and categorical attributes.
* Prepared the data for consistent analysis.

### 3️⃣ Missing Value Treatment

Missing values were examined to identify which attributes required attention.

**Columns with missing values included:**

* `director`
* `cast`
* `country`
* `rating`
* `duration`
* `date_added`

Missing entries in these columns were initially filled with  `"Unknown"`.

The `date_added` column was subsequently converted to Pandas datetime format, with invalid or unparseable values handled using `errors='coerce'`.

### 4️⃣ Exploratory Data Analysis (EDA)

**EDA was performed using:**

1. Bar Charts
2. Histograms
3. Scatter Plots
4. Box Plots
5. Pie Charts
6. Correlation Heatmaps

**Key Analysis Areas:**

1. Distribution of Movies and TV Shows.
2. Release-year distribution of Netflix titles.
3. Relationship between release year and the year content was added to Netflix.
4. Top 10 most frequently listed genres.
5. Comparison of release-year distributions between Movies and TV Shows.
6. Distribution of the five most frequent content ratings.
7. Correlation between release year and year added to Netflix.

### 5️⃣ Date Transformation & Feature Preparation

Additional date-related information was prepared to support the analysis.

* Converted `date_added` into datetime format.
* Extracted the year from `date_added`.
* Created the `year_added` column.
* Compared the original release year with the year content was added to Netflix.

### 6️⃣ Data Visualization

Matplotlib and Seaborn were used to present the analysis through different visual formats.

**Visualizations included:**

* Bar Chart - Content type distribution and top genres.
* Histogram -Distribution of release years.
* Scatter Plot - Release year versus year added.
* Box Plot - Release-year outliers and comparison of content types.
* Pie Chart - Distribution of the five most frequent ratings.
* Correlation Heatmap -Relationship between selected numerical variables.

## 📊 Key Findings

* **Content Type Distribution:** Movies make up a larger proportion of the Netflix catalogue than TV Shows.
* **Release Year Trends:** The release-year distribution highlights how Netflix's catalogue represents content from different periods.
* **Genre Distribution:** Genre analysis reveals the most frequently represented categories across Netflix titles.
* **Content Ratings:** Rating distribution provides an overview of how Netflix titles are classified for different audiences.

## 💡 What We Can Learn from This Project/Recommendations

1. Content creators can explore popular genres to understand the composition of Netflix's content library.
2. Businesses can analyze content distribution to better understand the platform's entertainment catalogue.
3. Comparing release years and content addition dates helps explore Netflix's content acquisition patterns.
4. Data visualization makes it easier to identify trends in content types, genres, ratings, and release years.

## ⚠️ Limitations & Considerations

1. The dataset contains missing information in attributes such as director, cast, and country.
2. The analysis is limited to the information available in the Netflix dataset.
3. The project focuses on data analysis and visualization rather than predicting content popularity or audience engagement.

## 🏁 Conclusion

1. This project successfully analyze and prepared Netflix Movies and TV Shows data by examining missing values, improving data consistency, and transforming date information for analysis.
2. The analysis showed useful patterns in content types, genre distribution, ratings, and release years, demonstrating how data analytics and visualization can help transform raw entertainment data into meaningful insights.
