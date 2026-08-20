# ConveGenius.AI – School Analytics Dashboard

> A Power BI analytics solution designed to provide a comprehensive view of school infrastructure, student learning outcomes, assessment performance, attendance, and academic performance across districts, blocks, and schools.

---

## 📊 Project Overview

The **ConveGenius.AI School Analytics Dashboard** is a multi-page Power BI reporting solution developed to transform school-level operational and academic data into actionable insights.

The dashboard brings together information related to:

* School infrastructure and resources
* Teachers and student population
* Student assessment performance
* Learning outcomes
* Attendance patterns
* Academic performance
* District and school-level comparisons

The solution enables users to interactively explore the data using filters for districts, blocks, schools, management types, school categories, grades, subjects, and session types.

---

## 🎯 Business Objective

The primary objective of this project is to help education stakeholders monitor school performance and identify areas requiring attention.

The dashboard is designed to answer questions such as:

* How many schools, teachers, and students are covered?
* Which districts have stronger infrastructure performance?
* Which schools have the highest infrastructure scores?
* How are students distributed across performance levels?
* Which learning outcomes are performing well or poorly?
* What is the relationship between attendance and academic performance?
* Which districts require additional attention?
* What does the teacher retirement outlook look like?

---

# 📑 Dashboard Pages

## 1. School Infrastructure & Resource Overview

This page provides an overview of school infrastructure, resources, teachers, and students.

### Key Metrics

* Total Schools
* Total Teachers
* Total Students
* Average Teacher Experience
* Pupil-Teacher Ratio (PTR)
* Average Students per School

### Key Visuals

* District-wise School Count by PTR Category
* Top 10 Schools by Infrastructure Score
* Teachers Approaching Retirement in the Next 5 Years
* District-level infrastructure comparisons
* Key infrastructure insights

### Purpose

This page helps identify differences in school resources and infrastructure across districts and schools.

---

## 2. Student Learning & Assessment Performance

This page focuses on student assessment performance and learning outcomes.

### Key Metrics

* Average Score
* Schools Participated
* Students Participated

### Key Visuals

* School-wise Performance Matrix
* District → Block → School hierarchy
* Student Distribution by Performance Level
* Top 10 Learning Outcomes
* Bottom 10 Learning Outcomes
* District-level performance comparison

### Purpose

This page helps education stakeholders understand student achievement, participation, and learning outcome performance across different geographical and academic dimensions.

---

## 3. Attendance Monitoring & Performance Correlation

This page focuses on attendance and its relationship with academic performance.

### Key Metrics

* Teacher Attendance Marked %
* Student Attendance Marked %
* Average Teacher Attendance
* Average Student Attendance

### Key Visuals

* Attendance vs Academic Performance scatter plot
* District-wise Performance Overview
* Attendance comparison
* Infrastructure vs performance comparison

### Purpose

This page helps identify attendance patterns and explore their relationship with student academic performance.

---

# 🗂️ Data Sources

The analysis uses multiple datasets covering different aspects of the education ecosystem:

| Dataset            | Description                                           |
| ------------------ | ----------------------------------------------------- |
| School Registry    | School information, infrastructure and classification |
| Student Registry   | Student-level information                             |
| Teacher Registry   | Teacher information and experience-related attributes |
| Assessment Dataset | Student assessment and learning outcome data          |
| Attendance Dataset | Teacher and student attendance information            |

> **Note:** Raw datasets are not included in this public repository. The dashboard was developed using datasets provided for the project/assessment.

---

# 🔄 Data Preparation

Data preparation and transformation were performed using **Power Query**.

Major preparation steps included:

* Data type correction
* Missing value handling
* Column standardization
* Data cleaning
* Duplicate handling
* Date transformation
* Data categorization
* Relationship preparation
* Creation of analytical fields
* Transformation of assessment and attendance data

---

# 🧩 Data Model

The Power BI solution combines multiple datasets to provide an integrated analytical model.

The model connects key entities such as:

```text
School
   │
   ├── Student
   │
   ├── Teacher
   │
   ├── Attendance
   │
   └── Assessment
```

The model enables analysis across:

**District → Block → School → Student / Teacher**

and supports interactive filtering throughout the report.

---

# 🧮 DAX & Measures

DAX was used to create analytical measures and KPIs including:

* Total Schools
* Total Teachers
* Total Students
* Average Score
* Average Teacher Experience
* Pupil-Teacher Ratio
* Students per School
* Attendance Metrics
* Infrastructure Metrics
* Learning Outcome Metrics
* Performance Level Distribution

Example:

```DAX
PTR Ratio =
DIVIDE(
    [Total Students],
    [Total Teachers]
)
```

---

# 🛠️ Tools & Technologies

### Business Intelligence

* Microsoft Power BI Desktop
* Power BI Service

### Data Transformation

* Power Query

### Data Analysis

* DAX
* Excel

### Visualization

* Power BI Visualizations
* Interactive Slicers
* KPI Cards
* Matrix
* Bar Charts
* Scatter Plot
* Conditional Formatting

---

# 🎨 Dashboard Features

The dashboard includes:

* Interactive page navigation
* Global filters
* KPI cards
* Drill-down hierarchy
* District-level analysis
* School-level analysis
* Top/Bottom performance analysis
* Interactive visual cross-filtering
* Conditional formatting
* Insight summaries
* Consistent ConveGenius.AI visual theme

---

# 📸 Dashboard Preview

### School Infrastructure & Resource Overview

![School Infrastructure Dashboard](https://github.com/RusshikeshPatil/ConveGenius-School-Analytics-PowerBI/tree/main/Dashboard)

---

### Student Learning & Assessment Performance

![Student Learning Dashboard](https://github.com/RusshikeshPatil/ConveGenius-School-Analytics-PowerBI/blob/main/Dashboard/02-Student-Learning-Assessment.png)

---

### Attendance Monitoring & Performance Correlation

![Attendance Dashboard](https://github.com/RusshikeshPatil/ConveGenius-School-Analytics-PowerBI/blob/main/Dashboard/03-Attendance-Performance-Correlation.png)

---

# 💡 Key Analytical Insights

The dashboard enables users to identify patterns such as:

* Differences in infrastructure performance across districts
* Districts with higher concentrations of schools in specific PTR categories
* Schools with stronger infrastructure scores
* Distribution of students across performance levels
* High- and low-performing learning outcomes
* Differences in academic performance across districts
* Attendance patterns across schools and districts
* Potential relationships between attendance and academic performance
* Teacher retirement trends requiring workforce planning

> Insights shown in the dashboard are dynamically affected by the selected filters.

---

# 📈 Business Value

This dashboard transforms raw education data into an interactive decision-support solution.

It can support:

* School resource planning
* Infrastructure monitoring
* Academic performance tracking
* Learning outcome improvement
* Attendance monitoring
* Teacher workforce planning
* District-level performance comparison
* Identification of areas requiring intervention

---

# 🚀 Project Highlights

* Built a **3-page interactive Power BI dashboard**
* Integrated **5 education-related datasets**
* Developed reusable DAX measures
* Created hierarchical district → block → school analysis
* Implemented interactive filtering and navigation
* Designed an executive-friendly dashboard interface
* Applied consistent visual hierarchy and color standards
* Combined operational, infrastructure, attendance, and academic metrics into one analytical solution

---

# 📁 Repository Structure

```text
ConveGenius-School-Analytics-PowerBI/
│
├── Dashboard/
│   ├── 01-School-Infrastructure.png
│   ├── 02-Student-Learning-Assessment.png
│   └── 03-Attendance-Performance-Correlation.png
│
├── Documentation/
│   └── Project-Overview.pdf
│
├── PowerBI/
│   └── ConveGenius-School-Analytics.pbix
│
├── Data/
│   └── README.md
│
└── README.md
```

---

# ⚠️ Data Privacy

The original datasets used for this project are not publicly distributed in this repository.

Only dashboard screenshots, documentation, and the Power BI project file are intended for portfolio demonstration, subject to applicable data-sharing permissions.

---

# 👨‍💻 Skills Demonstrated

**Power BI | DAX | Power Query | Data Modeling | Data Cleaning | Data Visualization | Dashboard Design | KPI Development | Business Intelligence | Data Analysis | Education Analytics**

---

## 📌 Project Type

**Business Intelligence / Data Analytics / Power BI**

**Domain:** Education Analytics

**Tool:** Microsoft Power BI

---

## ⭐ If you find this project useful

Feel free to explore the dashboard design and analytical approach.
