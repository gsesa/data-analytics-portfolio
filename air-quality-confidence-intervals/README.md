# 🌿 Air Quality Confidence Intervals – Estimating Mean AQI & Statistical Significance

This project was developed as part of **Course 3** of the *Google Advanced Data Analytics Certificate*.  
It simulates the role of a data analyst at the United States Environmental Protection Agency (EPA), focusing on how confidence intervals help quantify uncertainty when estimating average Air Quality Index (AQI) values across different states.

---

## 📌 Project Overview

The activity walks through constructing and interpreting confidence intervals for state-level AQI measurements. By comparing sample statistics with population parameters, you will:

- Explore AQI variability across multiple states.  
- Select representative samples and compute their means.  
- Build confidence intervals to understand the precision of those estimates.  
- Evaluate results in the context of environmental decision-making.

---

## 🧪 Development Process

### 1. Initial Setup
- Defined the objective: estimate mean AQI and express the estimate’s reliability.  
- Imported key libraries: `pandas`, `numpy`, `scipy.stats`, `matplotlib`, `seaborn`.

### 2. Data Loading & Exploration
- Loaded the EPA AQI dataset (`c4_epa_air_quality.csv`).  
- Inspected shape, descriptive statistics, and value counts for `state_name`.  
- Identified a subset of states of interest (California, Florida, Michigan, …) to compare air-quality profiles.

### 3. Visualization & Descriptive Analysis
- Plotted box-and-whisker charts to show AQI spread by state.  
- Created an in-line distribution plot to highlight differences among states’ AQI values.

### 4. Statistical Inference
- Isolated the state with the highest mean AQI (California in this run).  
- Calculated sample mean (`x̄`) and sample standard deviation (`s`).  
- Selected a 95 % confidence level and derived the margin of error (ME) using  

  \[
  \text{ME} = z_{\alpha/2} \times \frac{s}{\sqrt{n}}
  \]

- Constructed the confidence interval manually and verified results with `scipy.stats.norm.interval()`.

### 5. Results & Evaluation
- Re-computed the interval after modifying sample parameters to observe how width changes with *n* and *s*.  
- Interpreted findings: “We are 95 % confident the true mean AQI for California lies between *L* and *U*.”  
- Discussed implications for public-health monitoring and resource allocation.

---

## 📊 Key Insights

| Insight                              | Take-away                                                                                           |
|--------------------------------------|------------------------------------------------------------------------------------------------------|
| Sample vs. population means          | The sample mean deviated slightly from the full-dataset mean, illustrating typical sampling variability. |
| Interval width & sample size         | Increasing the sample size reduced the standard error and yielded a narrower interval, giving a more precise estimate. |
| Practical relevance                  | Confidence intervals provide actionable ranges that help environmental analysts decide where to prioritize intervention or additional monitoring. |

---

## 📁 Project Files

| File name                                            | Description                                                                                              |
|------------------------------------------------------|----------------------------------------------------------------------------------------------------------|
| `Activity_Explore confidence intervals.ipynb`        | Jupyter Notebook containing the complete workflow: data loading, exploration, visualizations, statistical calculations, and narrative commentary. |

---

## 🛠 Tools Used

- Google Colab / Jupyter Notebook  
- Python (`pandas`, `numpy`, `scipy`, `matplotlib`, `seaborn`)

---

This project showcases fundamental inferential-statistics techniques that data analysts apply to environmental datasets. By quantifying uncertainty through confidence intervals, analysts can communicate findings clearly, support evidence-based policy, and ensure reproducible decision-making grounded in statistical rigor.
