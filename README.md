#  **README — Red Wine Quality Data Analysis (EDA Project)**

##  **Project Title:**

**Exploratory Data Analysis (EDA) on Red Wine Quality Dataset**

---

##  **Project Overview**

This project performs a **complete Exploratory Data Analysis (EDA)** on the **Red Wine Quality dataset**.
The goal is to understand:

* How chemical properties of wine vary
* Which features influence wine quality
* Data distribution, outliers, skewness
* Feature relationships (bivariate correlations)
* Basic feature engineering (labels, log transforms)

No machine learning is used — this project focuses purely on **data understanding**.

---

##  **Dataset Information**

* **File:** `winequality-red.csv`
* **Rows:** 1599
* **Columns:** 12
* **Target variable:** `quality` (rated from 0 to 10)

### Features include:

| Feature              | Description                        |
| -------------------- | ---------------------------------- |
| fixed acidity        | non-volatile acids                 |
| volatile acidity     | acetic acid content                |
| citric acid          | citrus-like taste factor           |
| residual sugar       | remaining sugar after fermentation |
| chlorides            | salt content                       |
| free sulfur dioxide  | free SO2 level                     |
| total sulfur dioxide | total SO2                          |
| density              | density of wine                    |
| pH                   | acidity level                      |
| sulphates            | stabilizer                         |
| alcohol              | % alcohol                          |
| quality              | wine quality rating                |

---

##  **Technologies Used**

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook

---

##  **Project Steps (Pipeline)**

### **✔ Step 1 — Load Dataset**

* Read the CSV with correct delimiter (`;`)
* Preview head, shape, and info

### **✔ Step 2 — Data Cleaning**

* Check missing values
* Check duplicate rows
* Fix delimiter issues
* Convert datatypes if needed

### **✔ Step 3 — Univariate Analysis**

* Histograms
* Boxplots
* Understanding distribution
* Highlighting skewness

### **✔ Step 4 — Outlier Analysis**

* IQR-based outlier detection
* Optional winsorization (capping)

### **✔ Step 5 — Bivariate Analysis**

* Scatterplots
* Variation with target variable (`quality`)
* Boxplots grouped by quality

### **✔ Step 6 — Correlation Analysis**

* Correlation matrix
* Heatmap
* Identify key relationships (Wines with high alcohol = higher quality)

### **✔ Step 7 — Feature Engineering**

* Create **quality_label** (low, medium, high)
* Log-transform skewed features
* Save processed dataset

---

##  **Key Insights**

* No missing values in the dataset
* Several features are **right-skewed** (chlorides, total sulfur dioxide, etc.)
* Outliers present in many continuous features
* Higher **alcohol** content is strongly associated with higher quality
* **Density** is negatively correlated with alcohol
* Free and total sulfur dioxide are highly correlated
* Most wines fall under **medium quality (5 & 6)**

---

##  **Project Files**

```
    Red-Wine-EDA
│
├── winequality-red.csv
├── Red_Wine_EDA.ipynb  (main notebook)
├── winequality-red-processed.csv
├── README.md
└── images/  (optional graphs)
```

---

## **How to Run the Project**

1. Clone the repository:

```
git clone https://github.com/your-username/your-repo-name.git
```

2. Install dependencies:

```
pip install pandas numpy matplotlib seaborn
```

3. Open notebook:

```
jupyter notebook Red_Wine_EDA.ipynb
```

---

## **Author**

**Himanchal mishra**
Engineering Student — NIT Bhopal
Learning Data Analytics & ML

---

## ⭐ **If you like this project, give it a star!**
