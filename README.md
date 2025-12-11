# 🎬 Netflix Catalog Analysis: A Power BI Dashboard
<img width="918" height="516" alt="Netflix Report " src="https://github.com/user-attachments/assets/6eb15feb-3bc1-447f-922b-cbb4c3636c84" />

This project presents a comprehensive analysis of the **global Netflix content catalog**, visualized through an interactive **Power BI dashboard**. The goal of this project is to explore how Netflix's content library has evolved over time by examining trends in **content growth**, **content type distribution**, **ratings**, **geographical coverage**, and **genre popularity** from **1925 to 2020**.

---

## 📌 Key Project Metrics

The dashboard highlights several high-level statistics describing the size and scope of Netflix’s catalog:

* **Total Titles:** 6,169
* **Locations Covered:** 555
* **Total Genres:** 462
* **Data Span:** 1925 – 2020

---

## 📊 Data Insights & Visualization

The dashboard provides rich insights into Netflix’s catalog. Key findings from each visual include:

### **1. Content Type Distribution**

* Movies make up the majority of the catalog with **4.27K titles (68.42%)**.
* TV Shows account for **1.97K titles (31.58%)**.
* This is illustrated by a donut chart clearly showing movies as the dominant category.

### **2. Ratings Distribution (Top 7 Categories)**

* **TV-MA** is the most common rating with **2,027 titles**.
* **TV-14** follows with **1,698 titles**.
* Other significant categories include:

  * **TV-PG — 700 titles**
  * **TV-Y — 508 titles**
  * **PG-13 — 286 titles**
* The horizontal bar chart highlights the strong presence of mature-rated content on the platform.

### **3. Top Contributing Countries**

From the treemap visualization:

* The **United States** contributes the largest proportion of titles with **2.03K**.
* Other top countries include:

  * **India — 0.78K**
  * **Japan — 0.35K**
  * Contributions also visible from countries like Canada, Spain, and Turkey.

### **4. Content Growth Over Time**

* The line chart ("Total Movies and TV Shows By Year") shows **slow and steady growth** from 1925 to 2000.
* Around the early 2000s, title additions increase **exponentially**, peaking just before 2020.
* This reflects Netflix’s rapid expansion and aggressive content acquisition strategy.

### **5. Top Genres by Total Titles**

Based on the bar chart:

* **Documentaries — 299**
* **Stand-Up Comedy — 273**
* **Dramas / International Movies / Independent Films — 248**
* **Comedies — 186**
* These genres represent the core pillars of Netflix’s catalog volume.

### **6. Ratings Breakdown (Donut Chart)**

* The ratings pie chart reinforces the findings of the bar chart:

  * **TV-14 (24.09%)** is the largest slice.
  * **TV-MA (22.09%)** closely follows.
* These two categories combined represent nearly half of all titles on the platform.

---

## 🛠️ Data Source & Preparation

### **Data Source**

The dataset used for this project is sourced from publicly available Netflix catalog data, commonly found on platforms such as **Kaggle** or similar open-data repositories. The dataset includes details about:

* Title name
* Release year
* Ratings
* Genres
* Contributing countries
* Content type (Movie / TV Show)

### **ETL Process (Power Query Editor)**

A structured data cleaning and transformation workflow was performed:

1. **Data Cleaning**

   * Removed duplicates and handled null or incomplete fields.
   * Standardized inconsistent entries in categorical columns (e.g., ratings, countries).

2. **Data Transformation**

   * Split multi-value fields such as *country* and *listed_in (genres)* into separate rows to support many-to-many modeling.
   * Converted date columns to proper date formats.
   * Normalized text fields for consistency.

3. **Data Loading**

   * Final cleaned data was loaded into the Power BI data model as dimension and fact tables.
   * Relationships were built to support accurate cross-filtering in visuals.

---

## 🧰 Tools & Technologies Used

* **Power BI Desktop** – for dashboard design, modeling, and visualization.
* **Power Query (M Language)** – for data extraction, transformation, and cleaning.
* **DAX (Data Analysis Expressions)** – for calculated measures such as:

  * *Total Titles*
  * *Total Genres*
  * *Content Type Counts*
  * Time-intelligence calculations

---
