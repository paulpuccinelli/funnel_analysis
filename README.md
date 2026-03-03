# E-Commerce Funnel Analytics & Conversion Behavior Analysis

## Project Overview
This project performs an end-to-end analysis of user behavior in an e-commerce conversion funnel. Using event-level datasets, the analysis reconstructs the customer journey from the initial site visit to final purchase. The objective is to quantify user drop-off at each stage of the funnel and identify behavioral patterns that influence conversion.

The project demonstrates practical applications of **data manipulation, exploratory data analysis, feature engineering, and behavioral analytics** using Python.

---

## Problem Statement
Online businesses rely heavily on conversion funnels to understand customer behavior and optimize revenue. A significant proportion of users typically exit the funnel before completing a purchase. Identifying **where and when users abandon the funnel** is critical for improving product design, marketing strategies, and user experience.

This project answers several key questions:

- What proportion of visitors never add items to their cart?
- How many users abandon the funnel before checkout?
- What percentage of checkout sessions result in completed purchases?
- How long does it take for a typical user to convert?
- Are there temporal patterns (hour or month) associated with higher purchase activity?

---

## Dataset
The analysis uses four event datasets representing sequential stages of an e-commerce funnel.

| Dataset | Description |
|--------|-------------|
| `visits.csv` | Records of users visiting the website |
| `cart.csv` | Events where users add items to their cart |
| `checkout.csv` | Events where users initiate the checkout process |
| `purchase.csv` | Completed purchase transactions |

Each dataset contains **user identifiers and timestamps**, allowing the reconstruction of the full customer journey.

---

## Analytical Workflow

### 1. Funnel Reconstruction
The funnel is reconstructed by merging event tables using **left joins** to preserve the complete set of visitors and track progression through subsequent stages.

$$\text{Visit}\rightarrow\text{Cart}\rightarrow\text{Checkout}\rightarrow\text{Purchase}$$

This structure allows for direct measurement of **conversion and abandonment rates** at each stage.

---

### 2. Early Funnel Engagement
Visitors who never add an item to their cart are identified to measure **initial engagement failure**.

Metric computed:
- Proportion of visitors with **no cart interaction**

This highlights how effectively the site converts passive visitors into active shoppers.

---

### 3. Cart Abandonment Analysis
Users who add items to their cart but never initiate checkout are identified.

Metric computed:
- **Cart → Checkout conversion rate**

Cart abandonment is a critical metric for e-commerce optimization.

---

### 4. Checkout Abandonment Analysis
Users who begin checkout but fail to complete a purchase are analyzed.

Metric computed:
- **Checkout → Purchase conversion rate**

This stage typically reflects friction in the payment or account creation process.

---

### 5. Time-to-Conversion Analysis
For completed purchases, the time elapsed between the initial visit and purchase event is calculated.

Metric computed:
- **Average time to purchase**

This provides insight into typical buyer decision cycles.

---

### 6. Temporal Purchase Patterns
Purchasing behavior is analyzed across time.

Exploratory analyses include:

- **Hourly purchase distribution**
- **Monthly purchase trends**

These insights help identify periods of peak user engagement.

---

## Technologies Used

| Tool | Purpose |
|-----|--------|
| **Python** | Core programming language |
| **pandas** | Data cleaning, merging, and transformation |
| **NumPy** | Numerical operations |
| **Matplotlib** | Data visualization |
| **Jupyter Notebook** | Interactive analysis environment |

---

## Key Data Science Skills Demonstrated

- Data wrangling and dataset merging
- Behavioral funnel analysis
- Conversion rate computation
- Feature engineering using timestamps
- Exploratory data analysis
- Visualization of behavioral metrics
- Structured analytical workflow

---


---

## Potential Extensions
Future improvements could include:

- Building a **predictive model for purchase likelihood**
- Performing **cohort analysis** on user groups
- Implementing **funnel visualization dashboards**
- Applying **A/B testing frameworks** to evaluate conversion improvements
- Conducting **statistical hypothesis tests** on conversion rates

---

## Author
This project was created to demonstrate practical skills in **data analysis, statistical reasoning, and behavioral analytics using Python**.



