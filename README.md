# 📊 Funnel Analysis – Product Conversion Funnel

## 📌 Project Overview

This project analyzes a user conversion funnel for a signup and checkout process. The objective is to understand how users progress through each stage of the funnel, calculate stage-to-stage conversion rates, identify where the largest user drop-off occurs, and provide actionable business recommendations.

This type of analysis is commonly performed by Product, Growth, and Data Analytics teams to identify friction points and improve user conversion.

---

## 🎯 Business Problem

Users follow a fixed sequence of events:

**Visited Site → Signup Started → Details Filled → Email Verified → Purchase Completed**

Not every user completes the entire journey. The goal is to determine:

* How many unique users reached each stage.
* The conversion rate from one stage to the next.
* The stage with the highest user drop-off.
* Recommendations to improve the conversion funnel.

---

## 📂 Dataset

The dataset contains event-level records with the following columns:

| Column      | Description                           |
| ----------- | ------------------------------------- |
| `user_id`   | Unique identifier for each user       |
| `step`      | Funnel stage reached by the user      |
| `timestamp` | Date and time when the event occurred |

### Funnel Stages

1. Visited Site
2. Signup Started
3. Details Filled
4. Email Verified
5. Purchase Completed

---

## 🛠️ Tools & Libraries

* Python
* Pandas
* Matplotlib
* Jupyter Notebook

---

## 📋 Project Workflow

### 1. Data Loading

* Imported the CSV dataset using Pandas.
* Converted timestamps to datetime format.

### 2. Data Cleaning

* Removed duplicate events for the same user and stage.
* Maintained the correct funnel stage order.

### 3. Funnel Analysis

* Counted unique users at each funnel stage.
* Calculated stage-to-stage conversion rates.
* Calculated user drop-offs between consecutive stages.

### 4. Visualization

* Created a funnel/bar chart to visualize user progression through the funnel.

### 5. Business Insight

* Automatically identified the stage with the highest user drop-off.
* Suggested a product improvement based on the findings.

---

## 📈 Analysis Results

### Unique Users by Stage

| Stage              | Users |
| ------------------ | ----: |
| Visited Site       |   200 |
| Signup Started     |   150 |
| Details Filled     |    96 |
| Email Verified     |    52 |
| Purchase Completed |    44 |

### Conversion Rate (%)

| Stage              | Conversion Rate |
| ------------------ | --------------: |
| Visited Site       |         100.00% |
| Signup Started     |          75.00% |
| Details Filled     |          64.00% |
| Email Verified     |          54.17% |
| Purchase Completed |          84.62% |

### Drop-off Analysis

| Stage              | Users Lost |
| ------------------ | ---------: |
| Signup Started     |         50 |
| **Details Filled** |     **54** |
| Email Verified     |         44 |
| Purchase Completed |          8 |

**Largest Drop-off:** **Signup Started → Details Filled (54 users lost)**

---

## 💡 Business Recommendation

The largest drop-off occurs between **Signup Started** and **Details Filled**, where 54 users abandon the process. This indicates that the registration form may be too lengthy, confusing, or require unnecessary information. Simplifying the signup form by reducing mandatory fields or enabling social sign-in (such as Google or Apple login) could improve the completion rate. Running an A/B test would help validate whether these changes increase user conversions.

---

## 📁 Project Structure

```text
Funnel-Analysis/
│
├── funnel_events.csv
│   
│── funnel_event_samples.csv
├
│── funnel_summary.csv 
│   
│── Funnel Visualization 
├
│── Funnel_Analysis.ipynb
│ 
└── README.md
```

---

## 🚀 How to Run

1. Clone the repository.

```bash
git clone https://github.com/your-username/Funnel-Analysis.git
```

2. Install the required libraries.

```bash
pip install pandas matplotlib
```

3. Open the Jupyter Notebook or run the Python script.

---

## 📌 Key Skills Demonstrated

* Data Cleaning
* Exploratory Data Analysis (EDA)
* Product Funnel Analysis
* User Conversion Analysis
* Drop-off Analysis
* Data Visualization
* Business Insight Generation
* Python (Pandas & Matplotlib)

---

