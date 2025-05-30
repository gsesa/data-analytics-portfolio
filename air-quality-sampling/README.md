🌿 Air Quality Sampling – Central Limit Theorem & Standard Error
This project was developed as part of Course 3 of the Google Advanced Data Analytics Certificate. It simulates the role of a data analyst at the United States Environmental Protection Agency (EPA), focusing on understanding the sampling process and the implications of the Central Limit Theorem (CLT) in air quality analysis.

📌 Project Overview
The activity centers on simulating random samples from air quality data to explore variability in AQI values and the behavior of sample means. The main goals are to demonstrate the effects of sampling with replacement, calculate standard errors, and understand the sampling distribution of the mean.

🧪 Development Process
Initial Setup
Defined the objective: Understand how sample statistics vary and how they relate to population parameters.

Imported key libraries: pandas, numpy, matplotlib.

Data Exploration & Sampling
Loaded EPA dataset containing Air Quality Index (AQI) metrics.

Focused on the aqi column to study air quality variability.

Generated a sample of 50 observations using random sampling with replacement.

Ensured reproducibility by setting a random_state.

Statistical Analysis
Calculated the sample mean and sample standard deviation.

Computed the standard error of the mean (SEM) to quantify sampling variability.

Discussed how the Central Limit Theorem supports the use of the sample mean as an estimator.

📊 Key Insights
The sample mean differs slightly from the population mean, demonstrating natural variability in random samples.

The standard error provides a numeric measure of that variability and decreases with larger sample sizes.

Using a fixed random_state ensures that sampling is reproducible, a best practice in data analysis.

This exercise highlights the importance of statistical concepts in interpreting environmental data.

📁 Project Files
Activity_Explore sampling.ipynb
→ Jupyter Notebook with the full sampling procedure, code, and interpretation

🛠 Tools Used
Google Colab / Jupyter Notebook

Python

pandas

numpy

matplotlib

This project demonstrates essential statistical techniques used by data analysts when working with environmental datasets. It reflects core responsibilities in public health and policy-driven contexts: understanding variability, building reproducible analysis, and interpreting the significance of sample-based statistics.

