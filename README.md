# Corporate Learning Lakehouse

Portfolio-ready Analytics Engineering and Learning Analytics platform using Databricks, PySpark and Medallion Architecture concepts.

---

# Business Context

Organizations investing in Data Literacy, AI Enablement and corporate learning often struggle to:

- measure learning adoption
- track course completion
- identify engagement patterns
- monitor AI Enablement initiatives
- generate executive-level learning KPIs
- connect training initiatives to business outcomes

This project simulates a modern corporate learning ecosystem and builds a scalable analytics platform to transform raw learning data into trusted business metrics.

---

# Project Goals

- Build a Medallion Architecture pipeline
- Simulate enterprise learning data
- Apply Analytics Engineering practices
- Create business-ready KPIs
- Demonstrate Databricks and PySpark workflows
- Apply governance and data quality concepts
- Prepare future integrations with AI and front-end applications

---

# Architecture

## Bronze Layer
Raw ingestion layer containing source learning data.

Examples:
- users_raw
- courses_raw
- enrollments_raw
- learning_events_raw

---

## Silver Layer
Cleaned, standardized and validated datasets.

Examples:
- users
- courses
- enrollments
- learning_events

---

## Gold Layer
Business-ready metrics and analytical views.

Examples:
- learning_adoption_by_persona
- course_completion_rate
- ai_enablement_kpis
- monthly_learning_engagement

---

# Tech Stack

## Data & Analytics
- Databricks
- PySpark
- Delta Lake
- SQL
- Python
- pandas

## Engineering
- GitHub
- WSL2
- Linux
- VS Code

## Future Roadmap
- Azure
- Terraform
- React Front-end
- Azure OpenAI
- Databricks Genie
- Power BI

---

# Repository Structure

```txt
corporate-learning-lakehouse/
├── data/
├── notebooks/
├── docs/
├── scripts/
├── sql/
├── tests/
└── assets/
```

---

# Business KPIs

This project generates metrics such as:

- course completion rate
- learning adoption by persona
- AI Enablement engagement
- monthly active learners
- learning funnel conversion
- average completion time
- training participation trends

---

# Data Strategy

All datasets are synthetic and generated exclusively for portfolio and educational purposes.

No real corporate, educational or personal data is used.

---

# Roadmap

- [ ] Generate synthetic datasets
- [ ] Build Bronze ingestion layer
- [ ] Create Silver transformations
- [ ] Create Gold business metrics
- [ ] Add data quality checks
- [ ] Add observability metrics
- [ ] Add dashboard layer
- [ ] Add Terraform infrastructure
- [ ] Add React front-end
- [ ] Add AI assistant integration

---

# Future Improvements

- Add Delta Live Tables
- Add CI/CD pipelines
- Add Unity Catalog concepts
- Add FastAPI services
- Add AI-powered analytics assistant
- Add semantic layer for BI tools

---

# Author

VK Schmitz

Focused on Data Literacy, AI Enablement, Analytics Engineering, corporate education and modern data platforms.
