# InsightFlow Dynamic Analytics

## AI-Powered Dynamic CSV Data Analysis & Business Reporting

InsightFlow Dynamic Analytics is an automated data analytics workflow built with **n8n** that transforms uploaded CSV datasets into structured business insights, dynamic KPIs, AI-generated management reports, and formatted email reports.

The system is designed to work with **different types of datasets** without hardcoding the analysis for a specific business domain.

---

## 🎯 Project Objective

The objective of InsightFlow Dynamic Analytics is to automate the repetitive stages of a data analyst's workflow:

CSV Dataset  
→ Data Profiling  
→ Data Quality Analysis  
→ Dynamic KPI Generation  
→ AI Business Analysis  
→ Management Report  
→ Email Delivery

The workflow dynamically detects the characteristics of the uploaded dataset and generates relevant analysis based on the available columns and data.

---

## 🏗️ Workflow Architecture

```text
                    CSV DATASET
                         │
                         ▼
                ┌─────────────────┐
                │   CSV Upload    │
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │ Dataset Profile │
                │ & Data Quality  │
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │ Dynamic KPI     │
                │ Engine          │
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │ Business Insight│
                │ Preparation     │
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │ Google Gemini   │
                │ AI Analysis     │
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │ Report Formatter│
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │   HTML Email    │
                │ Report          │
                └─────────────────┘
## 📸 Project Demo

### 1. Complete Automation Workflow

The complete n8n workflow connects dataset ingestion, profiling, dynamic KPI generation, AI analysis, report formatting, and email delivery.

![InsightFlow Dynamic Analytics Workflow](workflow.png)

---

### 2. Dynamic KPI Engine

The KPI engine analyzes the structure and available metrics of the uploaded dataset and generates relevant analytical information dynamically.

![Dynamic KPI Engine](dynamic-kpi.png)

---

### 3. AI-Generated Business Report

Google Gemini converts the structured KPI information into a management-oriented business report.

![AI Business Report](ai-report.png)

---

### 4. Automated HTML Email Report

The final business report is formatted into a professional HTML email for automated delivery.

![Automated Email Report](email-report.png)

🔄 How It Works
1. CSV Data Ingestion

The workflow receives a CSV dataset and extracts the available records.

The dataset is not assumed to belong to a particular business domain.

2. Dataset Profiling

The workflow identifies:

Number of rows
Number of columns
Numeric columns
Categorical columns
Date columns
Missing values
Duplicate records
Data-quality status
3. Dynamic KPI Engine

The Dynamic KPI Engine automatically calculates KPIs based on the available data.

For numeric columns it can calculate:

Count
Sum
Average
Minimum
Maximum

For categorical columns it can calculate:

Unique values
Top categories
Category frequency

For date columns it can identify:

Valid date records
Earliest date
Latest date

The KPI engine does not depend on a single predefined dataset.

4. Automatic Dataset Detection

The workflow can identify the general dataset category based on available column information.

Examples may include:

Sales
Customer
Employee / HR
Education
Subscription
General business datasets

The analysis is based on the supplied data rather than assuming a fixed dataset type.

5. AI Business Analysis

The generated KPI information is passed to Google Gemini.

The AI is instructed to:

Use only supplied KPI information
Avoid inventing numbers
Avoid unsupported trends
Identify business risks
Identify opportunities
Provide practical recommendations
Clearly distinguish facts from interpretation
6. Management Report

The AI generates a structured business report containing sections such as:

Executive Summary
Key Findings
Entity / Customer Analysis
Product / Category Analysis
Revenue / Financial Analysis
Geographic Analysis
Risks
Recommendations
Management Questions

Sections that cannot be supported by the available dataset are identified as unavailable or not applicable.

7. HTML Email Report

The final report is converted into a professional HTML email format.

The email contains:

Professional header
Report title
Structured sections
Business insights
Recommendations
Automated footer
🛠️ Technology Stack
Technology	Purpose
n8n	Workflow automation
Google Gemini	AI business analysis
JavaScript	Dynamic KPI and workflow logic
CSV	Dataset input
HTML/CSS	Email report formatting
Google Drive	Dataset storage / integration
📊 Key Features
Dynamic Dataset Support

The workflow is designed to process different CSV datasets rather than being limited to one dataset.

Dynamic KPI Generation

KPIs are generated from the detected column types and available information.

Data Quality Monitoring

The workflow identifies important data-quality indicators such as:

Missing values
Duplicate records
Quality status
AI-Assisted Business Analysis

Google Gemini converts structured KPI information into a management-oriented report.

Automated Reporting

The final report can be delivered through email without manually preparing the report.

🔐 Data & Security

Sensitive information such as:

API keys
Passwords
OAuth tokens
Private credentials

should never be committed to this repository.

The workflow configuration should be reviewed before sharing publicly.

🚀 Future Improvements

Potential future improvements include:

Automated Google Drive dataset ingestion
Scheduled reporting
Multi-dataset analysis
Advanced anomaly detection
Automated dashboard generation
Historical KPI comparison
Trend analysis
Business alert generation
Power BI integration
👩‍💻 Author

Janki Patel

Data Analyst | Python | SQL | Excel | Power BI | Pandas | NumPy | n8n | Generative AI
                
