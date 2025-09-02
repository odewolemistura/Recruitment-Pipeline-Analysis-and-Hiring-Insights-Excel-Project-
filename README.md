# Recruitment-Pipeline-Analysis-and-Hiring-Insights-Excel-Project-

## Project Overview  

This **Recruitment Pipeline Analysis and Hiring Insights** report is built to enable HR teams to make informed, data-driven choices in talent acquisition and workforce planning. The study examines applicant demographics, qualifications, work experience, salary expectations, and recruitment funnel dynamics. Its purpose is to reveal insights that enhance hiring effectiveness, highlight process bottlenecks, and guide strategic HR planning.  


## Problem Statement  

Recruitment teams often face challenges in making sense of applicant demographics, balancing salary expectations with experience, and ensuring an efficient hiring process. Even with large volumes of application data, it can be difficult to extract actionable insights that support faster and smarter decision-making.  

Common issues include:  
- Monitoring candidate progress through each stage of the hiring funnel  
- Identifying job roles that attract many applicants but few successful hires  
- Detecting mismatches between experience levels and salary demands  
- Limited visibility into regional sourcing trends and pipeline bottlenecks  

The goal of this analysis is to use synthetic recruitment data to deliver insights that streamline hiring, strengthen talent pool management, and guide strategic HR decisions.  

To address these challenges, the following steps were taken.  


## Posing Business Questions  

To drive meaningful insights, I began by identifying key stakeholders (HR managers, recruiters, and talent acquisition leads) and posed essential business questions to guide this analysis:  

1. What is the demographic and educational profile of applicants, and how does this shape the overall talent pool?  
2. How are applications distributed across job titles, countries, and age groups, and what does this reveal about job demand and sourcing regions?  
3. How do years of experience and desired salary expectations align, and what patterns emerge across applicant groups?  
4. Where do candidates drop off within the recruitment funnel, and which stages face the most bottlenecks?  
5. Which job roles convert the highest percentage of applicants into hires, and what factors contribute to their success?  
6. How do application volumes and hiring outcomes vary over time and across experience ranges?  
7. Which countries or regions contribute the most successful hires, and how does this inform sourcing strategies?  

These questions form the foundation of the analysis, focusing on applicant demographics, salary alignment, and recruitment pipeline performance to support data-driven HR decision-making.  


## Dataset Overview  

The dataset used in this project was sourced from **Kaggle** and consists of **synthetic recruitment records** simulating real-world job applications and hiring activity.  

- **Size:** 3,000 applications  
- **Period:** May – August 2023  
- **Coverage:** 600+ unique job titles across multiple countries  

### Key Data Components  
- **Applicant Demographics:** Age, gender, country, city, education level  
- **Professional Background:** Years of experience, desired salary, job title  
- **Application Details:** Application date, applicant ID, status (applied, in review, interviewing, offered, rejected, hired)  
- **Personal Information:** Name, address, contact details (excluded from analysis)  

This dataset enabled a multi-dimensional analysis of applicant profiles, talent pool quality, and recruitment funnel performance to uncover insights that support data-driven HR decision-making.  


## Data Cleaning & Transformation  

Data preparation was conducted in **Power Query** and **Excel**. Key steps included:  

- Merging name fields to create a single full-name column  
- Removing irrelevant columns (e.g., personal contact details)  
- Standardizing data types (dates, numeric values, categorical variables)  
- Calculating applicant age at the time of application and grouping into ranges (18–24, 25–34, 35–44, 45+)  
- Grouping years of experience into ranges (0–2, 3–5, 6–10, 11–15, 16–20)  
- Renaming and reorganizing columns for clarity  

These transformations ensured the dataset was consistent, analysis-ready, and optimized for interactive dashboards using Pivot Tables and Power Pivot.  


## Measures (DAX)  

**Description:** Contains calculated measures created using **DAX** within Power Pivot to derive key recruitment KPIs and track hiring efficiency. These measures form the foundation of the dashboard, providing insights into applicant demographics, salary expectations, and recruitment funnel outcomes.  

**Fields:**  
- Total Applications  
- Average Age  
- Average Desired Salary  
- Average Years of Experience  
- Total Rejected Applications  
- Total Hired Applications  
- Applications in Progress  

**Purpose:**  
Delivers summary metrics that power data-driven analysis of the applicant pool and recruitment process. These measures help HR teams:  
- Track pipeline progress  
- Detect inefficiencies  
- Compare candidate expectations with hiring outcomes  
- Strengthen workforce planning  

## Data Analysis and Visualization  

The dashboard is organized into **two main pages**, each targeting distinct HR objectives and providing actionable insights for recruitment teams and decision-makers.  


## Page 1: Applicant Demographics & Talent Pool Overview  

**Goal:** Understand who is applying and their qualifications.  

![image alt](https://github.com/odewolemistura/Recruitment-Pipeline-Analysis-and-Hiring-Insights-Excel-Project-/blob/390f77c37840cbcf2a7fb545689933d8ddbf0201/Recruitment%20Dashboard1.png)

### Key Metrics (Top of Chart)  

- **Total Applicants**  
- **Average Years of Experience**  
- **Average Age**  
- **Average Desired Salary**  

These headline KPIs provide a quick snapshot of the applicant pool and overall talent profile.  

- **Total Applications**: Represents the full number of job applications submitted during the analysis period.  
- **Average Age**: Highlights the typical age of applicants, giving insight into workforce demographics.  
- **Average Years of Experience**: Shows the general professional background applicants bring to their desired roles.  
- **Average Desired Salary**: Reflects compensation expectations across the applicant pool, helping assess alignment with hiring budget.  

Together, these indicators give HR stakeholders a clear overview of applicant volume, qualifications, and salary expectations, critical for evaluating the strength and composition of the talent pipeline.  

With **Application Month** and **Status** as slicers, these KPIs dynamically update to show how applicant profiles and hiring outcomes shift over time and across recruitment stages, helping stakeholders detect seasonal patterns and focus on specific points in the pipeline.  



## Visualizations (Page 1 – Applicant Demographics & Talent Pool)  

- **Applicant Gender Distribution (Donut Chart):** Displays the breakdown of applicants by gender, providing a quick view of gender diversity within the applicant pool. Supports HR efforts in monitoring inclusivity and demographic balance.  

- **Applicants by Education Level (Bar Chart):** Shows how applicants are distributed across education levels (High School, Bachelor’s, Master’s, PhD). Highlights the qualification profile of the talent pool.  

- **Applicants by Country – Top 10 (Map Chart):** Visualizes the top 10 countries contributing applicants, helping identify sourcing hotspots and geographic patterns in application volume.  

- **Applicant Age Group Distribution (Column Chart):** Segments applicants into defined age brackets (18–24, 25–34, 35–44, 45+). Provides insights into workforce demographics.  

- **Years of Experience vs. Desired Salary (Bar Chart):** Compares average desired salary across grouped experience levels. Reveals how salary expectations scale with professional background, enabling alignment with market benchmarks.  

- **Top 10 Job Titles by Applicant Count (Column Chart):** Highlights job roles with the highest number of applications. Helps HR identify positions attracting the most interest for workforce demand analysis.  



## Page 2: Recruitment Funnel & Hiring Performance  

**Goal:** Track recruitment pipeline efficiency and outcomes.  


![image alt](https://github.com/odewolemistura/Recruitment-Pipeline-Analysis-and-Hiring-Insights-Excel-Project-/blob/068ea5d2c5c9012f819c3beee746755535ff1de4/Recruitment%20Dashboard2.png)


### Key Metrics (Top of Chart)  

- **Total Applications**  
- **Total Hired Applicants**  
- **Total Rejected Applications**  
- **Applications in Progress**  

These recruitment KPIs provide a clear snapshot of hiring outcomes and pipeline efficiency.  

- **Total Hired Applicants** shows the number of candidates who successfully progressed through all recruitment stages and were hired.  
- **Total Rejected Applications** represents applicants who were not selected, helping HR track drop-offs and rejection rates.  
- **Pending Applications** reflects candidates still in progress, offering visibility into the current workload and pipeline status.  
- **Total Applications** confirms the overall applicant volume and serves as a baseline for calculating conversion metrics.  

Together, these measures allow HR teams to assess recruitment performance, monitor conversion rates, and identify potential delays or imbalances within the funnel.  

With **Application Month** and **Status** as slicers, these KPIs dynamically update to show how applicant profiles and hiring outcomes shift over time and across recruitment stages, helping stakeholders detect seasonal patterns and focus on specific points in the pipeline.  



### Visualizations  

- **Recruitment Hiring Status Distribution (Bar Chart):** Displays the number of applicants segmented by hiring status (e.g., Hired, Rejected, In Progress). Highlights the overall distribution of outcomes, helping HR assess pipeline balance and recruitment effectiveness.  

- **Experience Range vs Hiring Status (Clustered Column Chart):** Compares candidate experience ranges against their hiring status. Reveals whether certain experience levels are more likely to progress successfully, supporting better alignment of roles with experience expectations.  

- **Average Desired Salary of Hired Applicants by Job Title – Top 10 (Bar Chart):** Shows the average salary expectations of successfully hired candidates across the ten most common job roles. Provides insights into compensation trends and supports salary benchmarking.  

- **Applications Over Time (Line Chart):** Tracks the number of applications received over time. Identifies recruitment peaks, seasonal trends, and sourcing effectiveness during different periods.  

- **Applications by Job Title & Status – Top 10 Roles (Stacked Bar Chart):** Displays applications across the top 10 job titles, segmented by hiring status. Highlights which roles attract the highest volumes and where conversion challenges exist.  

- **Hires by Country (Map Chart):** Visualizes the geographic distribution of hired candidates. Enables HR to identify regional hiring strengths, sourcing effectiveness, and workforce patterns.  



## Key Analysis Findings  

### Overview  
The dataset contains **3,000 job applications** with:  
- Average applicant age: **40 years**  
- Average work experience: **10 years**  
- Average expected salary: **$65,079**  
- Gender distribution: almost balanced  
- Education levels: evenly split across Bachelor’s, Master’s, PhD, and High School  
- Applications peak: **June and July**  
- Largest group: Professionals aged **45–65**  

### Key Findings  
- The **45–65 age range** dominates applications, suggesting a mature workforce. The **18–24 group** is the smallest, signaling weaker entry-level pipelines.  
- **Gender distribution** is even, with neutral recruitment outcomes showing no visible bias.  
- **Salary expectations** remain consistent ($64k–$66k) across experience levels, suggesting market standardization.  
- **Geography:** Applications are widely spread, but countries like **Korea, India, and Paraguay** contribute notably. Smaller regions (e.g., Falkland Islands, British Virgin Islands) appear disproportionately in hires, hinting at niche roles.  

### Recruitment Journey  

- Out of **3,000 applications**:  
  - **610 hires**  
  - **594 rejections**  
  - **~1,800 in progress**  

- Hiring stages progress evenly across applied → review → interview → offer, showing consistent flow.  

### Conversion Performance  
- **6–10 years of experience** group shows the strongest conversion with fewer drop-offs.  
- **0–2 years (early career)** group faces higher rejection ratios, indicating lower role fit.  

### Job Titles  
- Niche roles (e.g., Translator, Therapeutic Radiographer) progress heavily into interviews but face high rejection later.  
- Roles like **Administrator** and **Sound Technician** show higher offer-to-hire success.  

### Country Insights  
- Hiring is globally distributed, with multiple smaller countries contributing equally. No single geography dominates.  

### Salary Trends in Hires  
- Highest-paying hires fall into **specialist/professional roles** (e.g., Associate Professors, Hospital Doctors, Psychologists) averaging **~$99k**, showing a premium on expertise.  



## Recommendations  

1. **Strengthen Early-Career Recruitment**  
   - Introduce graduate trainee programs, internships, or mentorships to improve entry-level fit and long-term hiring success.  

2. **Target High-Conversion Experience Groups**  
   - Prioritize applicants with **6–10 years experience** for mid-level roles to maintain efficiency and reduce drop-offs.  

3. **Optimize Specialized Role Screening**  
   - Refine pre-screening/skill assessments for niche roles (e.g., Translators, Radiographers) to reduce mismatches earlier.  

4. **Enhance Geographic Strategy**  
   - Focus on high-performing regions contributing disproportionately to hires, instead of spreading efforts evenly.  

5. **Align Salary Structures**  
   - Adjust job postings to reflect realistic salary ranges per role level, aligning candidate expectations with outcomes.  

6. **Reduce Funnel Abandonment**  
   - Use automated communication (status updates, nudges, assessments) to shorten cycle time and improve candidate experience.  



## Limitations  

- **Data Scope:** Only 3,000 applications, limiting broader generalization.  
- **Time Dimension:** Covers May–Aug 2023 only; seasonal peaks may not be recurring trends.  
- **Job Title Variety:** 600+ roles, with some having too few applicants for reliable insights.  
- **Geographic Bias:** Uneven representation; outliers (e.g., Falkland Islands) exaggerated due to low counts.  
- **Salary Insights:** Based on self-reported expectations, not actual negotiated offers.  
- **Incomplete Funnel Outcomes:** ~60% of candidates remain "in progress," so conversion ratios may shift as more outcomes finalize.  
