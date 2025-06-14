# Titanic Survival Exploratory Data Analysis (EDA)

This project explores the **Titanic dataset** using Python and popular data science libraries. The goal of this EDA is to understand the structure of the data, identify relationships between features, and gain insights that can inform predictive modeling.

---

## 📁 Dataset

- Source: https://www.kaggle.com/datasets/mdrabbiali/titanic-data-set

---

## 📊 EDA Steps

### 0. **Data Loading**
- Loaded the dataset into a Pandas DataFrame.

### 1. **Loading the data**
- Checked the shape and data types.
- Used `.info()` and `.describe()` for summary statistics.

### 2. **Cleaning the Data**
- Dropped and handled missing columns (e.g., dropped `'Cabin'`, handled missing `'Age'` replacing it with median).

### 3. **Univariate Analysis**
- Plotted distributions of features like:
  - `Age`
  - `Fare`
  - `Survived`

### 4. *Bivariate Analysis (Survival vs. Features)**
- Used bar plots and box plots to examine survival rates against:
  - `Sex`
  - `Pclass`

### 5. **Outlier Detection**
- Used boxplot to detect outliers in:
  - `Fare`
  - `Age`

### 6. **Correlation Analysis**
- Selected only numerical columns.
- Plotted a **heatmap** of the correlation matrix to identify strong relationships.
  - Notable findings:
    - `Fare` is positively correlated with `Survived`.
    - `Pclass` is negatively correlated with both `Survived` and `Fare`.

---

## 📌 Libraries Used

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`

---

## 🔍 Key Insights

* **Gender significantly impacted survival:** Female passengers consistently showed a much higher survival rate compared to males.
* **Passenger class correlated with survival:** Individuals in **1st class** were considerably more likely to survive than those in **2nd or 3rd class**.
* **Fare and survival had a positive link:** A higher fare paid for a ticket appears to correlate with a greater chance of survival. This might be due to the correlation between fare and passenger class or potentially better cabin locations.
* **Age's impact on survival was weak:** While there was a slight negative correlation between age and survival, it suggests that **children might have been prioritized** in rescue efforts.




