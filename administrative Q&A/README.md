# 🏥 Administrative Questions and Answers

For this part of the project, I used **DAX** to answer the specific administrative questions provided for the dataset. My goal here was not just to build visuals, but to translate each business question into measurable logic inside Power BI so the answers could update dynamically with the data.

I started by breaking each question into the exact logic it required, especially where time-based analysis was involved, such as **past 48 hours**, **current month**, **past 7 days**, **past 14 days**, **past 3 months**, **within 30 days**, and **subsequent admissions**.

To answer them accurately, I:
- 📅 created time-based columns such as month, month-year, visit hour, and date-difference logic
- 🚨 built risk classification columns for vitals such as **Normal**, **Moderate**, **High**, and **Critical**
- 🔁 calculated readmission logic using previous admission dates and days since last admission
- 📊 created summary tables and measures to isolate top patients, delayed doctors, and department-level trends
- ✅ validated the results against filtered source data to ensure consistency

This section focuses only on the **administrative questions and answers**.



## ❤️ 1. Patient Risk and Vitals

### Question 1  
**Which patients have recorded abnormal vital signs within the past 48 hours?**

### Answer  
I used timestamp-based logic to isolate the most recent 48-hour window from the vitals table, then filtered the results to show only patients classified as **High** or **Critical** risk.

### Question 2  
**Who are the top 10 patients with the highest frequency of abnormal vital readings over the current month?**

### Answer  
I filtered the vitals data to the current month, kept only abnormal readings, then ranked patients by the number of occurrences to identify the top 10.

### 💡 Insight  
This part of the analysis showed that patient instability is not just a one-time event. A small group of patients appeared repeatedly with abnormal vital readings, which suggests persistent clinical instability, unresolved illness, or delayed recovery.

### 🩺 Recommendation  
I would recommend that the hospital treats these patients as a priority monitoring group. In hospital settings, repeated abnormal vitals often appear before major escalation such as ICU transfer, emergency intervention, or readmission. A practical response would be to create an automatic review list for patients with repeated high-risk readings so clinicians can intervene earlier instead of waiting until the case becomes critical.



## 🔁 2. Admissions and Readmissions

### Question 3  
**What proportion of patients discharged from the hospital were readmitted within 30 days?**

### Answer  
I created DAX logic to identify each patient’s previous admission date, calculate the number of days between admissions, and flag readmissions that occurred within 30 days. From there, I calculated the readmission proportion.

### Question 4  
**Which departments are associated with the highest rates of patient readmission?**

### Answer  
I compared readmission rates across departments and visualized the result to identify where readmission pressure was highest.

### 💡 Insight  
The readmission rate stood out as one of the strongest operational warning signs in the project. The results suggest that some patients are returning to the hospital too quickly after discharge, especially in departments handling more clinically fragile patients or chronic-condition cases.

### 🩺 Recommendation  
I would recommend that management reviews discharge planning and follow-up pathways in the highest-readmission departments. In hospital scenarios, high readmission is often linked to incomplete recovery, weak discharge communication, poor medication understanding, or missed follow-up. A realistic intervention would be stronger discharge counseling, earlier outpatient review, and closer follow-up for high-risk patients, especially those leaving Pulmonology, Cardiology, or ICU-related care.



## ⏱️ 3. Doctor Responsiveness

### Question 5  
**What is the average doctor response time across departments over the past seven days?**

### Answer  
I filtered doctor visit records to the past 7 days and calculated the average response time by department.

### Question 6  
**Which doctors have an average response time greater than 10 minutes over the past 14 days?**

### Answer  
I summarized doctor activity over the last 14 days, calculated average response times, and filtered the results to show only doctors above the 10-minute threshold.

### 💡 Insight  
The response-time analysis showed that delays were not isolated to one department. While the average response times were not extreme, they were high enough to matter, especially in a hospital setting where even moderate delays can affect deteriorating patients.

### 🩺 Recommendation  
I would recommend that the hospital reviews doctor responsiveness alongside workload rather than judging the numbers in isolation. Slow response times do not always mean poor performance; they can reflect doctors covering multiple wards, high patient volume, or inefficient task allocation. A more realistic hospital action would be to compare response time against staffing levels, ward coverage, and peak activity hours to determine whether the real issue is staffing pressure or workflow design.



## 📈 4. Workload and Capacity

### Question 7  
**What is the count of admissions by department for each of the past three months?**

### Answer  
I created month-based logic and summarized admissions by department across the last 3 months, displaying the result in a matrix format so each month appeared as a separate column.

### Question 8  
**What are the most common hours for doctor visits based on the recorded visit times?**

### Answer  
I extracted the visit hour from the doctor visit timestamp and counted visit frequency by hour to identify peak consultation periods.

### 💡 Insight  
The workload analysis showed that pressure is not evenly distributed across departments or across the day. Some departments carried noticeably higher admission counts, and doctor visits were concentrated in specific hours rather than spread evenly.

### 🩺 Recommendation  
I would recommend that the hospital uses these patterns for staffing and capacity planning. In real hospital environments, demand usually rises around ward rounds, handovers, escalation periods, and evening deterioration windows. A realistic action would be to align doctor and nursing coverage more closely to the hours where activity peaks, instead of relying on evenly distributed staffing that may not match actual demand.



## 📋 5. Patient Outcomes

### Question 9  
**Among patients recorded with ICU status, how many had subsequent admissions resulting in death?**

### Answer  
To answer this, I tracked patients who had previously been admitted with an ICU outcome and then identified those who later returned with a subsequent admission ending in death. This allowed me to isolate patients whose care pathway progressed from critical illness to later mortality.

### Question 10  
**What is the distribution of patient outcomes (Recovered, ICU, Deceased, Readmitted) by department?**

### Answer  
I compared outcomes across departments to show where recovery was strongest and where ICU, deceased, or readmitted outcomes were more present.

### 💡 Insight  
Although recovered cases remained the dominant outcome overall, the ICU-to-death pattern highlighted a small but very important group of highly vulnerable patients. This suggests that for some patients, surviving the ICU phase did not necessarily mean long-term recovery.

### 🩺 Recommendation  
I would recommend that the hospital reviews the pathway for ICU survivors after discharge or transfer. In standard hospital care, post-ICU patients are often still medically fragile and may deteriorate later due to relapse, complications, infection, or incomplete recovery. A realistic response would be to strengthen post-ICU monitoring, specialist follow-up, and transitional care so these patients are not treated as fully stable too early.


## ✨ My Overall Takeaway from the Administrative Q&A

Working through these questions with DAX helped me move beyond surface-level dashboarding and actually solve the types of operational questions hospital administrators would ask in practice. What stood out most to me was that the answers were connected: abnormal vitals, readmissions, delayed response times, workload peaks, and ICU-related mortality were not separate issues. Together, they told a bigger story about where the hospital may be under pressure and where earlier intervention could improve outcomes.

What I liked most about this part of the project was that it felt practical. I was not just counting records; I was using data to mirror real hospital decisions around patient safety, staff responsiveness, discharge quality, and resource planning.
