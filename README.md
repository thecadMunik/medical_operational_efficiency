# 🏥 MedioPharm Medical Center: Operational Efficiency & Patient Outcome Analysis

## 📌 Project Overview

Modern hospitals generate large volumes of operational and patient data every day, but without a centralized analytical view, it becomes difficult for management to turn that data into actionable decisions. This project was designed to analyze hospital operations and patient care patterns in order to identify inefficiencies, uncover patient-risk trends, and support better decision-making across departments.

The analysis focuses on key hospital challenges such as rising admission pressure, delayed doctor responsiveness, repeated patient readmissions, abnormal vital-sign activity, and differences in patient outcomes across departments. Rather than viewing these issues separately, I approached the project by connecting them into a broader operational story of how workload, responsiveness, patient condition, and care outcomes interact in a real hospital environment.

This repository focuses on the two main analytical dashboards:
- **Hospital Operations Overview**
- **Patient Care & Outcome Analysis**

> 📌 The write-up for the **Administrative Q&A** section is available in the **Administrative Q&A** folder here:  
> [Administrative Q&A README](https://github.com/thecadMunik/medical_operational_efficiency/blob/main/administrative%20Q%26A/README.md)

---

## 🎯 Problem Statement

Hospital inefficiencies and inconsistent patient outcomes can affect care quality, resource use, and overall performance. Understanding trends in admissions, patient risk, doctor responsiveness, readmissions, and outcomes helps management intervene early and improve hospital decision-making.

---

## 🎯 Project Objectives

This project was carried out to:
- monitor hospital admissions and operational workload across departments
- evaluate doctor activity and responsiveness
- assess patient care outcomes across the hospital
- identify abnormal vital-sign patterns and potential patient risk
- compare departmental performance using outcome and activity measures
- support hospital leadership with data-driven insights for planning and intervention

---

## 🧰 Tools Used

- **Power BI Desktop**
- **Power Query**
- **DAX (Data Analysis Expressions)**

---

## 🗂️ Datasets Used

This project uses **4 connected datasets**:

1. **Admissions**
2. **Doctor Visits**
3. **Patients**
4. **Vitals**

---

## 🛠️ Approach

To complete the project, I followed a structured analytical process:

1. Loaded and reviewed the datasets to understand their structure and relationships  
2. Cleaned and transformed the data for consistency and usability  
3. Built the data model to connect hospital operations and patient care records  
4. Created supporting calculated columns and measures for time analysis, patient profiling, workload, and outcomes  
5. Designed two dashboards to separate operational performance from patient care analysis  
6. Generated insights and recommendations based on realistic hospital scenarios  

---

# 📊 Dashboard 1: Hospital Operations Overview

This dashboard focuses on the **operational side of hospital performance**. It highlights the scale of patient activity, department workload, doctor activity, response time, and overall hospital flow.

## What this dashboard contains
- operational KPI cards
- admissions trends over time
- admissions by department
- admissions vs discharges analysis
- doctor activity and responsiveness trends
- patient distribution views
- workload and flow indicators

## 🖼️ Dashboard Preview


# ❤️ Dashboard 2: Patient Care & Outcome Analysis

This dashboard focuses on the clinical and outcome side of hospital performance. It examines how patients are progressing through care, where recovery is strongest, where higher-risk outcomes are more visible, and how patient condition patterns may relate to overall care quality.

What this dashboard contains
patient outcome KPI cards
outcome distribution across the hospital
departmental outcome comparison
patient risk and abnormal vital analysis
demographic outcome patterns
chronic condition trends
length-of-stay and care quality indicators
🖼️ Dashboard Preview

Add Dashboard 2 screenshot here

![Patient Care and Outcome Analysis](insert-dashboard-2-image-link-here)

# 💡 Key Insights

The hospital is operating at a high activity level, with strong admission and doctor-visit volume across the reporting period. This suggests a busy care environment where both operational coordination and staff responsiveness are critical.

Emergency stands out as a major workload center, while Pulmonology and Cardiology also show substantial activity. This indicates that pressure is spread across multiple clinically important departments rather than concentrated in one area alone.

The average hospital stay suggests that many admissions are not quick-turnover cases. This points to sustained bed occupancy and moderate treatment complexity, both of which affect capacity planning and patient flow.

Doctor activity is strong overall, but average response time indicates that responsiveness may be under pressure. In real hospital settings, this matters because moderate delays may still affect deteriorating patients even if routine cases remain manageable.

On the patient care side, Recovered remains the dominant outcome, which suggests that the hospital is generally effective in delivering successful treatment for most patients. However, the continued presence of ICU, readmitted, and deceased cases across departments shows that the hospital is also managing a meaningful number of medically vulnerable patients.

The abnormal vital pattern is one of the strongest clinical signals in the analysis. A high level of abnormal or critical vital activity suggests the hospital is caring for many unstable patients whose conditions may change quickly and require urgent intervention.

Departmental outcome patterns show that recovery is strongest overall, but some departments carry a heavier burden of ICU or readmitted outcomes. This suggests that patient risk and clinical complexity are not evenly distributed across the hospital.

The demographic and chronic-condition patterns strengthen this picture further. Older patients and those living with conditions such as asthma, heart disease, hypertension, and diabetes appear more exposed to care complexity, which is realistic in hospital settings where chronic disease often increases the likelihood of complications, slower recovery, and repeat hospital use.

Taken together, the dashboards show that hospital operations and patient care outcomes are closely linked. High admissions, longer stays, response-time pressure, unstable vitals, and chronic disease burden are not separate issues. They form part of the same broader hospital performance story.

# 🩺 Recommendations

I would recommend that the hospital uses these dashboards as both an operational monitoring tool and a patient safety support tool. In real-life hospital settings, departments with high admissions, longer stays, and strong doctor activity can quickly become pressure points if staffing and workflow do not adjust early enough.

The hospital should review staffing and workflow coverage in the busiest departments, especially where high patient volume overlaps with slower response times. In practice, service pressure often becomes visible through delayed reviews, congested patient flow, and moderate response-time slippage before it becomes a larger operational problem.

Staffing should also be aligned more closely with real demand timing. Hospitals usually experience concentrated activity around ward rounds, escalation periods, handovers, and evening deterioration windows. Matching coverage to those periods can improve responsiveness more effectively than spreading staff evenly across all hours.

On the patient-care side, the hospital should strengthen its response to repeated high-risk or critical vital patterns. In real care settings, these are often the patients most likely to deteriorate further, require ICU escalation, or return through readmission. Earlier warning and faster intervention could reduce avoidable escalation.

Departments with heavier ICU, readmitted, or deceased outcome patterns should be reviewed with context, not judged in isolation. In reality, poorer outcomes may reflect higher-acuity patient populations rather than poor care alone. A more realistic response is to combine outcome analysis with workload, chronic-condition burden, and response-time measures before making performance decisions.

The hospital should also strengthen support for patients with chronic conditions, since those patients are often more vulnerable to relapse, delayed recovery, and repeat hospital use. Better continuity of care, follow-up planning, and transition monitoring would likely improve both patient outcomes and operational efficiency.

Finally, I would recommend that the hospital pays close attention to patients leaving higher-acuity care, especially those moving out of ICU-level treatment. In real-life scenarios, patients may appear stable enough for transfer or discharge while still remaining medically fragile underneath. Better transition monitoring could reduce later deterioration, readmission, and poor outcomes.

# ✨ Overall Reflection

What stood out most to me in this project is how closely hospital operations and patient outcomes are connected. The analysis made it clear that the hospital is not simply busy; it is managing a patient population with both operational pressure and clinical complexity.

This project gave me the chance to analyze hospital data in a practical way that goes beyond reporting numbers. The dashboards help show where attention is needed, where patient risk may be increasing, and where operational or clinical improvements could make the greatest difference.
