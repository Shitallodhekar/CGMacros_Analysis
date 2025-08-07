🍽️ **Glucose & Microbiome Insights Dashboard**
📊 **Project Overview**
This comprehensive Power BI project explores how metabolic markers, glucose responses, microbiome composition, and macronutrient intake interact to influence overall health. Built for a datathon, it integrates continuous glucose monitoring (CGM),
biometric lab results, gut microbiome data, and lifestyle inputs to enable personalized health insights. The dashboard suite delivers both population-wide trends and subject-specific analysis to drive precision nutrition and metabolic optimization.

📚 **Dataset Description**
Collected: 10-day tracking per subject

Sample Size: 45 subjects (ages 18–69)

**Data Types**:

Continuous Glucose Monitoring (Libre & Dexcom)

Macronutrient intake and meal logs

Heart rate and step counts

Gut microbiome profiles (2000+ microbe features)

Clinical biomarkers: HbA1c, fasting glucose, cholesterol, triglycerides

**Demographics**: Age, gender, ethnicity

🛠 **Technologies Used**
Power BI – for building dashboards and interactive insights

Python (Pandas) – for data preprocessing and summarization

SQL – for querying and cleaning tabular data

DAX – for creating measures and interactive elements

Bookmark Navigation – to display per-subject reports

🧹**Key Data Cleaning & Engineering Steps**
Converted minute-level CGM and Fitbit data to hourly averages

Resolved missing photo paths by automating file-name extraction

Grouped 2000+ microbiome species into functional categories (Good / Bad / Neutral)

Built DAX parameters to dynamically compare glucose with macronutrients

Used Power BI advanced visuals (due to Python-Power BI integration limitations)

🧠 **Dashboards & Key Insights**
1. Biometrics Dashboard
Assesses HbA1c, BMI, fasting glucose, cholesterol, and triglycerides to classify subjects by metabolic risk.

35% of subjects are prediabetic, 31% diabetic

High obesity prevalence, especially in females

27% at cardiovascular risk based on triglyceride + HDL scores

Aging reduces "good" gut microbes while increasing harmful ones

38% show abnormal cholesterol levels needing intervention

2. Subject Health Report Dashboard
Offers a deep dive into each subject’s profile: glucose spikes, gut microbes, heart rate, and nutrient intake.

Gut imbalance (e.g., low butyrate, high pathogens) correlates with poor glucose control

Personalized spike analysis by meal type (e.g., dinner causes most spikes for some)

Detects volatile glucose patterns, hypoglycemia risk, and timing-based sensitivity

Suggests time-restricted eating and macro adjustment strategies

3. Microbial & Gut Health Dashboard
Analyzes the microbiome's impact on inflammation and glucose variability.

Low butyrate producers linked to high inflammation and cholesterol issues

Dysbiosis (imbalance of harmful vs. beneficial bacteria) seen in obese subjects

Subjects with endotoxin-producing microbes (LPS biosynthesis) show higher insulin resistance

Stratified subjects into metabolic risk zones based on HbA1c + gut markers

4. Meal & Macronutrient Impact Dashboard
Compares glucose behavior based on nutrient ratios and meal timing.

High-carb, low-fat meals cause largest glucose spikes

Higher fiber intake reduces spikes across subjects

Dinner is the most calorie-dense and variable in glucose response

No clear link between calories and glucose—meal composition matters more

5. Glucose Response Trends Dashboard
Visualizes hourly glucose patterns and risk clustering based on biomarkers.

Peak glucose observed between 12–8 PM

Activity levels inversely correlated with glucose trends

Most spikes occur after breakfast—likely due to fasting effect

Combined risk markers (high triglycerides, low HDL, high insulin/glucose) categorize subjects from prediabetic to cardiac arrest risk

🧩 **Challenges & Solutions**
Challenge	Solution
Missing photo paths in CGMacros	Scripted automated photo ID matching and inserted correct paths
Large CGM data (per-minute)	Aggregated to hourly data to retain trends but reduce volume
2000+ microbes per subject	Grouped by functionality and categorized as good, bad, or neutral
Subject-specific visualizations	Used Power BI bookmarks to navigate individual profiles
Repeated charts per macronutrient	Created dynamic parameters to toggle nutrients in a single visual
No Python-Power BI visual interaction	Used native Power BI visuals and advanced chart features

🧾 **Conclusion**
This project transformed raw, complex health data into personalized and actionable insights. From identifying glucose triggers to profiling microbial imbalances, the dashboards provide a multi-dimensional view of metabolic health. 
Our focus wasn’t just on creating visuals—but telling the story within the data and guiding practical interventions.

Each minute of input became an hour of clarity—analyzing not just what participants ate or did, but how their bodies responded.

