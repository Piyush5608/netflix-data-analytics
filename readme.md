# 🎬 Netflix Data Analytics | Python, Pandas, Matplotlib & Plotly

**Exploring Netflix Movies and TV Shows through Data Analysis and Visualization.**

This project focuses on cleaning, analyzing, and visualizing the Netflix Movies and TV Shows dataset using Python. It explores content distribution, country-wise production, release-year trends, audience ratings, and popular genres to discover meaningful patterns and insights.

The project is divided into **5 tasks**, progressing from basic data cleaning to advanced content rating and genre analysis.

---

## 📌 Project Overview

| Project Details | Information |
|---|---|
| Project Name | Netflix Data Analytics |
| Project Type | Exploratory Data Analysis (EDA) |
| Programming Language | Python 3 |
| Data Manipulation | Pandas |
| Data Visualization | Matplotlib, Plotly |
| Development Tools | VS Code / Jupyter Notebook |
| Dataset | Netflix Movies and TV Shows |
| Total Tasks | 5 |

## 🎯 Project Objectives

- Clean and prepare raw Netflix data for analysis.
- Understand the distribution of Movies and TV Shows.
- Identify the leading countries producing Netflix content.
- Analyze content release patterns over the years.
- Explore content ratings, audience categories, and popular genres.
- Generate meaningful insights through data visualization.

---

## 🛠️ Tech Stack

- **Python:** Programming and data analysis.
- **Pandas:** Data cleaning, manipulation, filtering, grouping, and aggregation.
- **Matplotlib:** Static charts and visualizations.
- **Plotly:** Interactive charts and heatmaps.
- **OpenPyXL:** Reading Excel datasets.
- **VS Code / Jupyter Notebook:** Development environment.

---

## 📂 Dataset Information

**Dataset:** Netflix Movies and TV Shows (`netflix_titles`)

The dataset contains information about movies and television shows available on Netflix.

Important columns include:

| Column | Description |
|---|---|
| show_id | Unique ID of each title |
| type | Movie or TV Show |
| title | Name of the content |
| director | Director of the title |
| cast | Actors and actresses |
| country | Country of production |
| date_added | Date the content was added to Netflix |
| release_year | Original release year |
| rating | Content rating |
| duration | Movie duration or TV show seasons |
| listed_in | Genres and categories |
| description | Short description of the content |

---

# 🔍 Project Tasks & Analysis

## Task 1: Netflix Data Cleaning & Preparation

<badge>Easy</badge>

**Objective:** Prepare the raw Netflix dataset by removing inconsistencies and handling missing information before performing analysis.

**What I performed:**

1. Imported the Netflix dataset using Pandas.
2. Checked dataset shape, columns, data types, and missing values.
3. Handled missing values in director, cast, country, and rating by replacing them with `Unknown`.
4. Removed duplicate records.
5. Removed unnecessary whitespace and standardized text values.
6. Corrected records where duration values were incorrectly stored in the rating column.
7. Exported the cleaned dataset into a new CSV file.

**Key Pandas operations:**
`read_excel()`, `isnull()`, `fillna()`, `drop_duplicates()`, `str.strip()`, `to_csv()`.

**Output:** `netflix_cleaned.csv`

**Result:** A cleaned and standardized dataset ready for further analysis.

---

## Task 2: Content Type Analysis – Movies vs TV Shows

<badge>Easy</badge>

**Objective:** Understand the distribution and proportion of Movies and TV Shows available in the Netflix dataset.

**What I performed:**

1. Counted the total number of Movies and TV Shows.
2. Grouped content based on the `type` column.
3. Calculated the percentage distribution of each content type.
4. Compared Movies and TV Shows using visualizations.
5. Interpreted the content distribution to understand which type dominates the catalog.

**Visualizations:**
- Bar Chart – Movies vs TV Shows.
- Pie Chart – Percentage distribution of content types.

**Libraries:** Pandas, Matplotlib.

**Key Finding:** Identifies whether Movies or TV Shows represent the larger share of Netflix's catalog.

---

## Task 3: Country-Wise Netflix Content Analysis

<badge color="info">Medium</badge>

**Objective:** Identify the leading countries contributing to Netflix's content library and compare their content distribution.

**What I performed:**

1. Extracted country information from the dataset.
2. Handled titles associated with multiple countries.
3. Split multiple country entries into individual rows.
4. Counted the number of titles associated with each country.
5. Ranked the top 10 content-producing countries.
6. Compared Movies and TV Shows across the leading countries.
7. Exported the country-wise analysis into a CSV report.

**Visualizations:**
- Top 10 Countries by Content Production.
- Country-Wise Movies vs TV Shows Comparison.

**Output:** `country_ranking_report.csv`

**Libraries:** Pandas, Matplotlib.


**Key Finding:** Identifies the countries with the highest representation in the Netflix dataset.

---

## Task 4: Trend Analysis by Release Year

<badge color="info">Medium</badge>

**Objective:** Understand how Netflix content releases have changed over different years and identify important trends.

**What I performed:**

1. Grouped content by `release_year`.
2. Counted the number of titles released each year.
3. Analyzed yearly content growth.
4. Calculated year-on-year growth to identify increases and decreases.
5. Identified peak release years.
6. Compared release trends for Movies and TV Shows.
7. Visualized the overall content release pattern.

**Visualizations:**
- Overall Content Release Trend.
- Movies vs TV Shows Release Trend.
- Year-on-Year Growth Analysis.

**Libraries:** Pandas, Matplotlib.

**Chart Preview:**

![Netflix Release Year Trend](charts/screenshots/release_year_trend.png)

**Key Finding:** Highlights the years with the highest content representation and shows how the release pattern changes over time.

*Note: The dataset's latest years may show fewer releases because of the dataset's collection cut-off.*

---

## Task 5: Content Rating & Genre Analysis

<badge color="warning">Advanced</badge>

**Objective:** Explore Netflix content ratings, audience categories, and popular genres to understand the types of content represented in the catalog.

**What I performed:**

### A. Content Rating Analysis

1. Examined the distribution of content ratings.
2. Grouped rating categories into audience segments:
   - Kids
   - Family / Older Kids
   - Teens
   - Adults
3. Compared content ratings across Movies and TV Shows.
4. Identified the most frequently occurring rating categories.

### B. Genre Analysis

1. Extracted genre information from the `listed_in` column.
2. Split titles containing multiple genres into individual entries.
3. Counted genre frequency.
4. Identified the most common genres.
5. Compared genre distributions between Movies and TV Shows.

### C. Interactive Visualizations

Created interactive charts using Plotly:

- Content Rating Distribution.
- Top Genres Analysis.
- Movies vs TV Shows Genre Comparison.
- Genre vs Audience Category Heatmap.

**Libraries:** Pandas, Plotly, Matplotlib.

**Key Finding:** Helps identify the most common content ratings, audience categories, and genres represented in Netflix's catalog.

---

## 📊 Key Insights & Findings

The following findings are generated from the analysis:

| Analysis | Insight |
|---|---|
| Content Type | Percentage of Movies vs TV Shows |
| Country Analysis | Top 10 countries by title count |
| Release Trends | Peak content release year |
| Content Ratings | Most common rating category |
| Audience Analysis | Largest audience segment |
| Genre Analysis | Most frequently occurring genres |

---

## 📁 Project Structure

```text
netflix-data-analytics/
│
├── DATASET/
│   ├── Dataset.csv
│   └── netflix_cleaned.csv
│
├── charts/
│   ├── screenshots/
│   │   ├── task2_Movies_TV Shows.png
│   │   ├── task3_country_by_type.png
│   │   ├── task3_top_countries.png
│   │   ├── task4_trend_per_year.png
│   │   ├── task4_trend_by_type.png
│   │   
│
├────TASK/
├──  ├──01_EASY_TASK
├──         ├──task1
├──         ├──task2
├──
├──  ├──02_MEDIUM_TASK
├──         ├──task3
├──         ├──task4
├──
├──  ├──03_ADVANCED_TASK
├──         ├──task5   
│
└── README.md
```


---

## 🚀 Skills Demonstrated

- Python Programming
- Data Cleaning and Preprocessing
- Pandas Data Manipulation
- Data Filtering and GroupBy Operations
- Data Aggregation
- Exploratory Data Analysis (EDA)
- Time Series Trend Analysis
- Data Visualization with Matplotlib
- Interactive Visualization with Plotly
- Analytical Thinking and Business Insights

---

## 👨‍💻 Author

**Piyush Vohra**

B.Tech Computer Science Engineering Student

Aspiring Data Analyst | Python Developer

**Interests:** Python, Data Analytics, SQL, and Data Visualization.

---

⭐ If you find this project interesting, feel free to explore the repository and its visualizations.

**Thank you for visiting!**