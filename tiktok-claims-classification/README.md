# TikTok Claims Classification

This project was developed as part of **Course 2 of the Google Advanced Data Analytics Certificate**. It simulates a real-world business case in which a data analyst supports the development of a machine learning model to classify TikTok videos as **claims** or **opinions**.

---

## 📌 Project Overview

The goal of the activity is to explore a dataset of TikTok videos, understand the relationship between variables, and prepare the data for a classification model. The dataset includes user engagement metrics (views, likes, shares, comments) and metadata such as claim status and author moderation status.

**Main questions explored:**
- What percentage of videos are labeled as claims vs. opinions?
- How does engagement differ between claims and opinions?
- Are banned or under-review authors associated with higher engagement?

---

## 🧪 Development Process

1. **Initial Planning**  
   - Used the PACE framework to define the approach  
   - Identified key variables for analysis (`claim_status`, `author_ban_status`, engagement metrics)

2. **Data Inspection & Cleaning**  
   - Loaded and reviewed 19,382 records  
   - Checked for missing values and data types  
   - Created new features:
     - `likes_per_view`
     - `shares_per_view`
     - `comments_per_view`

3. **Exploratory Analysis**  
   - Compared engagement levels across `claim_status` and `author_ban_status`  
   - Calculated summary statistics (mean, median)  
   - Identified anomalies and potential outliers  

---

## 📊 Key Insights

- The dataset is well balanced:  
  - **9,670 claims**  
  - **9,512 opinions**
  
- **Claim videos consistently received higher engagement** (views, likes, and shares) than opinion videos.

- **Banned and under-review authors** had the highest median share counts:
  - Banned: 14,468  
  - Under review: 9,444  
  - Active: 437

These trends suggest that more viral content may often come from accounts that are eventually moderated or banned.

---

## 📁 Project Files

- `Activity-Template_-Course-2-PACE-strategy-document.pdf`  
  → Project planning document (PACE structure)

- `TikTok Project Lab - 1.ipynb`  
  → Jupyter Notebook with all data inspection, cleaning, and analysis

- `TikTok-Course-2-executive-summary.pdf`  
  → Final summary with findings, visuals, and recommendations

---

## 🛠 Tools Used

- Python  
- pandas  
- Jupyter Notebook  

---

This project demonstrates the full data analysis cycle: planning, exploration, insight generation, and communication. It reflects core responsibilities of a data analyst in a real business environment.
