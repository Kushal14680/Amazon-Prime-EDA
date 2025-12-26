# Amazon Prime TV Shows and Movies – Exploratory Data Analysis (EDA)

## 📌 Project Overview
This project performs an **Exploratory Data Analysis (EDA)** on Amazon Prime Video’s catalog of TV shows and movies available in the United States. The objective is to extract meaningful insights related to **content diversity, trends over time, audience ratings, popularity, and production characteristics** to support data-driven business decisions in the streaming industry.

---

## 🎯 Business Objective
To analyze Amazon Prime Video’s content library and identify patterns that can help guide:
- Content investment strategies  
- Platform growth and retention decisions  
- Understanding of audience preferences  

---

## 📂 Dataset Description
The analysis uses two datasets:

### 1. `titles.csv`
Contains metadata for movies and TV shows:
- `id`, `title`, `type`, `description`
- `release_year`, `runtime`, `seasons`
- `genres`, `production_countries`
- `age_certification`
- `imdb_score`, `imdb_votes`
- `tmdb_score`, `tmdb_popularity`

### 2. `credits.csv`
Contains cast and crew information:
- `person_id`
- `id` (title ID)
- `name`
- `character`
- `role` (ACTOR / DIRECTOR)

---

## 🛠️ Tools & Libraries Used
- **Python**
- **Pandas** – Data manipulation
- **NumPy** – Numerical operations
- **Matplotlib & Seaborn** – Data visualization
- **SciPy** – Statistical hypothesis testing
- **Scikit-learn** – Pipeline-based data wrangling (custom transformers)

---

## 🔄 Project Workflow
1. Understanding the problem statement  
2. Dataset loading and inspection  
3. Initial data wrangling (duplicates, missing values, data types)  
4. Variable understanding and statistical summary  
5. Data visualization (univariate & bivariate analysis)  
6. Hypothesis testing  
7. Business insights and recommendations  
8. Final conclusion  

---

## 🧹 Data Wrangling (Initial Cleaning)
Minimal but necessary cleaning was performed to make the data usable for EDA:
- Removed duplicate records  
- Standardized column names  
- Corrected obvious data types  
- Handled structural missing values (e.g., seasons for movies, character for directors)  
- Performed minimal dataset merging where required  

> 📌 The goal was **exploratory readiness**, not model-level preprocessing.

---

## 📊 Data Visualization & Key Insights
- **14 visualizations** were created using multiple chart types:
  - Bar charts
  - Histograms
  - Scatter plots
  - Box plots
  - Heatmaps
  - Pair plots

### Key Insights:
- TV shows generally have higher average ratings than movies  
- Ratings across IMDb and TMDB are strongly correlated  
- Popularity is driven by a small number of titles  
- Content quality matters more than runtime or production scale  
- Multi-season shows tend to maintain better audience reception  

---

## 📈 Hypothesis Testing
Three statistically sound hypotheses were tested using:
- **Independent two-sample t-tests**
- **Pearson correlation tests**

These tests validated insights related to:
- Ratings differences between movies and TV shows  
- Cross-platform rating consistency  
- Relationship between content longevity and quality  

---

## 💡 Business Recommendations
- Invest more in **high-quality episodic content**  
- Use cross-platform ratings for content evaluation  
- Balance marketing efforts with content quality  
- Avoid over-reliance on short-term popularity spikes  

---

## ✅ Conclusion
The exploratory analysis reveals that Amazon Prime Video’s catalog is diverse, recent, and popularity-driven, but long-term engagement is better supported by **high-quality, multi-season TV content**. The dataset is well-structured, with missing values largely contextual, making it suitable for reliable analysis. The insights derived can help guide strategic decisions in content acquisition, renewal

