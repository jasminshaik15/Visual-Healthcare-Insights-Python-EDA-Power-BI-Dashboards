<p align="center">
  <img src="Images/Healthcare Project Guide Illustration.jpg" alt="Healthcare Data Insights Banner" width="700" height="400">
</p>

# Visual-Healthcare-Insights-Python-EDA-Power-BI-Dashboards

## 📚 Table of Contents

1. [Project Overview](#1-project-overview)  
2. [Project Description](#2-project-description)  
3. [Key Features](#3-key-features)  
4. [Tools & Technologies](#4-tools--technologies)  
5. [Project Folder Structure](#5-project-folder-structure)  
6. [Installation & Setup](#6-installation--setup)  
7. [How to Run](#7-how-to-run)  
8. [Detailed Overview of Health_Care_EDA in Python](#8-detailed-overview-of-health_care_eda-in-python)  
    - 8.1 [Description of the Dataset](#81-description-of-the-dataset)  
    - [8.2 Data Cleaning & Preparation](#82-data-cleaning--preparation)  
        - [8.2.1 Merging All Datasets](#821-merging-all-datasets)  
        - [8.2.2 Standardizing Data](#822-standardizing-data)  
        - [8.2.3 Data Integrity Validation](#823-data-integrity-validation)  
        - [8.2.4 Handling Missing Values](#824-handling-missing-values)  
        - [8.2.5 Handling Duplicates](#825-handling-duplicates)  
        - [8.2.6 Converting Datatypes](#826-converting-datatypes)  
        - [8.2.7 Creating Derived Columns](#827-creating-derived-columns)  
        - [8.2.8 Mapping Categorical Values](#828-mapping-categorical-values)  
9. [Exploratory Data Analysis (EDA)](#9-exploratory-data-analysis-eda)  
    - [9.1 Univariate Analysis](#91-univariate-analysis)  
    - [9.2 Bivariate Analysis](#92-bivariate-analysis)  
    - [9.3 Multivariate Analysis](#93-multivariate-analysis)  
    - [9.4 Distribution Analysis](#94-distribution-analysis)  
    - [9.5 Correlation Analysis](#95-correlation-analysis)  
10. [Detailed Overview of Power BI Dashboard](#10-detailed-overview-of-power-bi-dashboard)  
    - [10.1 Overview Dashboard](#101-overview-dashboard)  
    - [10.2 Medical Condition & Outcome Analysis](#102-medical-condition--outcome-analysis)  
    - [10.3 Billing & Insurance Analysis](#103-billing--insurance-analysis)  
    - [10.4 Doctor & Hospital Performance](#104-doctor--hospital-performance)  
    - [10.5 Time-Based Analysis](#105-time-based-analysis)


 

## 📌 Project Overview <a name="1-project-overview"></a>
&nbsp;&nbsp;&nbsp;&nbsp;This project focuses on analyzing healthcare data to uncover key insights into patient admissions, medical conditions, treatment outcomes, and hospital performance. By combining Python for data preparation and cleaning with Power BI for interactive dashboards, the project aims to support healthcare administrators in making data-driven operational and clinical decisions.


## 📌 Project Description <a name="2-project-description"></a>
&nbsp;&nbsp;&nbsp;&nbsp;The Healthcare Data Analysis and Visualization Project involves working with a multi-sheet Excel dataset containing patient details, hospital information, doctor records, and patient visit data. The project workflow starts with merging and cleaning the data using Python libraries such as Pandas and NumPy in a Jupyter Notebook environment. Key data cleaning steps included handling missing values, standardizing text data, mapping admission type codes, calculating patient length of stay, and identifying high billing cases.

After preparing a clean and integrated dataset, exploratory data analysis (EDA) was performed in Python to validate data distributions and detect anomalies. The prepared dataset was then visualized in Power BI, where a series of interactive dashboards were built to deliver actionable insights.

The dashboards created include:

🔍 **Overview Dashboard:**  Patient Admissions Summary: Visualizing patient admission counts, age distribution, gender splits, and admission trends.

🏥 **Medical Condition & Outcome Analysis:** Analyzing the frequency of medical conditions, treatment outcomes, and recovery rates.

💵 **Billing & Insurance Analysis:** Tracking billing amounts, insurance coverage patterns, and flagging high-cost cases.

🧑‍⚕ **Doctor & Hospital Performance:** Evaluating doctor-wise and hospital-wise patient outcomes, admissions, and billing performance.

📅 **Time-Based Analysis:** Examining trends over time including admissions, discharges, and length of stay patterns.

This project demonstrates how Python-based data engineering can seamlessly integrate with BI tools like Power BI to deliver healthcare insights that improve operational efficiency and patient care decisions.


## 📌 Key Features <a name="3-key-features"></a>

- 📑 Merges multiple Excel sheets into a single clean dataset.

- 🧹 Cleans and standardizes patient, doctor, and hospital details.

- ⚙ Handles missing values (numeric → median, categorical → mode).

- 📏 Calculates Length of Stay for each patient.

- 💸 Flags patients with High Billing Amounts.

- 🔢 Maps Admission Types to numeric codes for analysis.

- 📊 Performs EDA using Python (Pandas, Matplotlib, Seaborn).

- 📈 Builds Power BI dashboards for dynamic visual insights.

## 📌 Tools & Technologies <a name="-tools--technologies"></a>

- Python
  
  - Pandas
    
  - NumPy
    
  - Matplotlib
    
  - Seaborn
    
- Power BI
  
- Microsoft Excel
  
- Jupyter Notebook
  
- CSV & Excel Files (for data storage)

## 📌 Project Folder Structure <a name="-project-folder-structure"></a>

├── 📁 Data/ # Healthcare Excel dataset files

│ ├── healthcare_dataset.xlsx

│

├── 📁 Images/ # Project images for README or dashboards

│

├── 📁 Python/ # Python notebook, requirements, and scripts

│ ├── HEALTHCARE_EDA.ipynb

│ ├── requirements.txt

│

├── 📁 PowerBI/ # Power BI dashboard files

│ ├── HEALTHCARE_DASHBOARD.pbix

│

├── 📄 .gitignore # Git ignore rules

├── 📄 LICENSE # Project open source license

├── 📄 README.md # Project overview and documentation

## 📌 Installation & Setup (One Block for Python + Power BI) <a name="-installation--setup"></a>

#### 1️⃣ Clone the repository
git clone [https://github.com/jasminshaik15/Visual-Healthcare-Insights-Python-EDA-Power-BI-Dashboards.git](https://github.com/jasminshaik15/Visual-Healthcare-Insights-Python-EDA-Power-BI-Dashboards)

cd Visual-Healthcare-Insights-Python-EDA-Power-BI-Dashboards

#### 2️⃣ Install required Python packages
pip install -r Python/requirements.txt

#### 3️⃣ Launch the Jupyter Notebook
jupyter notebook Python/HEALTHCARE_EDA.ipynb

#### 4️⃣ Open the Power BI Dashboard manually:
#### Navigate to the 'PowerBI' folder and open 'HEALTHCARE_DASHBOARD.pbix' in Power BI Desktop

## 📌 How to Run (For both Python EDA + Power BI) <a name="-how-to-run"></a>

### Run Python EDA Notebook

#### 1️⃣ Install dependencies  
Make sure you have all the necessary dependencies by running the following command:

pip install -r Python/requirements.txt

#### 2️⃣ Launch the Jupyter Notebook
After installing the dependencies, open the Jupyter notebook with the following command:
jupyter notebook Python/HEALTHCARE_EDA.ipynb

#### 3️⃣ In your browser, open the notebook and run all cells sequentially
Once the notebook is open in your browser, execute all the cells to run the EDA analysis.


### 📊 Open Power BI Dashboard
#### 1️⃣ Install Power BI Desktop
If you haven't already, install Power BI Desktop. You can download it from here.

#### 2️⃣ Open the Power BI file
To view the dashboards, open the Power BI file located in the PowerBI directory:

&nbsp;&nbsp;&nbsp;&nbsp; PowerBI/HealthCare_Dashboard.pbix

#### 3️⃣ Explore all the interactive dashboards
Once the Power BI file is open, you can explore the following interactive dashboards:

 - 📊 Overview Dashboard

 - 🩺 Medical Condition & Outcome Analysis

 - 💸 Billing & Insurance Analysis

 - 🧑‍⚕ Doctor & Hospital Performance

#### 4️⃣ Refresh the dataset if needed

If you need to refresh the data, connect to the Excel file located under the /data/ directory.

## 📌 Detailed overview of Healthcre_EDA in python <a name="8-detailed-overview-of-health_care_eda-in-python"></a>
  













