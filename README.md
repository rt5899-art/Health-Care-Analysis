# Healthcare Patient and Operational Performance Analysis Dashboard

## Project Overview

This repository contains a healthcare data analytics project built to monitor and evaluate patient volumes, admissions trends, medical condition frequencies, and demographic distributions. The primary objective of this project is to centralize hospital transactional records and patient profiles into an interactive administrative dashboard. By providing real-time operational visibility, this project solves the challenge of disconnected clinical datasets, enabling hospital administrators to track target thresholds, evaluate regional resource demands, and optimize clinical capacity planning.

## Business Problem

Healthcare organizations generate large volumes of patient and operational data. Without proper analysis, it becomes difficult to:

- Track patient volumes over time.
  
- Monitor billing performance.
  
- Understand trends in medical conditions.
  
- Evaluate hospital and insurance provider performance.
  
- Identify opportunities to improve patient care and operational efficiency.

This dashboard addresses these challenges through interactive visualizations and KPI monitoring.

## Project Requirements

The objective of the project was to:

1. Analyze patient admission trends.
 
2. Monitor total patient count.
 
3. Evaluate billing-related performance.
 
4. Analyze patient demographics.
 
5. Understand medical condition trends.
 
6. Measure patient stay duration.
 
7. Enable filtering by hospital and insurance provider.
 
8. Generate actionable insights for healthcare management.


## Tools and Technologies Used

- Power BI Desktop
 
- Power Query

- DAX (Data Analysis Expressions)

- Data Modeling

- Data Visualization

- Healthcare Dataset

## Data Preparation

The following data preparation activities were performed:

- Data cleaning and validation

- Handling missing values

- Data type correction

- Date transformation for trend analysis

- Creation of calculated measures and KPIs

- Data modeling and relationship management

## Dashboard Features

![image alt](https://github.com/rt5899-art/Health-Care-Analysis/blob/main/ss-%20Health%20care%20BI.png?raw=true)


## Challenges Faced

Overlapped X-Axis Label Text: Displaying long physician names (e.g., Michael Johnson, Michael Smith) and dense date lines on historical column charts led to visual compression and label truncation. This layout challenge was overcome by customizing row-width allocations, adjusting side margins, and establishing responsive font constraints.

Complex Multi-Series Line Alignment: Tracking six separate chronic medical conditions simultaneously across a continuous 12-month calendar created visual noise and trace-line crossovers. This was resolved by grouping data types efficiently and configuring targeted data labels at major peaks to preserve visual legibility.

Synchronizing Goal KPI Thresholds: Setting up custom KPI cards that show variance progress against explicit, hardcoded targets (such as monthly patient volume ceilings and financial revenue limits) required building advanced, conditional DAX measures to cleanly handle negative and positive percentage variances.

### Key Insights

An evaluation of the metrics processed across the healthcare analytics interface reveals the following clinical and operational insights:

High-Level Operational Target Variances: The hospital tracks current operational performance directly against standard administrative goals. Last Month Patient Count reached 4.65K, which represents a -7.02% deficit against the 5K patient target. Conversely, revenue tracking reveals a strong positive position, capturing 118.84M against a 100M baseline goal, representing an +18.84% positive variance. The system also logs an explicit indicator score of 51.17 and a specific target marker score of 16 against a target baseline of 10.

Chronic Medical Condition Seasonality Profiles: Monthly tracking of patient volumes across six core medical conditions reveals highly consistent volume tiers throughout the calendar year:

High-Volume Segment: Diabetes and Hypertension consistently lead admission volumes, tracking between 1,000 and 1,256 patients per month. Diabetes reached a noticeable operational peak in July at 1,256 patients, while Hypertension maintained an elevated presence throughout June (1,181) and July (1,188). Obesity acts as a solid third volume driver, tracking near the 1,100 to 1,180 patient range.

Low-Volume Segment: Asthma, Cancer, and Arthritis represent a separate, lower-tier volume grouping, with each condition consistently tracking between 300 and 509 monthly patients. The maximum peak within this lower tier was recorded for Cancer admissions in August at 509 patients.

Demographic Volume Trends and Gender Split: Longitudinal historical analysis shows that patient admission volumes grew from a 2019 baseline (3K Female, 4K Male) to achieve maximum operational saturation across the 2020 to 2023 windows, maintaining a steady run-rate of approximately 10K total patients per year. Gender distributions remain balanced, with Female and Male patient volumes reflecting nearly equal shares (averaging 5K to 6K each per year), while a small Non-binary segment is consistently tracked across all periods. The 2024 data block shows a partial-year recording tracking at 4K Female and 2K Male admissions.

Patient Distribution by Blood Group: Blood type categorization highlights specific distribution volumes. Type A+ represents the largest operational patient cluster, capturing 19.43K (35%) of the total distribution. Type O+ represents the second-largest pool at 13.88K (25%), followed by Type O- at 8.33K (15%). Remaining blood types, including A-, AB-, AB+, and B-, make up smaller 5% individual shares.

Physician Caseload Rankings: Tracking patient volume across individual staff members isolates peak operational assignments. Dr. Michael Smith managed the highest patient caseload at 27 assignments, followed by Dr. John Smith and Dr. Robert Smith at 22 cases each, and Dr. James Smith alongside Dr. Michael Johnson tracking identical volumes at 20 cases each.

### Recommendations for Improvements

Deploy Target Interventions for the July Diabetes Peak: Because Diabetes admissions experience a seasonal surge that peaks at 1,256 patients in July, hospital management should proactively allocate additional endocrinology staff, diabetic care consumables, and outpatient monitoring resources in late Q2 to handle this predictable influx.

Address the Last Month Patient Count Deficit: The dashboard displays a -7.02% deficit (4.65K actual vs 5K target) in recent patient volumes. Clinical coordinators should analyze outpatient scheduling workflows, referral channels, and check-in processing to remove administrative barriers that could be depressing patient throughput.

Audit High-Volume Blood Group Inventories: Given that Type A+ (35% / 19.43K) and Type O+ (25% / 13.88K) safely constitute a 60% supermajority of the patient profile, the hospital's central blood bank should adjust its minimum stock thresholds to guarantee that blood supply lines match this high demographic concentration.

Balance Doctor Caseloads to Prevent Burnout: Case assignment tracking shows that Dr. Michael Smith handles the highest workload at 27 cases. Implementing an automated scheduling or triaging system would distribute new admissions more evenly to peers like Dr. James Smith (20 cases), ensuring balanced caseloads and maintaining high patient care standards.

## Conclusion

The Health Care Analysis Dashboard transforms raw healthcare data into meaningful business insights. Through KPI monitoring, trend analysis, demographic evaluation, and operational reporting, the solution supports better healthcare management, improved decision-making, and enhanced operational efficiency.
