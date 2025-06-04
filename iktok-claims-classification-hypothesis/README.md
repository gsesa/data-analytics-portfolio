# TikTok Verified-Status Analysis  

This project was developed for **Course 4 of the Google Advanced Data Analytics Certificate**.  
It recreates a real-world scenario in which a data-analytics team supports a machine-learning pipeline by first testing whether a creator’s verification badge affects the number of views their TikTok videos receive.

---

## 📌 Project Overview
We explored a dataset of **19 382 TikTok videos** that includes engagement metrics (views, likes, shares, comments) and creator attributes such as `verified_status`.

**Main steps**

1. **Descriptive comparison** – calculate the mean `video_view_count` for verified vs. unverified creators.  
2. **Two-sample Welch *t*-test** – confirm whether the observed gap is statistically significant.

These findings will feed the feature-engineering phase of a future claim-classification model.

---

## 🧪 Development Process

| Stage | Key actions |
|-------|-------------|
| **Planning** | Applied the **PACE** framework; defined the research question and success criteria. |
| **Data inspection & cleaning** | Loaded all records, enforced numeric types, and dropped missing `video_view_count` values. |
| **Exploratory analysis** | *Group means*<br>• **Unverified ≈ 265 663** views<br>• **Verified ≈ 91 439** views<br>Visualized distributions to check skew and outliers. |
| **Hypothesis testing** | Welch *t*-test → **t = 25.50**, **p ≈ 2.6 × 10⁻¹²⁰**. The gap is not due to chance. |
| **Next step** | Build a **logistic regression** using `verified_status` and additional features to predict claim status, accounting for skewed data and class imbalance. |

---

## 📊 Key Insights

* **Unverified creators attract nearly 3× more views** than verified creators on average.  
* The difference is **statistically decisive** (p ≈ 2.6 × 10⁻¹²⁰).  
* Possible drivers: click-bait tactics, trend chasing, or bot amplification among unverified accounts.  
* Understanding these behaviors is critical before using view counts or verification as model features.

---

## 📁 Project Files

| File | Description |
|------|-------------|
| `Activity_Course 4 TikTok project lab.ipynb` | Jupyter Notebook with data cleaning, EDA, and hypothesis testing. |
| `Course 4 PACE-strategy-document.pdf` | Planning document outlining Purpose, Audience, Context, and Execution. |
| `TikTok Course 4 executive-summary.pdf` | One-page report with visuals and business recommendations. |

---

## 🛠 Tools Used

* **Python** (`pandas`, `NumPy`, `SciPy`)  
* **Jupyter Notebook**  
* **Matplotlib** / **Seaborn** for quick plotting

---

This README captures the full data-analysis cycle—planning, exploration, statistical validation, and forward-looking recommendations—mirroring the responsibilities of a data analyst in a live business environment.
