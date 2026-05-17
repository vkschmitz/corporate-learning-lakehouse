# Architecture Overview

## Project Goal

This project simulates a modern corporate learning and AI enablement platform using Analytics Engineering concepts, Databricks and Medallion Architecture.

The goal is to transform raw learning activity data into business-ready analytics for Data Literacy and AI Enablement initiatives.

---

# High-Level Architecture

```txt
Users / Learning Platforms
            ↓
        Bronze Layer
            ↓
        Silver Layer
            ↓
         Gold Layer
            ↓
 Dashboards / AI / BI
```

---

# Data Flow

## Source Layer

Synthetic educational datasets simulate:

- users
- courses
- enrollments
- learning events
- feedback
- AI adoption interactions

---

# Bronze Layer

Raw ingestion layer.

Characteristics:
- append-only
- source-aligned
- minimal transformations
- ingestion metadata included

Examples:
- users_raw
- courses_raw
- enrollments_raw
- learning_events_raw

---

# Silver Layer

Cleaned and standardized data.

Characteristics:
- deduplication
- schema standardization
- data quality validations
- normalized formats

Examples:
- users
- courses
- enrollments
- learning_events

---

# Gold Layer

Business-ready analytical layer.

Characteristics:
- aggregated KPIs
- persona analytics
- engagement metrics
- learning funnels
- AI Enablement indicators

Examples:
- learning_adoption_by_persona
- course_completion_rate
- monthly_learning_engagement
- ai_enablement_kpis

---

# Technologies

## Data Platform
- Databricks
- Delta Lake
- PySpark
- SQL

## Engineering
- GitHub
- WSL2
- Linux
- VS Code

## Future Roadmap
- Azure
- Terraform
- React Front-end
- Power BI
- Databricks Genie
- Azure OpenAI

---

# Governance Concepts

The project applies foundational governance concepts such as:

- schema organization
- layer separation
- naming conventions
- synthetic data strategy
- quality validation
- business metric ownership

---

# Future Evolution

## Planned Improvements

- Delta Live Tables
- CI/CD pipelines
- observability metrics
- semantic layer
- metadata documentation
- AI-powered analytics assistant
- front-end learning portal
