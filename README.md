# SepsisProject

Sepsis is a life-threatening condition that affects 1.7 million people in the U.S. annually, leading to 270,000 deaths. It contributes to over one-third of hospital fatalities and accounts for $24 billion in healthcare costs annually.

Despite its severity, early detection remains a challenge due to sepsis' syndromic nature, often leading to delayed treatment and poor patient outcomes. This project aims to develop a data-driven approach to early sepsis detection.

**<h2>Objective</h2>**
Identify a patient's risk of sepsis and make a prediction of sepsis for every hourly time window in the patient’s clinical record.

**<h2>About Data</h2>**
The Sepsis project involved the analysis of a vast dataset comprising over 1.5 million data points from more than 40,000 ICU patients. This dataset included hourly records, demographic information, and the presence of a sepsis label indicating the hour of sepsis diagnosis. Additionally, the project included the bloodwork test results of 34 key biomarkers associated with sepsis.

**<h2>Demographic Analysis </h2>**
Utilized Calculated Fields, Level of Details Expressions(LOD) with the "FIXED" keyword to accurately classify patients into sepsis, non-sepsis, and onset sepsis
![Alt text](https://github.com/K-Manjula/SepsisProject/blob/master/S_Cat.png)

<img src="https://github.com/K-Manjula/SepsisProject/blob/Develop/Demo.png" width="700" height=500 alt="Description of image" />

* Dashboard displays patient distribution: 98.02% without sepsis and 1.98% with sepsis.
* The primary goal is swift diagnosis and treatment for the non-sepsis patients (98.02%) to prevent sepsis development.
* These patients were primarily admitted due to infections or SIRS.
* Demographic analysis factors in age and gender, revealing a heightened sepsis risk in the 60-80 age group, with males at higher risk than females.

**<h2>Patient Distribution</h2>**
* Total patients: 40,336
* Sepsis incidence: 1% (426 patients)
* Onset Sepsis: 6% (2,506 Patients)
* Non-sepsis patients: 93% (37,404 patients)

**<h2>ICU Admissions</h2>**
* MICU sepsis admissions: 1% (189 patients)
* SICU sepsis admissions: 2.% (87 out of 2,932 patients)
* Non-sepsis MICU admissions: 11,301 patients
* Non-sepsis SICU admissions: 11,802 patients
  
**<h2>Gender Distribution</h2>**
* Female patients: 44.05%
* Male patients: 55.95%
  
**<h2>Age and Gender Analysis</h2>**
* Male patients showed higher susceptibility to sepsis across age groupsPatients classified into ten age groups
* Demographic analysis factors in age and gender, revealing a heightened sepsis risk in the 60-80 age group, with males at higher risk than females.

**<h2>ICU Length of Stay (ICULOS)</h2>**
* Sepsis patients: Shorter ICU stays compared to non-sepsis patients
* Onset sepsis patients: Longest ICU stays
* Average ICU stay for sepsis patients: 8.85hours

**<h2>Patient Admission Patterns</h2>**
* Relationship established between patient volume and hospital admission time
* Gender-specific variations in admission times for sepsis patients
* MICU and SICU patient counts fluctuated during the first 24 hours of admission
* Highest count in the 1st hour
* Decreasing trend towards the 24th hour
  
This demographic analysis provides crucial insights into patient distribution, sepsis incidence, and ICU utilization patterns. These findings can inform strategies for optimizing patient care and resource allocation.

**<h2>SIRS (Systemic inflammatory response syndrome) Analysis</h2>**
Systemic inflammatory response syndrome(SIRS) is a serious condition that occurs when the body has an exaggerated defense response to a harmful stressor

![Alt text](https://github.com/K-Manjula/SepsisProject/blob/Develop/Bio.png)

* 22% of total patients in this data set got admitted with SIRS symptoms. It is hard to find the time of trigger since many patients may not keep track of the time when they start showing each symptom.
* Over 50% of patients have high heart rates and increased respiratory rates. Around 2% of patients are admitted with Acute-phase Reactions (high temp & high WBC), which can be fatal. Within the first hour of admission, many patients show more than 2 SIRS symptoms, requiring immediate medical attention.

<img src="https://github.com/K-Manjula/SepsisProject/blob/Develop/Email.png" width="500" height=500 alt="Description of image"/>    <img src="https://github.com/K-Manjula/SepsisProject/blob/Develop/SIRS.png?raw=true" width="400" height=400 alt="Description of image" />

* Utilized calculated fields, Level of Details Expressions(LOD) with the "FIXED" keyword to specifically target and identify the SIRS trigger hour for patients.
* Implemented dummy axes technique and formatted cell colors to effectively highlight abnormal test results, enabling quick identification and analysis.
* Added URL actions to implement email alerts, ensuring the prompt notification of responsible hospital staff when patients meet the pre-alert criteria, facilitating timely attention and response.
  
**<h3>Key Observations</h3>**
* Heart Rate: Patient ID 4 had a Heart Rate of 113 bpm at Trigger Hour 10.
* Respiratory Rate: Patient ID 9 recorded a Respiratory Rate of 30 bpm during the Trigger Hour.
* Temperature: Patient ID 18 had a Temperature of 38.56 degree C during the Trigger Hour
* WBC Count and PaCO2: Patient ID 8 had a WBC Count of 11.4 and PaCO2 of 25 mmHg during the Trigger Hour. This study emphasizes the importance of monitoring key biomarkers such as Temperature, Heart Rate, Respiratory Rate, PaCO2, and WBC Count for timely identification and management of SIRS.
  
**<h2>Conclusion</h2>**
This project demonstrates the significant impact of data analysis on patient care. By identifying crucial risk factors and sepsis-related patterns, we empower doctors to detect and treat this severe condition proactively, potentially saving lives and reducing hospital stays. This not only improves patient outcomes but also enhances ICU operational efficiency by up to 30%.








