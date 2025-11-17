<h1 align="center">🎬 Netflix EDA Project</h1>
<p align="center">An end-to-end Exploratory Data Analysis using Python, Regex, Kaggle Dataset & Jupyter Notebook</p>

<p align="center">
  <!-- Badges -->
  <img src="https://img.shields.io/badge/Notebook-Jupyter-orange?style=for-the-badge&logo=jupyter" />
  <img src="https://img.shields.io/badge/Language-Python-blue?style=for-the-badge&logo=python" />
  <img src="https://img.shields.io/badge/Dataset-Kaggle-20BEFF?style=for-the-badge&logo=kaggle" />
  <img src="https://img.shields.io/badge/Library-Pandas-150458?style=for-the-badge&logo=pandas" />
  <img src="https://img.shields.io/badge/Visualization-Matplotlib-0C63E7?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Regex-Used-success?style=for-the-badge" />
</p>

---

# 📌 **Project Overview**

This project performs a complete **Exploratory Data Analysis (EDA)** on the **Kaggle Netflix Titles Dataset**, focusing on:

- 🔧 **Data cleaning**  
- 🧵 **Regex-based extraction**  
- 🔍 **Feature engineering**  
- 📊 **Visualization**  
- 🧠 **Insight generation**  
- 📁 **Cleaned dataset export**  

Executed entirely in a **Jupyter Notebook**, this project showcases essential Data Analyst and Data Science skills.

Dataset includes movies & TV shows, with metadata such as cast, director, country, ratings, duration, and more.

---

# 📁 **Dataset**
**Source:** Kaggle – *Netflix Movies and TV Shows*  
This dataset contains all titles available on Netflix up to the upload date.

---

# 🎯 **Project Goals**
- Clean raw Netflix metadata  
- Handle missing, inconsistent, and multi-valued fields  
- Extract structured features using **Regex**  
- Analyze global content trends  
- Identify patterns in ratings, genres, countries, actors & directors  
- Visualize insights using aesthetic, clean graphs  

---

# 🧹 **Data Cleaning Steps**

### ✔ Column normalization  
- Lowercase all column names  
- Replace spaces with underscores  
- Trim whitespace  

### ✔ Missing value handling  
- Clean missing cast, director, rating, country  
- Remove or extract meaningful rows  

### ✔ Datetime conversions  
- Converted `date_added` to datetime  
- Extracted:
  - `added_year`
  - `added_month`

### ✔ Duration extraction using **Regex**

Regex patterns used:

```
(\d+)\s*min
(\d+)\s*Season
```

Extracted:
- `duration_minutes` for Movies  
- `seasons` for TV Shows  

### ✔ Multi-value normalization
Using `.str.split()` and `.explode()` for:
- Cast  
- Director  
- Genres  
- Country  

---

# 🔧 **Feature Engineering**

| Feature | Description |
|--------|-------------|
| `duration_minutes` | Numeric movie runtime |
| `seasons` | Number of seasons |
| `primary_genre` | First listed genre |
| `primary_country` | First listed country |
| `added_year` | Year added to Netflix |
| `added_month` | Month added |

---

# 📊 **Visualizations Included**

All visualizations use clean & aesthetic Matplotlib themes.

- ⭐ Movies vs TV Shows  
- ⭐ Rating distribution  
- ⭐ Top genres (Movie & TV separately)  
- ⭐ Top 20 countries  
- ⭐ Top actors & directors (post-explode)  
- ⭐ Duration distribution  
- ⭐ Boxplot for outlier detection  
- ⭐ Monthly & yearly addition trends  
- ⭐ Genre heatmaps (optional)

---

# 🔍 **Key Insights**

### ⭐ Content Type  
Netflix has significantly **more Movies than TV Shows**.

### ⭐ Ratings  
Most content is rated **TV-MA** → Netflix focuses heavily on mature audience content.

### ⭐ Country  
The **United States** leads content contribution, followed by **India**, UK, and Japan.

### ⭐ Genres  
Drama & International Movies dominate, while Kids & Reality genres dominate TV.

### ⭐ Duration  
Most movies lie between **80–110 minutes** — standard cinematic length.

### ⭐ Actors & Directors  
Exploded lists reveal a small group of recurring actors and directors responsible for many Netflix titles.

---

# 🛠 **Tech Stack**

### **Languages**
- Python  

### **Libraries**
- Pandas  
- NumPy  
- Matplotlib  
- Regex (`re` module)  
- Jupyter Notebook  

### **Platform**
- Kaggle (dataset source)  
- GitHub (version control & hosting)

---

# 📁 **Project Structure**

```
Netflix-EDA/
│
├── notebooks/
│   └── netflix_eda.ipynb          # main analysis notebook
│
├── data/
│   └── netflix_cleaned.csv        # cleaned dataset
│
├── images/
│   └── *.png                      # exported charts
│
├── README.md
├── requirements.txt
└── .gitignore
```

---

# 🚀 **How to Run**

```bash
git clone https://github.com/riyagoyal08010-glitch/Netflix_EDA_Project.git
cd Netflix_EDA_Project
pip install -r requirements.txt
jupyter notebook notebooks/NetflixEDA_Project.ipynb
```

---

# 📦 **requirements.txt (Minimal)**

```
pandas
numpy
matplotlib
seaborn
jupyter
wordcloud
```

---

# 🔚 **Conclusion**

This Netflix EDA project demonstrates core data analytics skills —  
**data cleaning, regex extraction, feature engineering, visualization, and storytelling** —  
all built in **Jupyter Notebook** using the **Kaggle Netflix dataset**.

It serves as a strong portfolio piece for Data Analyst / ML / Data Science internships.

