# 📱 Google Play Store Data Analysis

## 📌 Project Overview

This project analyzes the **Google Play Store dataset** using **Python and Pandas** to understand app ratings, reviews, categories, pricing, and installation patterns.

The project focuses on **data cleaning, missing-value handling, data formatting, exploratory data analysis (EDA), and extracting useful insights** from the dataset.

---

## 🎯 Objectives

The main objectives of this project are:

* Clean and prepare the Google Play Store dataset.
* Handle missing values appropriately.
* Convert columns into suitable data types.
* Analyze app ratings and reviews.
* Compare free and paid applications.
* Identify highly rated app categories.
* Find apps with the highest number of reviews and installations.
* Extract useful insights from the Play Store data.

---

## 🛠️ Technologies Used

* **Python**
* **Pandas**
* **NumPy**
* **Jupyter Notebook**

---

## 📂 Dataset

The project uses the **Google Play Store Apps dataset**, available in CSV format.

The dataset contains information such as:

* App name
* Category
* Rating
* Reviews
* Size
* Installs
* Type
* Price
* Content Rating
* Genres
* Last Updated
* Current Version
* Android Version

---

## 🔧 Data Cleaning

The following preprocessing steps were performed:

### Missing Values

Missing values were identified using:

```python
df.isnull().sum()
```

The following approaches were used:

* Missing **Rating** values were replaced with the mean rating.
* Missing **Current Ver** values were replaced with `Varies with device`.
* Missing **Android Ver** values were replaced with `4.1 and up`.
* Missing **Content Rating** values were replaced with `Everyone`.
* Remaining rows containing missing values were removed.

A backup of the original DataFrame was also created before modification.

```python
df_backup = df.copy()
```

### Data Type Formatting

The `Reviews` column was converted into a numeric format:

```python
df['Reviews'] = df['Reviews'].astype('float')
```

---

## 📊 Analysis Performed

The notebook performs several exploratory analyses, including:

### 🔹 Apps Containing "Astrology"

The project checks the number of applications containing **"Astrology"** in their title.

**Result:** 3 apps were identified.

### 🔹 Average App Rating

The overall average rating calculated in the notebook is approximately:

**4.19**

### 🔹 Rating by Category

The average rating of applications was calculated for each category.

The notebook identifies **Education** as having the highest average rating and **Dating** as having the lowest average rating.

### 🔹 Five-Star Applications

The analysis identifies applications with a rating of exactly **5.0**.

**Result:** 274 apps have a five-star rating.

### 🔹 Average Number of Reviews

The average number of reviews per application was calculated.

**Result:** Approximately **444,152 reviews per app** on average.

### 🔹 Free vs Paid Applications

The project compares the number of free and paid applications.

| App Type | Number of Apps |
| -------- | -------------: |
| Free     |         10,038 |
| Paid     |            799 |

### 🔹 Free vs Paid Ratings

The average rating was compared between free and paid applications using:

```python
df.groupby('Type')['Rating'].mean()
```

The notebook observes that paid applications have a higher average rating than free applications.

### 🔹 Most Reviewed Applications

The project identifies applications with the highest number of reviews using sorting on the `Reviews` column.

### 🔹 Top Installed Applications

The notebook also analyzes the applications with the highest installation counts.

---

## 📈 Key Insights

Some of the insights obtained from the analysis include:

* The average Play Store app rating is approximately **4.19**.
* **Education** has the highest average category rating in the analysis.
* **Dating** has the lowest average category rating in the analysis.
* **274 applications** have a perfect 5-star rating.
* The dataset contains significantly more **free applications** than paid applications.
* Paid applications have a higher average rating than free applications in this analysis.
* The project identifies the most reviewed and highly installed applications.

---

## 📁 Project Structure

```text
Google-Play-Store-Data-Analysis/
│
├── project 09 playstore data analysis.ipynb
├── googleplaystore.csv
└── README.md
```

---

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone <your-github-repository-url>
```

### 2. Install the required libraries

```bash
pip install pandas numpy jupyter
```

### 3. Open the notebook

```bash
jupyter notebook
```

Then open:

```text
project 09 playstore data analysis.ipynb
```

### 4. Update the dataset path

Change the CSV file path in the notebook to the location of your downloaded dataset.

---

## 💡 Skills Demonstrated

This project demonstrates practical experience with:

* Data Cleaning
* Missing Value Handling
* Data Type Conversion
* Exploratory Data Analysis
* Pandas DataFrames
* GroupBy Operations
* Sorting and Filtering
* Descriptive Statistics
* Data Analysis using Python
* Extracting Business Insights

---

## 👨‍💻 Author

**Prajwal NK**

Electronics & Communication Engineering | Data Analytics Enthusiast

---

⭐ If you find this project useful, consider giving the repository a star!
