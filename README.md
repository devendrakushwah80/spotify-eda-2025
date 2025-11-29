# 🎵 Spotify 2025 Tracks – Exploratory Data Analysis (EDA)

## 📌 Overview
This project performs **Exploratory Data Analysis (EDA)** on a Spotify dataset containing mainly **modern and contemporary tracks from 2025**.  
The objective is to understand track popularity, artist dominance, and relationships between numeric features using summary statistics and visualizations.

All findings in this project are derived **only from EDA** using **bar charts, histograms, and a correlation heatmap**.  
No machine learning or predictive modeling is applied.

---

## 📂 Dataset

### `spotify_data_clean.csv`
- **Rows:** 8,582  
- **Columns:** 15  
- **Time Period:** Mostly 2025  
- **Granularity:** Each row represents one Spotify track  

#### Key Fields Used
- `artist_name`
- `artist_genres`
- `artist_popularity`
- `artist_followers`
- `track_popularity`
- `track_number`
- Other numeric features used in correlation analysis

> ✅ This dataset was used **only for EDA purposes**.

---

## 🧹 Data Exploration & Cleaning

The following steps were performed in the notebook:

- Inspected dataset shape, columns, and data types
- Used `head()`, `tail()`, `info()`, and `describe()` for structure and statistics
- Checked for:
  - Missing values
  - Duplicate rows
  - Unique values per column
- Handled missing values:
  - `artist_name` filled with `"Unknown"`
  - `artist_genres` filled with `"Unknown"`
- Cleaned text data in `artist_name`:
  - Converted to string
  - Removed special characters using regex to ensure proper grouping

---

## 📊 Visualizations & Insights

All insights below are based solely on the graphs generated in the notebook.

---

### 1️⃣ Top 20 Artists by Average Popularity
**Visualization:** Bar chart  

**Insight:**
- Shows artists with the highest mean popularity scores
- Reveals that popularity is concentrated among a small group of dominant artists
- Highlights consistently high-performing artists on Spotify

---

### 2️⃣ Distribution of Track Popularity
**Visualization:** Histogram with KDE  

**Insight:**
- Track popularity is not evenly distributed
- Most songs fall in the mid-range popularity scores
- Highly popular tracks are comparatively fewer

---

### 3️⃣ Correlation Heatmap of Numeric Features
**Visualization:** Correlation heatmap  

**Insight:**
- Displays positive and negative correlations among numeric attributes
- Helps identify features that move together
- Provides understanding of data structure for future analysis

---

### 4️⃣ Top 20 Artists by Average Track Number
**Visualization:** Bar chart  

**Insight:**
- Indicates how artists’ tracks are positioned within albums or collections
- Artists with higher average track numbers often appear later in releases
- Adds structural perspective to artist releases

---

### 5️⃣ Top 20 Artists by Followers
**Visualization:** Bar chart  

**Insight:**
- Highlights artists with the largest listener base on Spotify
- Useful for comparing artist reach versus popularity-based rankings
- Shows platform influence of top artists

---

## 🧠 Key Takeaways
- The dataset is mostly clean and suitable for exploratory analysis
- Popularity and followers are concentrated among top artists
- Track popularity shows a skewed distribution
- Numeric features exhibit varying degrees of correlation
- All conclusions are supported **only by EDA visualizations**

---

## 🎯 Use Cases
- Learning Exploratory Data Analysis (EDA)
- Music data visualization
- Data analytics portfolio projects
- Understanding modern music trends

---

## 📜 License
**CC0 – Public Domain**

---

## 🙏 Acknowledgment
Data collected from **Spotify’s public API**  
Used only for **educational and research purposes**
