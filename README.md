# Healthcare Monitoring Analysis

## 📌 Problem Statement
Traditional health monitoring systems often categorize patient health status using rigid, predefined thresholds that may not capture nuanced variations across a diverse patient population.  
This can result in oversimplified assessments and overlook subtle but critical health patterns.  

The challenge is to develop a **dynamic and responsive approach using unsupervised learning** to identify natural groupings in health data, enabling **personalized and precise health management**.

---

## 🎯 Objectives
- **Identify Clusters**: Group patients into distinct clusters based on health metrics.  
- **Personalized Insights**: Understand unique health needs and risks for each group.  
- **Improve Monitoring**: Suggest targeted monitoring and interventions per cluster.  

---

## 📊 Dataset
- **File**: `healthmonitoring.csv`  
- **Records**: 500 individuals  
- **Features**:
  - Age  
  - Gender  
  - Heart Rate  
  - Blood Pressure  
  - Respiratory Rate  
  - Body Temperature  
  - Oxygen Saturation  
  - Sleep Quality  
  - Stress Level  
  - Activity Level  

All variables were collected over a specific monitoring period.  

---

## 🔄 Workflow
1. **Data Import & Exploration**  
   - Load dataset (`healthmonitoring.csv`).  
   - Check for null values and handle missing entries.  

2. **Data Cleaning**  
   - Fill missing values using median values.  
   - Ensure consistent data formatting.  

3. **Exploratory Data Analysis (EDA)**  
   - Summary statistics for all health metrics.  
   - Distribution plots for numerical features.  
   - Gender distribution visualization.  

4. **Activity, Sleep & Stress Analysis**  
   - Heart rate, oxygen saturation, respiratory rate, and body temperature analyzed across activity levels, sleep quality, and stress levels.  

5. **Patient Grouping**  
   - Patients categorized into simplified groups:  
     - **Age Group**: Young, Middle-aged, Senior  
     - **Blood Pressure Category**: Normal, Elevated, Hypertension Stage 1, Hypertension Stage 2  
     - **Heart Rate Category**: Low, Normal, High  
     - **Oxygen Saturation Category**: Normal, Low  

6. **Visualization & Insights**  
   - Boxplots and count plots visualize distributions and group characteristics.  

---

## 📊 Key Findings

### Gender Distribution
![Gender Distribution](images/gender_distribution.png)  
Nearly even split between male and female subjects, with males slightly higher at **51.2%**.  

### Correlation Matrix
![Correlation Matrix](images/correlation_matrix.png)  
No strong correlations among health metrics; all correlation values close to 0.  

### Heart Rate by Activity Level
![Heart Rate by Activity](images/hr_activity.png)  
- Increases from resting to walking.  
- Minimal increase from walking to running.  
- Outliers in resting heart rate indicate unusually high values for some individuals.  

### Blood Pressure Distribution
![Blood Pressure Distribution](images/bp_distribution.png)  
- **Systolic BP**: Wider spread, peaks around 120 mmHg and 140 mmHg.  
- **Diastolic BP**: Narrower, peak around 80 mmHg.  

### Health Metrics by Gender
![Heart Rate by Gender](images/hr_gender.png)  
![Oxygen Saturation by Gender](images/oxy_gender.png)  
- Heart rate and oxygen saturation **similar for males and females**.  
- Few outliers in oxygen saturation, but overall distribution unaffected.  

### Health Metrics by Sleep Quality & Stress Levels
![Heart Rate & Oxygen by Sleep/Stress](images/sleep_stress.png)  
- Heart rate remains fairly consistent; slight variation for poor sleep.  
- Oxygen saturation slightly decreases from excellent to poor sleep, with some outliers.  

### Respiratory Rate & Body Temperature by Activity Level
![Respiratory Rate & Body Temp](images/resp_temp_activity.png)  
- Respiratory rate increases with higher activity (walking → running).  
- Body temperature shows slight upward trend from resting to running.  
- Outliers indicate individual variations.  

---

## 🧩 Patient Grouping
Patients were grouped for simplified analysis instead of clustering:  

- **Age Group**: Young, Middle-aged, Senior  
- **Blood Pressure Category**: Normal, Elevated, Hypertension Stage 1, Hypertension Stage 2  
- **Heart Rate Category**: Low, Normal, High  
- **Oxygen Saturation Category**: Normal, Low  

---

## 🖼️ Grouped Data Visualization
### Distribution of Age Groups
![Age Group Distribution](images/age_group.png)  
Seniors largest, followed by Young, then Middle-aged.  

### Blood Pressure Categories
![Blood Pressure Categories](images/bp_category.png)  
Most normal, fewer elevated or hypertensive, very few stage 2.  

### Heart Rate Categories
![Heart Rate Categories](images/hr_category.png)  
Majority normal, few low or high.  

### Oxygen Saturation Categories
![Oxygen Saturation Categories](images/oxy_category.png)  
Almost all normal, few low.  

> **Note:** Replace the placeholder paths (`images/...`) with the actual filenames of your saved plots.  

---

## ✅ Conclusion
This analysis demonstrates how **unsupervised learning and grouped analysis** can enhance health monitoring:  

- Key health metrics were explored across **activity, sleep, stress, and gender**.  
- Patient groups were categorized to identify **at-risk populations**.  
- Visualizations provide **insightful overviews** for targeted monitoring and personalized interventions.  

By grouping patients and analyzing trends, this project supports **better-informed healthcare decisions** and **more precise, patient-centered monitoring strategies**.  
