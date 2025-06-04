# Google Fiber Customer Service Case Study

## Overview

This repository contains a business intelligence case study focused on analyzing and optimizing Google Fiber's customer service operations. The primary objective is to help BI analysts practice the full project lifecycle: from stakeholder requirements gathering to data modeling, ETL pipeline development, and dashboard design. The case study centers on understanding and reducing repeat customer service calls, thereby improving first-call resolution rates and overall customer satisfaction.

---

## Table of Contents

- [Project Goals](#project-goals)
- [Stakeholder Requirements](#stakeholder-requirements)
- [Dataset Description](#dataset-description)
- [Data Schema & Modeling](#data-schema--modeling)
- [ETL Pipeline](#etl-pipeline)
- [Dashboard Design](#dashboard-design)
- [Key Insights & Recommendations](#key-insights--recommendations)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

---

## Project Goals

- Quantify how often customers call support after their first inquiry
- Identify which customer issues generate more repeat calls
- Explore repeat caller trends across three anonymized market cities
- Enable stakeholders to view trends by week, month, quarter, and year
- Deliver actionable insights to reduce repeat calls and optimize support operations

---

## Stakeholder Requirements

- **Stakeholders:** Google Fiber Customer Service Team, including managers and BI leads
- **Core Questions:**
  - How frequently do customers make repeat calls after their initial contact?
  - Which problem types and markets are associated with higher repeat call volumes?
  - What trends can be observed over different time periods?
- **Desired Outcomes:**
  - Improved first-call resolution rates
  - Enhanced customer satisfaction
  - Data-driven recommendations for operational improvements

---

## Dataset Description

- **Source:** Three CSV files representing customer service interactions from January, February, and March 2022
- **Markets:** Data anonymized into `market_1`, `market_2`, and `market_3`
- **Problem Types:**
  - Type_1: Account management
  - Type_2: Technician troubleshooting
  - Type_3: Scheduling
  - Type_4: Construction
  - Type_5: Internet and Wi-Fi
- **Repeat Calls:** Columns track initial contact and subsequent calls over a seven-day period (e.g., `contacts_n_6` = six days after first contact).

---

## Data Schema & Modeling

- **Entities:** Customer, Market, Problem Type, Contact Event
- **Relationships:** Each contact event is linked to a customer, market, and problem type
- **Schema Documentation:** See `/schemas/` for ERD and JSON schema definitions

---

## ETL Pipeline

- **Extract:** Combine and import CSV files into a unified dataset
- **Transform:** Clean data, anonymize sensitive information, and engineer features (e.g., repeat call flags, time-to-repeat)
- **Load:** Store processed data in a relational database or BI tool for analysis
- **Tools:** SQL, Excel, Power Query, Python (optional)

---

## Dashboard Design

- **Visualization Tools:** Power BI, Tableau, or similar
- **Features:**
  - Dynamic filters by market, problem type, and time period
  - Charts for repeat calls by month, week, and day of week
  - Breakdown of repeat call drivers by issue type and geography
  - Accessibility features (large fonts, screen-reader compatibility)
- **Sample Dashboards:** See `/dashboard/` for screenshots and links to interactive dashboards

---

## Key Insights & Recommendations

- **Findings:**
  - *Internet & Wi-Fi issues (Type_5)* trigger the highest volume of repeat calls, especially in Market 1
  - *Scheduling issues (Type_3)* have lower repeat rates, indicating effective resolution protocols
  - Mondays see the highest volume of first-time contacts; Sundays the lowest
- **Recommendations:**
  - Implement targeted support training for high-repeat categories (e.g., Type_5 in Market 1)
  - Enhance self-service tools such as FAQs and chatbots
  - Monitor first-call resolution KPIs alongside repeat call volume to measure progress

---

## Getting Started
1. Clone this repository:

## Project Structure
/
├── data/ # Raw and sample data files
├── docs/ # Stakeholder requirements and documentation
├── schemas/ # Data schema definitions
├── etl/ # ETL scripts and notebooks
├── dashboard/ # Dashboard files, screenshots, and guides
├── requirements.txt # Dependencies
└── README.md # This file

---

## Contributing

Contributions are welcome! Please submit issues or pull requests to suggest improvements, bug fixes, or new features.

---

## License

This project is licensed under the MIT License.

---

## Acknowledgments

- Inspired by the Google Business Intelligence Professional Certificate capstone project
- Thanks to contributors who shared project documentation and dashboard mockups
- Data and scenario are fictionalized for educational purposes

---

> For more project details and documentation, see the `/docs/` folder and linked dashboard resources.  
> For live dashboard examples, refer to the links provided in the dashboard section.
