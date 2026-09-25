# 📊 Salary & Startup Funding Analysis — India

A two-part exploratory data analysis (EDA) project using **Python (Pandas, Matplotlib, Seaborn)** to uncover insights from real-world datasets on **Indian software professionals' salaries** and **Indian startup funding**.

This project was built as a final assignment to practice core data analyst skills: data cleaning, aggregation, merging, API integration, and data visualization.

---

## 🎯 Project Overview

| | |
|---|---|
| 🧩 **Part 1** | Analyze salaries, ratings, and job roles of 20k+ software professionals |
| 🚀 **Part 2** | Analyze Indian startup funding trends (2019–2021) and connect them to salary/rating data |
| 🛠️ **Tools** | Python, Pandas, Matplotlib, Seaborn, REST API |
| 📁 **Data** | Kaggle datasets (CSV) |

---

## 📁 Repository Structure

```
├── data/
│   ├── Software Professionals Salary.csv
│   ├── startup_funding2019.csv
│   ├── startup_funding2020.csv
│   └── startup_funding2021.csv
├── x_a1_12_Final_Assignment_P1.ipynb   # Part 1 - Salary Analysis
├── x_a2_Final_Assignment_P2.ipynb      # Part 2 - Startup Funding Analysis
└── README.md
```

---

## 🧩 Part 1 — Software Professionals Salary Analysis

Explored a dataset of **20,000+ software professionals** in India, including company ratings, job titles, salaries (₹), and locations.

**Key steps & questions answered:**
- 🔍 Explored dataset shape, unique job roles, and job titles
- 🐍 Filtered and counted "Python" role Analysts by company
- 🏢 Identified the company with the most salaries reported (**Amazon**) and how many locations it operates in
- 💱 **Converted salaries from INR to USD** in real time using the [ExchangeRate-API](https://www.exchangerate-api.com/docs/free)
- 📈 Calculated average USD salary by job role and by company
- 📊 Visualized the relationship between **Rating vs. Salary (USD)** and identified a salary outlier company

**Skills demonstrated:** data filtering, `groupby()` aggregation, API integration, currency conversion, data visualization, outlier detection

---

## 🚀 Part 2 — Indian Startup Funding Analysis

Combined **three years of startup funding data (2019–2021)** to explore investment trends across Indian cities.

**Key steps & questions answered:**
- 🔄 Merged 3 yearly CSV files into a single DataFrame using a `for` loop, tagging each row with its `Year`
- 🧹 Cleaned and converted `Founded`, `Amount($)`, and `Year` columns to numeric types, handling missing values
- 🏆 Ranked investors by number of companies funded (e.g., *Inflection Point Ventures*) — overall and by year
- 🌆 Built a **city-level comparison** by merging salary/rating data (Part 1) with 2021 funding data on `Location`/`HeadQuarter`
- 📉 Created a **scatterplot** comparing average salary vs. total funding received per city, highlighting the standout city

**Skills demonstrated:** multi-file ingestion, data type conversion, missing-value handling, advanced `groupby()` + ranking, DataFrame merging, cross-dataset analysis, visualization

---

## 🛠️ Tech Stack

- 🐼 **Pandas** — data wrangling & aggregation
- 📉 **Matplotlib** & **Seaborn** — data visualization
- 🌐 **Requests** — live currency conversion via REST API
- 📓 **Jupyter Notebook**

---

## ▶️ How to Run

1. Clone this repository
   ```bash
   git clone <your-repo-url>
   cd <repo-name>
   ```
2. Install the required libraries
   ```bash
   pip install pandas matplotlib seaborn requests
   ```
3. Open the notebooks in Jupyter and run the cells in order
   ```bash
   jupyter notebook
   ```

---

## 💡 Key Takeaways

- 💰 Salary and company rating show a generally positive relationship, with a few notable outliers
- 🏙️ Certain cities combine both high average salaries *and* high startup funding — a signal of strong tech ecosystems
- 📊 Ranking investors by year reveals shifts in activity that a single overall ranking would hide

---

## 👤 About Me

I'm a junior data analyst building hands-on experience with Python and real-world datasets. This project reflects my growing skills in **data cleaning, exploratory analysis, and storytelling with data**.

📫 Feel free to connect with me on [LinkedIn](#) or check out more of my projects on [GitHub](#)!

---

⭐ If you found this project interesting, consider giving it a star!
