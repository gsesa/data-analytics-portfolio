🔬 **Air Quality Hypothesis Testing – Null & Alternative Hypotheses, p-Values, and Decision Rules**  
This project was developed as part of the **Google Advanced Data Analytics Certificate** (Course 3). It simulates the role of a data analyst at the **United States Environmental Protection Agency (EPA)**, demonstrating how hypothesis-testing frameworks help determine whether differences in Air Quality Index (AQI) metrics are statistically significant or simply due to random sampling variation.

---

⚙️ **Objective**  
Formulate and test statistical hypotheses on AQI data (e.g., “Does California’s mean AQI differ from the national mean?”), calculate test statistics and p-values, and decide whether to reject the null hypothesis at a chosen significance level.

---

🔍 **Key Activities**  
- Loaded and cleaned **EPA AQI** data for carbon monoxide  
- Defined **null (H₀)** and **alternative (H₁)** hypotheses for comparing mean AQI values  
- Selected a **significance level (α = 0.05)** and drew random samples with replacement  
- Computed **test statistics** (one-sample *t*-test and two-sample *t*-test scenarios) with `scipy.stats`  
- Calculated **p-values** and applied decision rules to **reject or fail to reject H₀**  
- Visualized sampling distributions and critical regions to illustrate decision boundaries  
- Discussed potential **Type I / Type II errors** and the impact of sample size on statistical power  

---

💡 **Key Insights**  
- **Small p-values (< α)** provided evidence against H₀, indicating meaningful differences in AQI means for certain states  
- **Larger samples** increased statistical power, reducing the chance of missing real effects  
- Clear articulation of null and alternative hypotheses, combined with a predefined α, ensured objective decision-making  
- Hypothesis testing offered a rigorous framework for prioritizing environmental interventions where AQI deviations were significant  

---

📁 **Files Included**  
- 📓 *Jupyter Notebook* (`Activity_Explore hypothesis testing.ipynb`)  
- 📄 *Executive Summary* (PDF)  

---

🛠 **Tools Used**  
- Python  
- Jupyter Notebook  
- `pandas`, `numpy`, `scipy`, `matplotlib`, `seaborn`, `statsmodels`  

---

👤 **Developed by**  
Gabo Espinoza | Data Analyst & BI Specialist  

---

👉 **Click here to view the full project on GitHub**  
https://github.com/gsesa/data-analytics-portfolio
