---
title: "Estimation vitesse treuil"
date: 2025-07-09 22:59:55
categories:
  - blog
  - announcements
tags:
  - jekyll
  - github-pages
  - minimal-mistakes
  - first-post
excerpt: "bla bla"
header:
  teaser: /assets/images/1-estime-vitesse-treuil/ # Optional - add image later
---
# Method and Results

This document explains the methodology and summarizes the key results that are presented on the project webpage. The main results are visualized in the figures `slopes_boxplot_with_summary.png` and `plot_Leman_23-09-2024_08/39/08.png`.

---

## Method

The objective of this project is to estimate the winch velocity ("vitesse treuil") using collected sensor data. The methodology involves the following steps:

1. **Data Collection:**  
   Sensor data was recorded during winch operations, capturing relevant signals (e.g., time, position, velocity).

2. **Preprocessing:**  
   Raw data was cleaned and synchronized. Outliers and erroneous points were removed, and timestamps were aligned for further analysis.

3. **Estimation of Slopes:**  
   For each operational segment, a linear regression was applied to compute the slope, which corresponds to the estimated winch velocity.

4. **Statistical Analysis:**  
   Summaries of the estimated slopes were generated to quantify central tendency (median) and variability (quartiles, outliers).

5. **Visualization:**  
   The processed results were visualized to facilitate interpretation and comparison.

---

## Results

### 1. Boxplot of Estimated Slopes

![slopes_boxplot_with_summary](/assets/images/1-estime-vitesse-treuil/slopes_boxplot_with_summary.png)

The figure above presents a boxplot summarizing the estimated slopes (velocity estimates) across different operational segments. The boxplot displays the median, interquartile range, and any outliers in the data. This visualization helps to quickly assess the distribution and variability of the winch velocity estimates.

**Key findings:**
- The median slope provides a robust estimate of the typical winch velocity.
- The spread of the data (IQR) indicates the variability in operation.
- Outliers may correspond to unusual events or measurement anomalies.

---

### 2. Time Series Plot: Leman, 23-09-2024 08/39/08

![plot_Leman_23-09-2024_08/39/08](plot_Leman_23-09-2024_08/39/08.png)

This time series plot shows the evolution of the measured and/or estimated parameters during the operation on **Leman**, at the date and time `23-09-2024 08:39:08`. The plot provides detailed insight into the behavior of the system during a specific measurement campaign.

**Key findings:**
- The temporal evolution highlights phases of steady and variable winch velocity.
- Any deviations or abrupt changes are visible, which can be linked to operational events or anomalies in data collection.

---

## Conclusion

The methodology described above enables robust estimation and visualization of winch velocity. The summary statistics and time series visualization provide valuable insights for understanding system behavior and identifying areas for improvement in data collection or operational procedures.