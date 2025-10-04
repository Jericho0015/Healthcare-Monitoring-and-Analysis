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
![Gender Distribution](https://github.com/Jericho0015/Healthcare-Monitoring-and-Analysis/blob/main/Visualizations%20Plots/Gender%20Distribution.PNG)  
Nearly even split between male and female subjects, with males slightly higher at **51.2%**.  

### Correlation Matrix
![Correlation Matrix](https://github.com/Jericho0015/Healthcare-Monitoring-and-Analysis/blob/main/Visualizations%20Plots/Correlation.PNG)  
No strong correlations among health metrics; all correlation values close to 0.  

### Heart Rate by Activity Level
![Heart Rate by Activity](https://github.com/Jericho0015/Healthcare-Monitoring-and-Analysis/blob/main/Visualizations%20Plots/Heart%20Rate%20by%20Activity%20Level.PNG)  
- Increases from resting to walking.  
- Minimal increase from walking to running.  
- Outliers in resting heart rate indicate unusually high values for some individuals.  

### Blood Pressure Distribution
![Blood Pressure Distribution](https://github.com/Jericho0015/Healthcare-Monitoring-and-Analysis/blob/main/Visualizations%20Plots/Blood%20Pressure%20Distribution.PNG)  
- **Systolic BP**: Wider spread, peaks around 120 mmHg and 140 mmHg.  
- **Diastolic BP**: Narrower, peak around 80 mmHg.  

### Health Metrics by Gender
![Heart Rate by Gender](https://github.com/Jericho0015/Healthcare-Monitoring-and-Analysis/blob/main/Visualizations%20Plots/Health%20metrics%20by%20Gender.PNG)   
- Heart rate and oxygen saturation **similar for males and females**.  
- Few outliers in oxygen saturation, but overall distribution unaffected.  

### Health Metrics by Sleep Quality & Stress Levels
![Heart Rate & Oxygen by Sleep/Stress](https://github.com/Jericho0015/Healthcare-Monitoring-and-Analysis/blob/main/Visualizations%20Plots/Analyze%20heart%20rate%20and%20oxygen%20saturation%20by%20sleep%20quality%20and%20stress%20levels.PNG)  
- Heart rate remains fairly consistent; slight variation for poor sleep.  
- Oxygen saturation slightly decreases from excellent to poor sleep, with some outliers.  

### Respiratory Rate & Body Temperature by Activity Level
![Respiratory Rate & Body Temp](https://github.com/Jericho0015/Healthcare-Monitoring-and-Analysis/blob/main/Visualizations%20Plots/respiratory%20rate%20and%20body%20temperature%20by%20activity%20levelsPNG.PNG)  
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

## ✅ Conclusion
This analysis demonstrates how **unsupervised learning and grouped analysis** can enhance health monitoring:  

- Key health metrics were explored across **activity, sleep, stress, and gender**.  
- Patient groups were categorized to identify **at-risk populations**.  
- Visualizations provide **insightful overviews** for targeted monitoring and personalized interventions.  

By grouping patients and analyzing trends, this project supports **better-informed healthcare decisions** and **more precise, patient-centered monitoring strategies**.  
