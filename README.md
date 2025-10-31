# Cancer Risk Factors and Intensity Analysis

## Project Overview
This project explores how **lifestyle and environmental factors** contribute to cancer risk levels using data analysis in **Power Query, and Power BI**.
The aim is to identify high-risk groups and key factors (like smoking, alcohol use, obesity, diet, and air pollution) that impact cancer intensity and overall health risk.
The project demonstrates how analytical thinking, visualization, and data storytelling can support **preventive healthcare decisions**.

--------------
## Objectives
-	Analyze correlations between different risk factors and cancer intensity.
-	Classify patients into **High**, **Medium**, and **Low** risk categories.
-	Identify which habits (e.g., smoking, diet, physical inactivity) most increase overall risk.
-	Visualize patterns across **age**, **gender**, **BMI**.
-	Develop actionable insights for awareness prevention.
-------------
## Tools & Technologies
-	**Power Query Editor** -> Data Cleaning, basic analysis, Data transformation and column derivation.
-	**Power BI** -> Dashboard creation and visualization
-	**DAX** -> KPI calculations and measures
------
## Data Columns
‘Patient_ID’, ‘Cancer Type’, ‘Age’, ‘Gender’, ‘Smoking’, 'Alcohol Use’, ‘Obesity’, ‘Family History’,
‘Diet_Red_Meat’, ‘Diet_Salted_Processed’, ‘Physical_Activity’, ‘BMI’, ‘Air_Pollution’.
‘Occupational_Hazards’, ‘Overall_Risk_Score’, ‘Risk_Level’, ‘Physical_Activity_Level’
--------
## Visualization Created
-**KPI Cards:**
  - Total Patients
  - Average BMI
 - Average Age
-**Bar Charts:**
    - No. of Patients vs Risk Level
   - Cancer_Type vs Family_History
-**Pie Chart:**
    - Obesity vs Gender
- ** Donut Chart **
   - No. of Patients vs Cancer_Type
  - Smoking vs Age_Group
-**Line Chart**
  - Age_Distribution of Patients
 - Risk Vs Smoking
- Risk vs Obesity 
- Risk vs Salted_Processed
- Risk vs Age_Group
- Risk vs Occupational_Hazards
- Risk vs Air_Pollution
- Risk vs BMI
-** Area Chart**
- Risk vs Alcohol_Use
- Risk vs Physical_Activity
-Risk vs Red_Meat
-**Slicers**
- Gender
- Age_Group
- Risk Level
- Cancer Types
---
## Key Insights 
-	Total patients 2000, Avg BMI-26.18, and Avg. Age 63.25.
-	75% of patients fall under medium risk – a window for early intervention.
-	Smoking, Obesity, and alcohol are the top risk factors.
-	Processed foods & red meat elevate risk levels.
-	Among female patients, 44.52% suffer from breast cancer.
-	Among men patients, 31.19% suffer from prostate cancer.
-	Overweight (MBI above 31) & Underweight (BMI below 19) are at higher risk.
-	Risk levels tend to decrease with age, likely reflecting earlier lifestyle interventions older population.
-	Patients with a family history of cancer don’t show a higher prevalence.
-	Air pollution & occupational hazards are key environmental contributors to elevated cancer levels.
----
##DAX Measures Used 
-	Avg_Age = AVERAGE('cancer-risk-factors'[Age])
-	Avg_BMI = AVERAGE('cancer-risk-factors'[BMI])
-	Total_Patients = COUNT('cancer-risk-factors'[Patient_ID])


## Calculated Column
-	Age_Group = If [Age] < = 30 then “Young” else if [Age] < =50 then “Middle” else” Senior”
-	BMI_Category = If [BMI] < 18.5 then “Underweight” else if [BMI] < 24.9 then “Healthy weight” else if [BMI] < 29.9 then “Overweight” else “Obesity”
-	Lifestyle_Score = Avg. of (“smoking” + “Alcohol_Use” + “Obesity” + “Diet_Red_Meat” + “Diet_Salted_Processed” + “Physical_Activity_Level” )
-	Environmental_Score = Avg. of (“Air_Pollution” + “Occupational_Hazards”)


## Conclusion
 The analysis shows a clear relationship between lifestyle choices and cancer risk.
Behavioral factors such as smoking, poor diet, and inactivity directly raise the probability of higher risk levels. Encouraging healthier lifestyles can significantly reduce cancer incidence among at-risk populations.
“Data can’t cure cancer – but it can guide the fight against it”.

## Recommendations
-	Launch awareness campaigns targeting smoking cessation and dietary improvements.
-	Promote physical activity programs in workplaces and schools.
-	Most risk factors are preventable.
-	Awareness & early lifestyle changes can reduce intensity.
-	Data-driven insights can guide public health policy and early detection efforts.
## Skills Demonstrated
Data Cleaning, Power Query, Data Modeling, DAX Calculations, Power BI Dashboarding, Analytical Thinking, Data Visualization
## Dataset Source
The dataset was created for educational and analytical purposes.
Kaggle (https://www.kaggle.com/datasets/tarekmasryo/cancer-risk-factors-dataset)
## Connect With Me
I’m passionate about using data to improve healthcare insights and decision-making.
Let’s connect on LinkedIn- (https://www.linkedin.com/in/upasana-bara-225611247/)
## If you find this project interesting, please give it a star!

