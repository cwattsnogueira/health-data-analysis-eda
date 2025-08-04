# Health Data Analysis

## Overview
This project performs a full exploratory analysis of the NSMES1988 dataset, which includes demographic, socioeconomic, and healthcare-related attributes for 4,406 individuals. It was developed as part of the Incremental Capstone Session 1, focusing on uncovering insights around hospital visits, insurance coverage, income levels, and health conditions.

## Team
- Carllos Watts-Nogueira  
- Ranjan Baral  

Course: Artificial Intelligence & Machine Learning
University of San Diego / Fullstack Academy
Section: 2504-FTB-CT-AIM-PT
End Date: May/2025

## Dataset Summary
**File Name**: `NSMES1988.csv`  
**Source**: [Drive Folder](https://drive.google.com/drive/folders/1Bs-qDfJFSMKIpC_rFs2f-LmLougXonf-)  
**Columns**:
- Demographics: `age`, `gender`, `married`, `region`, `school`
- Health: `health`, `adl`, `chronic`, `hospital`, `emergency`
- Utilization: `visits`, `nvisits`, `ovisits`, `novisits`
- Economics: `income`, `insurance`, `medicaid`, `employed`
- Technical Note: `Unnamed: 0` renamed to `id`

## Data Summary & EDA (Task A)

** Steps Completed**:
- Renamed columns & cleaned data  
- Scaled `age × 10`, `income × 10,000`  
- Changed `age` dtype to `int16` for memory optimization  
- Saved output files: `NSMES1988_updated.csv`, `df2_updated.csv`

**Key Findings**:
- No missing data  
- Memory reduced from 654.1 KB → 628.3 KB  
- 3 income records show negative values (e.g. `-10125`)  
- Categorical columns analyzed using `value_counts()`  
- Age and income binned for group analysis

## Visual Insights & Task B

**Insurance vs Income**:
- Majority of participants are insured  
- High-income individuals more likely to hold private insurance  
- Medicaid associated with low-income groups

**Hospital Visits by Health Status**:
- Poor health correlated with higher physician visits  
- Excellent health linked to fewer visits across all categories

**Correlation Analysis**:
- Heatmaps reveal clear relationships between age/health and hospital visit frequency

**Other Insights**:
- More females than males in the dataset  
- Exploratory plots using jitter, scatter, and bar charts for distribution and relationships

## Hospital Data Report (Task C)

This section consolidates all analytical findings:

- Identified usage patterns across hospital visit types by health status  
- Found visual trends connecting insurance coverage, Medicaid reliance, and income brackets  
- Noted potential biases in gender distribution and health access  
- Recommended next steps for anomaly review and deeper cross-variable analysis  

## Technologies Used
- Python 3.10  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Google Colab / Jupyter Notebook

## Next Steps
- Investigate income anomalies  
- Build predictive models for insurance or chronic illness  
- Visualize age-income-health intersections using interactive dashboards (e.g., Plotly or Streamlit)


