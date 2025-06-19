# Data Science in Cyber Pipeline

A step-by-step Jupyter-based pipeline for detecting anomalies in network traffic.

---

## Pipeline Overview

This pipeline loads raw network traffic data, explores and preprocesses it, detects anomalies, clusters & segments connections, builds detection models.
- all resuslts summarized in a PDF report.

---

## Dataset

We use the **NSL-KDD** dataset:  
– Download link: https://www.kaggle.com/datasets/hassan06/nslkdd   


Key fields include:
- `duration` (connection length in seconds)
- `service` (destination service, e.g. http, smtp)
- `src_bytes` / `dst_bytes` (bytes sent/received)
- `label` (normal vs. specific attack types)

---

## Usage

1. **Clone**  
   ```bash
   git clone https://github.com/Basel6/Cyber-Data-Pipeline.git
   cd Cyber-Data-Pipeline
   ```
2. **Install dependencies**
  ```bash
   pip install -r requirements.txt
  ```
3. **Run the notebook**
  ```bash
   jupyter notebook Pipeline.ipynb
  ```
4.  **View the report**

    After running, open `reports/Report.pdf` for a concise summary of every step.

    ---
## Quick 12-Step Pipeline Checklist

1. **Dataset Selection**  
   We selected the **NSL-KDD** dataset for network-traffic anomaly detection.  
   Download link: https://www.kaggle.com/datasets/hassan06/nslkdd

2. **File System**  
   We documented all filenames, formats, sizes and version control details.

3. **Metadata Inspection**  
   We inspected data types, missing-value markers and schema definitions.

4. **Descriptive Statistics**  
   We computed means, standard deviations, minima/maxima and analyzed distributions, correlations, and duplicates.

5. **Abnormality Detection**  
   - **Univariate**: flagged extreme values in key features using z-scores and percentiles  
   - **Multivariate**: applied Local Outlier Factor to capture complex anomalies

6. **Clustering**  
   We ran k-means clustering, evaluated cluster assignments, and flagged low-confidence or unassigned points.

7. **Segmentation & Profiling**  
   We characterized each cluster, explored temporal patterns, and integrated domain insights.

8. **Text Analysis**  
   We performed NLP (sentiment/topic modeling, tokenization, style analysis) on any textual fields.

9. **Graphs & Visualization**  
   We created meaningful charts—distribution plots, network/flow graphs, feature importance visualizations.

10. **Modeling**  
    We trained classifiers (Decision Tree, Random Forest, XGBoost) to detect or predict anomalies.

11. **Reporting**  
    We summarized methods, results, and key takeaways in a concise PDF report with figures and tables.

12. **Improvement**  
    We proposed next steps—model tuning, feature selection, pipeline optimization, and scalability enhancements.

---
## Progress Update

### Completed: Steps 1–6  

All results, visualizations and discussion for these steps are in **reports/Report.pdf**.


### To Be Done: Steps 7–12

---

### **Author:**

Basel Shaer

### **Supervised by:**

Prof. Uri Itai
    
   
