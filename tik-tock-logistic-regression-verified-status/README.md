# TikTok Verified Status Classification

This project was developed as part of the Google Advanced Data Analytics Certificate. It simulates a real-world case in which a data analyst builds and evaluates a logistic regression model to predict whether a TikTok user is verified, supporting downstream improvements to a claims vs. opinions classifier.

---

📌 **Project Overview**  
The goal is to predict a user’s verified status (verified vs. not verified) based on video metadata, engagement metrics, and transcript length. Accurate prediction helps the claims-classification pipeline prioritize content from high-reach creators.

**Main questions explored:**  
- What is the class balance between verified and unverified users?  
- Which features (views, likes, shares, downloads, comments, duration, transcription length) most strongly distinguish verified accounts?  
- How severe is multicollinearity among engagement metrics?

---

🧪 **Development Process**

**Initial Planning**  
- Applied the PACE framework to define objectives and success metrics  
- Selected target (`verified_status`) and candidate features  

**Data Inspection & Cleaning**  
- Loaded ~19 000 records from `tiktok_dataset.csv`  
- Checked missing values (~1.5 % in engagement and transcription fields)  
- Handled class imbalance by upsampling the verified class (from 1 200 to 17 884 samples)  

**Feature Engineering**  
- Created `transcription_length` (character count of video transcription)  
- Considered but dropped highly collinear features, retaining only one engagement metric  

**Exploratory Analysis**  
- Visualized distributions of engagement by verification  
- Compared transcription lengths for verified vs. unverified  
- Generated a correlation heatmap to identify multicollinearity  

---

📊 **Key Insights**  
- **Class balance:** Upsampling yielded 17 884 verified vs. 17 884 not verified.  
- **Top predictor:** Video view count drove the strongest log-odds.  
- **Multicollinearity:** Engagement metrics are tightly correlated; avoid feeding all at once.  
- **Duration vs. transcription:** Video length adds almost no signal, while transcript length provides modest separation.

---

📁 **Project Files**  
- **Activity_Course 5 TikTok project lab.ipynb** → Jupyter notebook with complete code and analysis  
- **TikTok-Course-2-executive-summary.pdf** → Final executive summary and recommendations  

---

🛠 **Tools & Libraries**  
Python · pandas · seaborn · matplotlib · scikit-learn · Jupyter Notebook  

This project demonstrates the end-to-end analytics cycle: planning, data preparation, feature engineering, exploratory analysis, model construction, and interpretation.  
