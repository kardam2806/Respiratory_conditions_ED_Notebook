**Respiratory Conditions Analysis (2023-2026)
Machine Learning for Bioinformatics (BIFX546)**

**Student:** Kardam Patel

**Instructor:** Prof. Sarangan Ravichandran

**Project Overview**:
This project focuses on the analysis of a longitudinal dataset of Emergency Department (ED) visits for respiratory conditions across the United States at the state level. The study tracks clinical encounters across six distinct age demographics from October 2023 to January 2026. The primary goal is to apply coding logic, data visualization, and statistical testing to understand respiratory health trends and demographic vulnerabilities.

**Repository & Setup**:
The project is hosted on GitHub and is designed to run in a Jupyter environment or Google Colab.

**GitHub Repository**:
URL: https://github.com/kardam2806/Respiratory_conditions_ED_Notebook

**Original Data Source**: CDC website
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










**Learning Objectives**:


**Demographic Vulnerability:** Determine if specific groups (e.g., infants) show consistent vulnerability across all respiratory conditions or if risk is isolated to specific pathogens.

**Seasonal Periodicity:** Map the seasonal patterns of diseases and identify "sentinel" groups (such as school-aged children) whose outbreaks may precede those in the general population.

**Emerging Threat Identification:** Identify specific conditions showing a statistically significant upward trajectory in patient volume.

**Resource Allocation:** Isolate the most prevalent conditions to assist in the better allocation of healthcare resources.




**Technical Methodology:**

**Data Processing**:
**Source:** Data is retrieved from a tidy CSV format hosted on GitHub.

**Wrangling:** The dataset is converted from a longitudinal format to a wider format using pivot_table to handle multiple duplicate entries and facilitate easier observation.

**Time-Series Preparation:** Data is resampled to monthly averages (ME) to smooth out weekly fluctuations for trend analysis.

**Statistical & Machine Learning Analysis**:
The following methods were employed to derive insights from the data:

1. Spearman Correlation & Linear Regression: Used to provide evidence for decreasing vulnerability as age increases.

2. Pairwise Tukey's Test: Conducted to compare ED visit rates between age groups, revealing that the infant group has the highest frequency of visits.

3. K-means Cluster Analysis: Confirmed that most condition prevalence is isolated to specific groups rather than being consistent across all age demographics (with the exception of Acute URIs).

4. Random Forest Feature Selection: Identified 'age group' as a strong predictor for ED visits.

5. Negative Binomial Distribution: Utilized to capture clumped seasonal spikes, aiding in capacity planning.

**Key Findings & Inferences**:

**Primary Vulnerability:** The infant group should be the primary focus when planning and allocating healthcare resources.

**Strategic Planning:** Age and condition factors are critical for addressing emergency staffing schedules and future expansion plans.

**Seasonal Outbreaks:** Advanced strategies should be developed for conditions like Bronchitis and Tonsillitis, which exhibit sudden seasonal outbreaks during specific months of the year.

Repository Structure
Tidy_resp (6).ipynb: Main Jupyter notebook containing the analysis, visualizations, and statistical tests.

Raw_Data/: Directory containing the raw and tidy datasets used in the study.
