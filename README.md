# EDA with Sweetviz & D-Tale

An exploratory data analysis project exploring how Python tools such as **Sweetviz** and **D-Tale** can make the initial EDA process faster and more interactive.

The project uses a customer churn dataset containing **10,000 records and 12 features**.

---

## 📌 Project Overview

Exploratory Data Analysis (EDA) is an important part of any data analysis or machine learning workflow.

Traditionally, EDA often involves writing repetitive code using libraries such as Pandas, Matplotlib, and Seaborn.

In this project, I explored two Python tools that can help accelerate the initial exploration process:

* **Sweetviz** — automated visual EDA
* **D-Tale** — interactive DataFrame exploration

The goal was not simply to generate charts, but to understand:

> **How much of the initial EDA process can be accelerated using automated and interactive Python tools?**

---

## 📊 Dataset

The dataset contains:

* **10,000 records**
* **12 features**
* Customer-related information
* A `churn` target variable

The dataset was explored for data quality, distributions, categorical patterns, missing values, and potential anomalies.

---

## 🛠️ Tools & Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Sweetviz
* D-Tale
* Jupyter Notebook

---

## 🔍 EDA Findings

Some of the observations from the initial exploration included:

### Missing Values

Around **3% missing values** appeared in several columns.

In particular:

* `age` → approximately 300 missing values
* `satisfaction_score` → approximately 300 missing values

---

### Potential Extreme Values

The `monthly_charges` column showed a potentially unusual value:

* Maximum = **446**
* 95th percentile = **112**

This large difference suggests that the extreme values should be investigated further rather than automatically removed.

---

### Distribution

`support_calls` showed a **right-skewed distribution**.

This can be useful when deciding which statistical techniques or transformations may be appropriate for further analysis.

---

### Categorical Distribution

`contract_type` was dominated by **Month-to-month** customers.

This provides an interesting starting point for investigating customer behavior and churn.

---

### Churn Distribution

The `churn` variable was imbalanced, with **No** representing the majority class.

This is an important observation if the dataset is later used for predictive modeling.

---

## 📈 Sweetviz

Sweetviz was used to generate an automated visual overview of the dataset.

It helped provide a quick view of:

* Variable distributions
* Missing values
* Categorical variables
* Associations between variables
* Basic data-quality information

The main advantage was the speed of the initial overview.

---

## 🔎 D-Tale

D-Tale was used for interactive exploration of the Pandas DataFrame.

It provided a convenient way to:

* Inspect columns
* Explore distributions
* Filter and sort data
* Investigate suspicious values
* Interactively explore the dataset

This made it useful for moving from a general overview toward more detailed investigation.

---

## ⚡ Automated EDA ≠ Automated Analysis

One of the main takeaways from this project was:

> **Automated EDA is not the same as automated analysis.**

Tools such as Sweetviz and D-Tale can help identify patterns and potential issues quickly.

However, the analyst still needs to:

* Validate anomalies
* Understand the business context
* Decide how missing values should be handled
* Determine whether extreme values are actually problematic
* Investigate relationships between variables
* Ask meaningful analytical questions

Automation can accelerate exploration, but it does not replace analytical thinking.

---

## 🔄 Practical EDA Workflow

A useful workflow based on this exploration is:

```text
Dataset
   ↓
Automated Overview
   ↓
Sweetviz
   ↓
Interactive Exploration
   ↓
D-Tale
   ↓
Python Validation
   ↓
Business Context
   ↓
Meaningful Analysis
```

---

## 📁 Project Structure

```text
EDA-Sweetviz-DTale/
│
├── README.md
├── requirements.txt
│
├── notebooks/
│   └── EDA_Sweetviz_DTale.ipynb
│
├── data/
│   └── customer_churn.csv
│
├── reports/
│   └── Sweetviz_Report.html
│
├── presentation/
│   └── EDA_Sweetviz_DTale_LinkedIn_Carousel.pptx
│
└── screenshots/
    ├── sweetviz_overview.png
    └── dtale_exploration.png
```

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/EDA-Sweetviz-DTale.git
```

### 2. Move into the project directory

```bash
cd EDA-Sweetviz-DTale
```

### 3. Create a virtual environment

```bash
python -m venv venv
```

### 4. Activate the environment

**Windows:**

```bash
venv\Scripts\activate
```

**macOS/Linux:**

```bash
source venv/bin/activate
```

### 5. Install dependencies

```bash
pip install -r requirements.txt
```

### 6. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
notebooks/EDA_Sweetviz_DTale.ipynb
```

---

## 📌 Key Takeaway

This project reinforced an important idea:

> **Automation can accelerate exploration — but it doesn't replace the analyst.**

Sweetviz and D-Tale are useful for reducing repetitive work and getting a faster initial understanding of a dataset.

The real analytical value comes from what happens after those first observations: validation, interpretation, and asking the right questions.

---

## 👤 Author

**Abdul Basit**

Data Analyst | Data Engineering | BI | Python | SQL

---

## ⭐ If you found this project useful

Feel free to explore the repository, experiment with Sweetviz and D-Tale, and share your preferred approach to EDA.
