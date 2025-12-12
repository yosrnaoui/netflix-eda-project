# 📊 Netflix Movies Exploratory Data Analysis  
**Python for Data Science Portfolio Project**

This project explores Netflix’s catalog of **movies** using Python and performs a full **Exploratory Data Analysis (EDA)**.  
It is designed as a practical portfolio project to demonstrate data cleaning, visualization, and insight generation skills.

Dataset: *Netflix Movies & TV Shows* (public dataset used by DataCamp).

---

## 🚀 Project Objectives

- Clean and preprocess the Netflix dataset  
- Filter and analyze only **movies**  
- Extract insights about movies released in different decades  
- Explore movie durations, genres, countries, and ratings  
- Produce professional data visualizations  
- Summarize findings in a clear conclusions section

---

## 📁 Dataset Overview

The dataset contains:

- **8,807 rows**
- **12 columns**

Key columns include:
- `type` — Movie or TV Show  
- `title` — Movie title  
- `director`  
- `country`  
- `release_year`  
- `rating`  
- `duration`  
- `listed_in` — Genres  
- `description`  

For this project, only **movies** were analyzed.

---

## 🧹 1. Data Cleaning

Steps performed:

- Filtered rows where `type == "Movie"`  
- Converted `date_added` to datetime  
- Extracted movie length in minutes from `duration`  
- Filled missing values in `director`, `country`, and `rating`  
- Created a new `decade` feature:  
  - Example: 2018 → 2010s  
- Removed or normalized inconsistent entries  

---

## 📊 2. Exploratory Data Analysis (EDA)

Key analyses:

### 🔹 **Movies released per decade**
Bar chart showing growth in the number of movies, with a clear dominance of the **2010s**.

### 🔹 **Movie duration distribution**
Most movies fall between **80–120 minutes**, with a strong peak around 90 minutes.

### 🔹 **Most common genres**
Top genres include:
- Dramas  
- Comedies  
- Documentaries  

Genre data was exploded from comma-separated lists.

### 🔹 **Ratings distribution**
Most common categories:
- TV-MA  
- TV-14  
A majority of movies target mature and teen audiences.

### 🔹 **Top movie-producing countries**
The United States dominates, followed by:
- India  
- UK  
- Japan  
- Various European countries  

### 🔹 **Most prolific directors**
Most movies have unique directors.  
“Unknown” appears often due to missing metadata.

---

## 🧠 3. Key Insights

- Netflix’s catalog is heavily focused on **modern movies**, especially from the **2010s**.  
- Content diversity is high, with strong international representation.  
- Movies tend to follow a standard length between 1h20 and 2h.  
- Drama, comedy, and documentary genres are the most abundant.  
- Ratings distribution suggests Netflix prioritizes **teen and adult** audiences.

---

## 🛠️ Technologies Used

- Python  
- pandas  
- numpy  
- matplotlib  
- seaborn  
- Google Colab

---

## ▶️ How to Run the Project

1. Clone the repository:
   ```bash
   git clone https://github.com/yosrnaoui/netflix-eda-project.git
   cd netflix-eda-project
2. Open the notebook: colab notebook netflix_eda.ipynb
3. Make sure the dataset (netflix_titles.csv) is placed inside the data/ folder.
4. Run all cells to reproduce the analysis.

---

⭐ Future Improvements
Build a movie recommendation system

Cluster movies by genre/duration

Predict movie rating or popularity

Interactive visualizations (Plotly / Dash)


