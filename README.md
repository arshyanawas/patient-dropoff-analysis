# Patient No-Show Analytics Dashboard

![Python](https://img.shields.io/badge/Python-3.11-blue)
![Streamlit](https://img.shields.io/badge/Streamlit-Dashboard-red)
![Pandas](https://img.shields.io/badge/Pandas-EDA-green)
![Healthcare Analytics](https://img.shields.io/badge/Domain-Healthcare-purple)
![SQL](https://img.shields.io/badge/SQL-Analytics-orange)

[![Live App](https://img.shields.io/badge/Streamlit-Live_App-red)](https://patient-dropoff-analysis.streamlit.app/)

## Live Demo

[Open Dashboard](https://patient-dropoff-analysis.streamlit.app/)

---

## Executive Summary

This project analyzes **110,000+ hospital appointments** to uncover patterns behind patient no-shows and operational drop-offs. Using funnel analysis, behavioral segmentation, and an interactive Streamlit dashboard, the analysis identifies waiting time and patient behavior as major drivers of missed appointments and proposes practical strategies to improve attendance and resource utilization.

**Key Insight:** Nearly **1 in 5 patients** fail to attend their scheduled appointments, highlighting a significant operational challenge for healthcare providers.

---

## Business Problem

Missed appointments are more than a scheduling issue—they directly affect hospital efficiency and resource utilization.

Key operational impacts include:

* Idle doctor and staff time
* Increased operational costs
* Reduced patient throughput
* Lower appointment utilization rates
* Scheduling inefficiencies across departments

Understanding where and why patients drop off is essential for improving patient attendance and maximizing healthcare resources.

---

## Dataset

* **Dataset Size:** 110,526 hospital appointments
* **Domain:** Healthcare Operations
* **Focus Area:** Patient Attendance Behavior
* **Objective:** Identify drivers of patient no-shows and recommend operational improvements

---

## Analysis & Key Findings

### 1. Funnel Analysis

![Funnel Chart](results/charts/funnel_chart.png)

#### Insight

Out of **110,526 scheduled appointments**, only **88,207 were attended**, resulting in an approximate **20% drop-off rate**.

The drop occurs entirely at the final stage (**Scheduled → Attended**), indicating that the primary challenge lies in patient follow-through rather than appointment acquisition.

This suggests that improvements in scheduling experience, reminder systems, and attendance management could significantly improve operational efficiency.

---

### 2. No-Show Rate by Age Group

![Age Analysis](results/charts/age_no_show.png)

#### Insight

Adults and children exhibit the highest no-show rates at approximately **22–23%**.

Senior patients show significantly lower no-show rates at approximately **15%**, indicating stronger healthcare engagement and appointment commitment.

This finding highlights the need for age-specific engagement strategies, particularly for working-age adults and parents managing children's appointments.

---

### 3. SMS Reminder Effectiveness

![SMS Analysis](results/charts/sms_no_show.png)

#### Insight

Patients who received SMS reminders show a higher no-show rate (**~27%**) than patients who did not (**~17%**).

Rather than proving SMS reminders are ineffective, this likely indicates that reminders are being sent to already high-risk patients.

The finding suggests that reminder timing, message content, and communication channels should be reevaluated to improve effectiveness.

---

### 4. No-Show Rate by Day of Week

![Weekday Analysis](results/charts/weekday_no_show.png)

#### Insight

Attendance behavior varies across the week.

* Tuesday and Wednesday show the highest no-show rates (~23%)
* Thursday demonstrates the lowest no-show rate (~19%)

These patterns suggest opportunities for appointment redistribution and improved scheduling strategies that reduce risk during high-drop-off periods.

---

### 5. Interactive Dashboard

[Open Dashboard](https://patient-dropoff-analysis.streamlit.app/)

#### Dashboard Capabilities

The Streamlit dashboard enables stakeholders to:

* Explore patient attendance behavior interactively
* Identify high-risk patient segments
* Compare performance across demographics
* Monitor no-show trends
* Translate analytical findings into operational decisions

---

## Business Impact

Out of **110,526 scheduled appointments**, approximately **22,319 appointments were missed**.

Assuming an average appointment value of **₹500**, these missed appointments represent approximately:

**₹1.1 Crore in unrealized appointment value**

Beyond direct financial implications, no-shows contribute to:

* Inefficient resource allocation
* Reduced healthcare accessibility
* Lower staff productivity
* Increased scheduling complexity

This demonstrates why reducing no-show rates can deliver significant operational and financial benefits.

---

## Recommended Mitigation Strategies

### 1. Reduce Waiting Time

* Prioritize appointments within 3–5 days
* Optimize scheduling workflows to reduce backlog
* Monitor wait-time thresholds associated with higher no-show risk

### 2. Improve Reminder Systems

* Send reminders 24 hours before appointments
* Introduce same-day reminder notifications
* Use multiple communication channels (SMS, email, app notifications)

### 3. Target High-Risk Segments

* Identify patients with extended waiting periods
* Provide flexible rescheduling options
* Focus intervention efforts on higher-risk demographic groups

### 4. Optimize Scheduling Strategy

* Implement controlled overbooking using historical attendance data
* Balance appointment loads based on expected attendance patterns
* Continuously monitor attendance trends and adjust schedules accordingly

---

## Methodology

### Data Preparation

* Cleaned and standardized raw appointment data
* Processed date and time fields
* Removed inconsistencies and invalid records

### Feature Engineering

Created analytical features including:

* `waiting_days`
* `age_group`
* `appointment_dayofweek`

### Analytical Approach

* Funnel Analysis
* Behavioral Segmentation
* Attendance Pattern Analysis
* Demographic Analysis
* Operational Performance Assessment

---

## Tools & Technologies

* Python
* Pandas
* NumPy
* Plotly
* Streamlit

---

## Limitations

* No geographic information for regional analysis
* No patient history data for repeat attendance behavior
* Limited visibility into socioeconomic factors influencing attendance

---

## Future Improvements

* Build a predictive no-show risk model
* Integrate real-time scheduling data
* Add attendance forecasting capabilities
* Expand dashboard functionality with trend monitoring
* Incorporate patient history and behavioral scoring

---

## Project Structure

```text
hospital_funnel/
├── data/
├── scripts/
├── dashboard/
├── results/
└── README.md
```

---

## Key Takeaway

This project demonstrates the ability to:

* Translate healthcare data into actionable business insights
* Identify operational inefficiencies through funnel analysis
* Build interactive dashboards for decision-making
* Apply analytical thinking to real-world healthcare challenges
* Recommend data-driven operational improvements

```

Healthcare analytics is most valuable when insights lead to measurable action. This project focuses on turning patient attendance data into practical recommendations that improve operational efficiency and patient outcomes.
```
