# 🏠 Airbnb Data Analysis and Visualization

## 📌 Project Overview

This project performs **Exploratory Data Analysis (EDA)** on an Airbnb dataset to uncover patterns in pricing, property characteristics, and booking behavior.
The analysis leverages both **Matplotlib** and **Seaborn** to build visualizations ranging from basic plots to executive-level dashboards.

---

## 🎯 Objectives

* Analyze Airbnb listing characteristics
* Explore pricing behavior across different variables
* Visualize distributions and relationships in the dataset
* Build progressively advanced visualizations
* Generate insights for decision-making and reporting

---

## 🧰 Technologies Used

* **Python 3**
* `pandas` – data manipulation
* `numpy` – numerical operations
* `matplotlib` – basic visualizations
* `seaborn` – advanced and statistical visualizations

---

## 📂 Project Structure

```id="air02"
Airbnb-EDA/
│── AirBNB.csv              # Input dataset
│── Class.ipynb          # Jupyter/Colab notebook
│── README.md               # Documentation
```

---

## ⚙️ Setup Instructions

### 1. Clone Repository

```bash id="air03"
git clone https://github.com/your-username/Airbnb-EDA.git
cd Airbnb-EDA
```

### 2. Install Dependencies

```bash id="air04"
pip install pandas numpy matplotlib seaborn
```

---

## ▶️ Workflow Steps

### 🔹 Step 1: Load Dataset

```python id="air05"
import pandas as pd

df = pd.read_csv("AirBNB.csv")
df.head()
```

---

### 🔹 Step 2: Dataset Variables

Key variables analyzed include:

* `cancellation_policy`
* `room_type`
* `accommodates`
* `log_price`
* `bedrooms`
* `instant_bookable`

---

### 🔹 Step 3: Initial Visualizations (Matplotlib)

* Distribution of **cancellation policy** (bar chart)
* Distribution of **room types** (bar + pie chart)
* **Average price vs accommodates** (line graph)
* **Price distribution** (box plot)
* **Price vs capacity** (scatter plot)

---

### 🔹 Step 4: Enhanced Visualizations (Seaborn)

* Recreate key plots using Seaborn
* Improve aesthetics and readability
* Introduce statistical plotting features

---

### 🔹 Step 5: Advanced Visualizations

* Apply custom styles and palettes:

```python id="air06"
import seaborn as sns
sns.set_style("whitegrid")
sns.set_palette("coolwarm")
```

* Use:

  * `hue` for categorical comparison
  * `kde` for density estimation
  * Multi-variable plotting

---

### 🔹 Step 6: Executive-Level Visualizations

* **Room Type vs Instant Booking Availability**
* **Market Share of Room Types (Pie Chart)**
* **Average Price by Capacity (Line Plot)**
* **Price Distribution (Histogram + KDE)**
* **Price vs Capacity by Room Type (Bubble Scatter Plot)**

---

### 🔹 Step 7: Complex Multi-Variable Analysis

* **Catplot**:

```python id="air07"
sns.catplot(...)
```

* **Price Trends with Variability (Line Plot + Error Bars)**
* **Stacked Histograms for Price Distribution by Room Type**

---

## 📊 Example Insights

* Entire homes/apartments tend to have higher prices
* Listings with more bedrooms generally cost more
* Instant bookable listings show different availability patterns
* Price distributions are often skewed with outliers

---

## ⚠️ Key Notes

* `log_price` is used instead of raw price → interpret carefully
* Outliers may affect visualizations
* Dataset may require preprocessing (missing values, transformations)

---

## 🚀 Future Improvements

* Build **predictive pricing models (ML)**
* Integrate with **Power BI dashboards**
* Perform **geospatial analysis (maps)**
* Automate reporting with **R Markdown / HTML reports**
* Deploy as an interactive dashboard (Streamlit / Dash)

---

## ▶️ How to Run

1. Open the notebook (`Class.ipynb`) in **Jupyter** or **Google Colab**
2. Upload `AirBNB.csv` dataset
3. Run all cells sequentially
4. View generated visualizations

---

## 👤 Author

**Everline** |Data Analyst
