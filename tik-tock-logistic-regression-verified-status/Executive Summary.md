# TikTok Verified-Status Logistic Regression

## Objective
Build a logistic regression model to predict whether a TikTok user is verified, so we can leverage verification behavior when classifying videos as claims vs. opinions.

---

## Model Results

**Dataset:**  
19,382 videos (1,200 verified → upsampled to 17,884; 17,884 not verified)

**Features:**  
- Video view count  
- Transcription length  
- Video duration (sec)

**Performance:**  
- **Accuracy:** 65%  
- **Precision (verified):** 75%  
- **Recall (verified):** 45%  
- **Precision (not verified):** 61%  
- **Recall (not verified):** 85%  
- **F1-score (macro):** 0.64

---

## Key Insights
- **Audience reach** (view count) is the dominant predictor of verification (highest log-odds).  
- **Transcription length** adds modest predictive signal—verified users tend to post slightly longer captions.  
- **Video duration** shows near-zero effect on verification.  
- **Engagement metrics** (likes, shares, comments) were highly correlated, so we used a single representative metric to avoid multicollinearity.  
- **Class balancing** via upsampling was critical to improve recall on the verified minority.

---

## Next Steps
1. Integrate these insights into the final claims-vs-opinions model.  
2. Explore additional features (e.g. `likes_per_view`, `share_rate`) and regularization tuning via cross-validation.  
3. Evaluate alternate sampling methods (SMOTE, downsampling) to further boost recall on verified users.  
