### Predicting Emergency Department Surge: A Longitudinal Study of Age-Specific Respiratory Trends
**Course**: **Machine Learning for Bioinformatics (BIFX546)**

**Student:** Kardam Patel

**Instructor:** Prof. Sarangan Ravichandran

**Project Overview**:
This project focuses on the analysis of a longitudinal dataset of Emergency Department (ED) visits for respiratory conditions across the United States at the state level. The study tracks clinical encounters across six distinct age demographics from October 2023 to January 2026. The primary goal is to apply coding logic, data visualization, and applyied statistics and machine learning models to understand respiratory health trends and demographic vulnerabilities.

**Repository & Setup**:
The project is hosted on GitHub and is designed to run in a Jupyter environment or Google Colab.

**GitHub Repository**:
URL: https://github.com/kardam2806/Respiratory_conditions_ED_Notebook

**Original Data Source**: Center for Disease Control and Prevention

**Data Location:** The processed dataset is located in the Raw_Data/ directory at the following path:
Raw_Data/tidy_respiratory_conditions.csv

**How to Run the Notebook**:
To execute the analysis, follow these steps:

1. Direct GitHub Fetching:
The notebook is configured to automatically pull the necessary data directly from the GitHub repository using the following URL:
https://raw.githubusercontent.com/kardam2806/Respiratory_conditions_ED_Notebook/main/Raw_Data/tidy_respiratory_conditions.csv

2. Google Colab Setup:
If you are running the notebook in Google Colab and wish to save results to your personal drive, the script includes logic to mount Google Drive:

3. Ensure your project folder is named Respiratory_conditions_ED_Notebook in your Drive root.

The script will set the working directory to /content/drive/MyDrive/Respiratory_conditions_ED_Notebook.

**Required Libraries:**


Ensure you have the following Python packages installed:

Bash
pip install pandas openpyxl matplotlib seaborn scipy scikit-learn


**Execution:**
Run the cells in order to perform data wrangling (converting longitudinal data to a wider format via pivot_table), monthly resampling, and statistical testing.










### Learning Objectives:


**Demographic Vulnerability:** Determine if specific groups (e.g., infants) show consistent vulnerability across all respiratory conditions or if risk is isolated to specific pathogens.

**Seasonal Periodicity:** Map the seasonal patterns of diseases and identify "sentinel" groups (such as school-aged children) whose outbreaks may precede those in the general population.

**Emerging Threat Identification:** Identify specific conditions showing a statistically significant upward trajectory in patient volume.

**Resource Allocation:** Isolate the most prevalent conditions to assist in the better allocation of healthcare resources.




### Technical Methodology:

**Data Processing**:
**Source:** Data is retrieved from a tidy CSV format hosted on GitHub.

**Wrangling:** The dataset is converted from a longitudinal format to a wider format using pivot_table to handle multiple duplicate entries and facilitate easier observation.

**Time-Series Preparation:** Data is resampled to monthly averages (ME) to smooth out weekly fluctuations for trend analysis.


### Statistical & Machine Learning Analysis: Derived Insights

| Methodology | Objective | Key Findings & Insights |
| :--- | :--- | :--- |
| **Spearman Correlation & Linear Regression** | Trend Analysis | Established a statistically significant inverse relationship, showing **decreasing vulnerability as age increases**[cite: 1]. |
| **Pairwise Tukey's Test** | Group Comparison | Confirmed that the **infant group** has a significantly higher frequency of ED visits than any other age demographic[cite: 1]. |
| **K-means Cluster Analysis** | Demographic Profiling | Confirmed that condition prevalence is **isolated to specific groups**, with Acute URIs being the only cross-demographic exception[cite: 1]. |
| **Random Forest Feature Selection** | Variable Importance | Validated **'Age Group'** as a primary and powerful predictor for forecasting ED visit patterns[cite: 1]. |
| **Negative Binomial Distribution** | Seasonal Modeling | Successfully modeled **clumped seasonal spikes**, providing a robust statistical foundation for hospital capacity planning[cite: 1]. |


### 📊 Concluding Observations:

| Methodology | Key Findings | Strategic Insight |
| :--- | :--- | :--- |
| **One-Way ANOVA** | Age is a statistically significant driver of ED visits. | Validates demographic-based triage protocols. |
| **Two-Way ANOVA** | Age and Condition both act as significant factors leading to ED visits. | Accounts for interaction effects between age and health status. |
| **Spearman & Regression** | Evidence shows vulnerability decreases as age increases. | Focus preventative care and outreach on younger demographics. |
| **Pairwise Tukey’s Test** | Infants had the highest frequency of ED visits compared to all other groups. | Prioritize pediatric resource allocation and infant-specific capacity. |
| **K-Means Clustering** | Condition prevalence is isolated by age (except for universal Acute URIs). | Tailor clinical services to age-specific clusters. |
| **Random Forest** | Age Group is a stronger predictor for ED visits than clinical condition. | Prioritize demographic targeting for resource allocation. |
| **Negative Binomial** | Captured clumped seasonal spikes typical of respiratory illnesses. | Reliable for capacity planning and surge management. |



### Key Findings & Inferences:

**Primary Vulnerability:** The infant group should be the primary focus when planning and allocating healthcare resources.

**Strategic Planning:** Age and condition factors are critical for addressing emergency staffing schedules and future expansion plans.

**Seasonal Outbreaks:** Advanced strategies should be developed for conditions like Bronchitis and Tonsillitis, which exhibit sudden seasonal outbreaks during specific months of the year.
