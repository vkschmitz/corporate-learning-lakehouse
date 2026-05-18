# SQL Serving Queries Documentation

## Purpose

The SQL serving layer provides reusable analytical SQL queries optimized for dashboards, BI tools, ad-hoc analytics and AI-assisted consumption.

In this project, the SQL layer enables structured analytical exploration of gaming behavior, academic performance, study habits and educational KPIs.

---

# Notebook

```txt
09_serving_sql_queries
```

---

# Source Tables

```txt
learning_analytics.gold_grades_by_genre
learning_analytics.gold_sleep_performance
learning_analytics.gold_behavior_segments
learning_analytics.gold_performance_levels
learning_analytics.quality_gaming_academic_checks
```

---

# SQL Layer Goals

The SQL serving layer is responsible for:

- enabling reusable analytical queries
- simplifying dashboard integration
- supporting BI consumption
- preparing AI-readable query structures
- enabling executive analytics
- supporting ad-hoc analysis

---

# Planned SQL Queries

## Academic Performance Queries

| Query | Purpose |
|---|---|
| avg_grades_by_genre | Analyze grades by gaming genre |
| top_performance_profiles | Identify high-performing profiles |
| grade_distribution | Analyze academic performance distribution |

---

## Behavioral Queries

| Query | Purpose |
|---|---|
| study_vs_gaming_balance | Compare study and gaming behavior |
| behavioral_segmentation | Analyze behavioral profiles |
| gaming_hours_distribution | Understand gaming time distribution |

---

## Wellness Queries

| Query | Purpose |
|---|---|
| sleep_vs_performance | Analyze sleep impact on grades |
| stress_vs_grades | Correlate stress and academic outcomes |
| social_activity_analysis | Analyze social behavior metrics |

---

# Example SQL Queries

## Average Grades by Gaming Genre

```sql
SELECT
    gaming_genre,
    ROUND(AVG(grades), 2) AS avg_grades,
    ROUND(AVG(gaming_hours), 2) AS avg_gaming_hours,
    ROUND(AVG(study_hours), 2) AS avg_study_hours,
    COUNT(*) AS student_count
FROM learning_analytics.silver_gaming_academic_clean
GROUP BY gaming_genre
ORDER BY avg_grades DESC;
```

---

## Sleep vs Academic Performance

```sql
SELECT
    stress_level,
    ROUND(AVG(sleep_hours), 2) AS avg_sleep_hours,
    ROUND(AVG(grades), 2) AS avg_grades
FROM learning_analytics.silver_gaming_academic_clean
GROUP BY stress_level
ORDER BY avg_grades DESC;
```

---

## Behavioral Segmentation

```sql
SELECT
    CASE
        WHEN gaming_hours >= 6 AND study_hours <= 3 THEN 'High Gaming / Low Study'
        WHEN gaming_hours <= 2 AND study_hours >= 6 THEN 'Low Gaming / High Study'
        ELSE 'Balanced'
    END AS behavior_profile,
    COUNT(*) AS student_count,
    ROUND(AVG(grades), 2) AS avg_grades
FROM learning_analytics.silver_gaming_academic_clean
GROUP BY behavior_profile
ORDER BY avg_grades DESC;
```

---

# SQL Serving Architecture

```txt
Bronze Layer
    ↓
Silver Layer
    ↓
Gold KPIs
    ↓
Semantic Views
    ↓
SQL Serving Layer
    ↓
Dashboards / BI / AI
```

---

# SQL Consumers

The SQL layer supports:

- Databricks SQL
- Power BI
- dashboards
- ad-hoc analytics
- semantic views
- Databricks Genie
- AI copilots
- executive reporting

---

# SQL Design Principles

The SQL serving layer follows:

- reusable queries
- business-readable logic
- semantic consistency
- dashboard optimization
- AI-readable query structures
- centralized analytical logic

---

# Analytics Engineering Concepts Applied

This layer demonstrates:

- serving layer modeling
- analytical SQL optimization
- reusable business queries
- semantic query design
- dashboard-oriented SQL
- AI-ready analytical structures
- centralized query governance

---

# Related Notebooks

| Notebook | Responsibility |
|---|---|
| 03_silver_gaming_academic_transformations | Cleaned analytical datasets |
| 04_gold_gaming_academic_kpis | KPI generation |
| 05_quality_gaming_academic_checks | Quality validation |
| 06_dashboard_gaming_academic_views | Dashboard layer |
| 07_semantic_metric_views | Semantic metric abstraction |
| 09_serving_sql_queries | SQL analytical serving |

---

# Future Improvements

Planned future enhancements include:

- parameterized SQL queries
- SQL performance optimization
- AI-generated SQL
- query lineage tracking
- dashboard query acceleration
- semantic SQL generation
- advanced analytical views
- conversational SQL analytics

---

# Future AI Integration

The SQL serving layer prepares the platform for:

- Databricks Genie
- natural language querying
- AI-generated analytical SQL
- conversational BI
- semantic query generation
- AI-assisted analytics exploration

---

# Design Rationale

The SQL serving layer separates analytical consumption logic from transformation pipelines.

This improves:

- dashboard maintainability
- BI integration
- analytical consistency
- semantic readability
- AI-readiness
- query governance
- scalability

---

# Governance Perspective

The SQL layer helps ensure:

```txt
business users consume standardized and governed analytical logic
```
