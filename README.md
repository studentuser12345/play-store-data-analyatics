# 📱 Google Play Store Data Analysis

## 📌 Project Overview

This project analyzes the **Google Play Store dataset** using Python and Pandas to understand app categories, ratings, reviews, pricing, installations, and other app characteristics.

The analysis focuses on **data cleaning, preprocessing, exploratory data analysis (EDA), and extracting meaningful insights** from the dataset.

---

## 🎯 Objectives

* Analyze the distribution of apps across different categories.
* Understand app ratings and review patterns.
* Compare **free and paid applications**.
* Identify highly reviewed and highly installed apps.
* Analyze app categories based on average ratings.
* Explore content ratings, pricing, and installation trends.
* Extract useful insights from the Play Store dataset.

---

## 📊 Dataset

The dataset contains **10,841 rows and 13 columns** before cleaning.

After preprocessing, the final dataset contains **10,840 rows and 13 columns**.

### Dataset Features

| Column           | Description                 |
| ---------------- | --------------------------- |
| `App`            | Application name            |
| `Category`       | App category                |
| `Rating`         | App rating                  |
| `Reviews`        | Number of reviews           |
| `Size`           | Application size            |
| `Installs`       | Number of installations     |
| `Type`           | Free or Paid                |
| `Price`          | Application price           |
| `Content Rating` | Target audience             |
| `Genres`         | App genre                   |
| `Last Updated`   | Last update date            |
| `Current Ver`    | Current application version |
| `Android Ver`    | Required Android version    |

---

## 🛠️ Technologies Used

* **Python 3.9**
* **Pandas**
* **NumPy**
* **Jupyter Notebook**
* **Matplotlib / Seaborn**

---

## 🔄 Data Analysis Workflow

```text
Dataset
   ↓
Data Loading
   ↓
Data Inspection
   ↓
Missing Value Detection
   ↓
Data Cleaning
   ↓
Data Type Conversion
   ↓
Exploratory Data Analysis
   ↓
Grouping & Aggregation
   ↓
Insight Extraction
```

---

## 🧹 Data Cleaning

The dataset initially contained missing values in several columns.

### Missing Values Identified

* `Rating` → **1,474**
* `Type` → **1**
* `Content Rating` → **1**
* `Current Ver` → **8**
* `Android Ver` → **3**

### Handling Strategy

* Missing `Rating` values were replaced using the **mean rating**.
* Missing categorical values were replaced using their **most frequent values**.
* The remaining missing record was removed using `dropna()`.
* `Reviews` was converted from object/string format to a numeric data type.

After cleaning:

**10,840 rows × 13 columns**

---

## 📈 Key Analysis & Findings

### ⭐ Average App Rating

The average app rating in the cleaned dataset is approximately:

**4.19 / 5**

---

### 🏆 Category Rating Analysis

The project calculated the average rating for each of the **34 app categories**.

Examples:

| Category          | Average Rating |
| ----------------- | -------------: |
| Education         |          4.388 |
| Events            |          4.364 |
| Art & Design      |          4.350 |
| Books & Reference |          4.311 |
| Game              |          4.283 |
| Dating            |          4.008 |

---

### ⭐ Five-Star Apps

The analysis identified:

**274 apps with a 5.0 rating.**

---

### 💬 Review Analysis

The average number of reviews per app was approximately:

**444,153 reviews**

The maximum review count in the dataset was:

**78,158,306 reviews**

The app associated with this maximum was **Facebook**.

---

### 💰 Free vs Paid Apps

The dataset contains:

* **10,039 Free apps**
* **800 Paid apps**

Average ratings:

| App Type | Average Rating |
| -------- | -------------: |
| Free     |          4.187 |
| Paid     |          4.253 |

---

### 📥 Highly Installed Apps

The analysis examined the most-installed applications, including:

1. Temple Run 2
2. Google Duo - High Quality Video Calls
3. Viber Messenger
4. Google Calendar
5. Dropbox

---

### 🔮 Astrology Apps

The analysis searched application names containing **"Astrology"** and identified:

**3 applications**

---

## 📊 Statistical Analysis

Descriptive statistics were performed on the dataset to examine:

* Mean
* Median
* Standard deviation
* Minimum and maximum values
* Unique values
* Frequency distributions

For example, the median number of reviews was approximately **2,094**, while the 75th percentile was approximately **54,776 reviews**.

---

## 💡 Key Insights

* The Play Store dataset contains apps across **34 different categories**.
* The majority of applications are **free**, with 10,039 free apps compared with 800 paid apps.
* The overall average app rating is approximately **4.19**.
* **274 apps** achieved a perfect 5.0 rating.
* Education had an average rating of approximately **4.39**.
* Facebook recorded the highest number of reviews in the analyzed dataset.
* The analysis demonstrates how ratings, reviews, pricing, categories, and installations can be explored using Python.

---

## 📁 Project Structure

```text
Google-Playstore-Data-Analysis/
│
├── data analysis.ipynb
├── googleplaystore.csv
└── README.md
```

---

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone <your-repository-url>
```

### 2. Install dependencies

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### 3. Open Jupyter Notebook

```bash
jupyter notebook
```

### 4. Open

```text
data analysis.ipynb
```

Run the notebook cells sequentially to reproduce the analysis.

---

## 📌 Skills Demonstrated

**Python | Pandas | NumPy | Data Cleaning | Data Preprocessing | EDA | Data Analysis | Data Visualization | Statistical Analysis | Jupyter Notebook**

---

## 👤 Author

**Prajwal NK**

Electronics & Communication Engineering | Data Analytics & Python

---

## ⭐ Project Highlights

**10,840 cleaned records | 13 features | 34 categories | 274 five-star apps | 10,039 free apps | 800 paid apps | 444K average reviews**
