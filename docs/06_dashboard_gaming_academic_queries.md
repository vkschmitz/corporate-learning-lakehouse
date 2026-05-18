# Dashboard Views Documentation

## Purpose

The dashboard layer provides business-ready analytical views optimized for dashboards, executive reporting and visual analytical consumption.

In this project, the dashboard layer organizes educational and behavioral KPIs related to gaming habits, academic performance, study behavior and student engagement.

---

# Source Tables

```txt
learning_analytics.gold_grades_by_genre
learning_analytics.gold_sleep_performance
learning_analytics.gold_behavior_segments
learning_analytics.gold_performance_levels
```

---

# Notebook

```txt
06_dashboard_gaming_academic_views
```

---

# Dashboard Layer Goals

The dashboard layer is responsible for:

- preparing visual analytical datasets
- simplifying dashboard consumption
- supporting executive analytics
- enabling reusable visual metrics
- optimizing BI queries
- supporting AI-assisted visual analytics

---

# Planned Dashboards

| Dashboard | Description |
|---|---|
| Academic Performance Overview | General educational performance indicators |
| Gaming Behavior Dashboard | Gaming patterns and behavioral metrics |
| Sleep & Performance Analytics | Relationship between sleep and grades |
| Behavioral Segmentation Dashboard | Student profile segmentation |
| Study vs Gaming Dashboard | Balance between gaming and study habits |

---

# Dashboard KPIs

## Academic KPIs

- average grades
- performance distribution
- performance level segmentation
- attendance averages

---

## Behavioral KPIs

- average gaming hours
- study-to-gaming ratio
- gaming genre distribution
- addiction score analysis

---

## Wellness KPIs

- average sleep hours
- stress level distribution
- social activity analysis
- device usage patterns

---

# Dashboard Views

## vw_dashboard_academic_performance

Aggregated educational metrics for executive consumption.

### Metrics

- avg_grades
- avg_study_hours
- avg_attendance
- student_count

---

## vw_dashboard_gaming_behavior

Behavioral gaming metrics.

### Metrics

- avg_gaming_hours
- gaming_genre_distribution
- addiction_score
- device_usage

---

## vw_dashboard_sleep_analytics

Sleep and wellness metrics.

### Metrics

- avg_sleep_hours
- stress_level_distribution
- sleep_vs_grades
- wellness indicators

---

## vw_dashboard_behavior_segments

Student behavioral segmentation.

### Segments

- High Gaming / Low Study
- Low Gaming / High Study
- Balanced

---

# Dashboard Architecture

```txt
Bronze Layer
    ↓
Silver Layer
    ↓
Gold KPIs
    ↓
Dashboard Views
    ↓
Dashboards / BI / AI Consumption
```

---

# Dashboard Consumers

The dashboard layer supports:

- Databricks dashboards
- Power BI
- SQL analytics
- executive reporting
- semantic views
- Databricks Genie
- AI copilots

---

# Dashboard Design Principles

The dashboard layer follows:

- simplified consumption
- business-oriented metrics
- reusable analytical structures
- visual performance optimization
- semantic consistency
- AI-ready analytics

---

# Analytics Engineering Concepts Applied

This layer demonstrates:

- dashboard serving layers
- analytical modeling
- KPI abstraction
- reusable visual datasets
- dimensional thinking
- business analytics optimization
- semantic consumption structures

---

# Related Notebooks

| Notebook | Responsibility |
|---|---|
| 02_bronze_gaming_academic_ingestion | Raw ingestion |
| 03_silver_gaming_academic_transformations | Cleaning and transformations |
| 04_gold_gaming_academic_kpis | KPI generation |
| 05_quality_gaming_academic_checks | Data quality validation |
| 06_dashboard_gaming_academic_views | Dashboard serving layer |
| 07_semantic_metric_views | Semantic metrics |

---

# Future Improvements

Planned future enhancements include:

- interactive dashboards
- real-time monitoring
- AI-powered dashboards
- predictive educational analytics
- anomaly visualization
- advanced segmentation dashboards
- executive scorecards
- semantic dashboard layers

---

# Design Rationale

The dashboard layer separates analytical consumption from transformation logic.

This improves:

- dashboard maintainability
- BI performance
- metric standardization
- semantic consistency
- AI-readiness
- visual scalability

---

# Future AI Integration

The dashboard layer is designed to support:

- conversational BI
- Databricks Genie
- AI copilots
- semantic analytics
- natural language dashboard exploration
- educational insight generation

---

# Visualization Strategy

The project prepares future integrations with:

- Databricks Dashboards
- Power BI
- React front-end dashboards
- embedded analytics
- AI-assisted visualization layers
