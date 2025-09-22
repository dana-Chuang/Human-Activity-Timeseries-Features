# 🏃‍♀️ Human Activity Time‑Series Feature Engineering (AReM)

Feature engineering and statistical analysis for **human activity recognition** using the
[AReM dataset](https://archive.ics.uci.edu/ml/datasets/Activity+Recognition+system+based+on+Multisensor+data+fusion+%28AReM%29).
Each instance contains **6 time series** of length ~480; activities span 7 classes (e.g., walking, standing, bending).

This repo focuses on **time‑domain feature extraction**, **bootstrap confidence intervals**, and **feature selection** to prepare
a robust tabular dataset for downstream classifiers.

---

## ✨ What’s Inside
- **Time‑domain features** per time series: `min, max, mean, median, std, q1, q3`
- **Bootstrap (90%) CIs** for the **standard deviation** of each feature
- **Compact feature table**: one row per instance, 6×7 = **42 features** (+ optional normalized variants)
- **EDA visuals**: class‑colored scatterplots and boxplots
- **Feature selection**: choose the **top 3** features (e.g., min/mean/max) to carry forward
