# Notebook Structure

## Overview

The project follows a layered Analytics Engineering and Lakehouse approach using Databricks, PySpark and Medallion Architecture concepts.

The notebooks are organized by responsibility and analytical layer to simulate a modern educational analytics platform focused on gaming behavior, academic performance and learning analytics.

---

# Notebook Architecture

| Notebook | Responsibility |
|---|---|
| 02_bronze_gaming_academic_ingestion | Public Kaggle dataset ingestion and Bronze layer creation |
| 03_silver_gaming_academic_transformations | Data cleaning, standardization and feature engineering |
| 04_gold_gaming_academic_kpis | Business-ready KPIs and analytical aggregations |
| 05_quality_gaming_academic_checks | Data quality validation and governance rules |
| 06_dashboard_gaming_academic_views | Dashboard-oriented analytical views and reporting datasets |
| 07_semantic_metric_views | Semantic layer and reusable metric views for BI and AI |
| 08_observability_metrics | Pipeline observability, monitoring and operational metrics |
| 09_serving_sql_queries | SQL serving layer for dashboards, BI tools and analytical consumption |

---

# Medallion Flow

```txt
Raw Public Dataset
        ↓
Bronze Layer
        ↓
Silver Layer
        ↓
Gold KPIs
        ↓
Semantic Views
        ↓
Dashboards / SQL Serving / AI Consumption
