# Bronze Gaming Academic Ingestion

## Purpose

This notebook creates the Bronze ingestion layer for the Gaming Academic Performance Lakehouse project.

The notebook ingests a public Kaggle educational dataset stored in GitHub and prepares the raw analytical foundation for the Medallion Architecture pipeline.

---

# Business Context

The project simulates a modern Learning Analytics and Analytics Engineering environment focused on:

- gaming behavior
- academic performance
- student engagement
- educational analytics
- behavioral segmentation
- AI-assisted analytics exploration

The Bronze layer preserves the original dataset structure while adding ingestion and governance metadata.

---

# Source Dataset

## Public Dataset

Gaming vs Academic Performance

Source:
- Kaggle

Dataset URL:
- https://www.kaggle.com/datasets/aiexplorer77/gaming-vs-academic-performance

GitHub Raw File:
- Gaming_Academic_Performance.csv

Repository:
- corporate-learning-lakehouse

---

# Source Layer

The dataset is ingested directly from GitHub using pandas and converted into Spark DataFrames.

Main ingestion flow:

```txt
GitHub Raw CSV
        ↓
pandas DataFrame
        ↓
Spark DataFrame
        ↓
Bronze Layer
```

---

# Technologies Used

## Data Platform
- Databricks
- Spark
- PySpark

## Engineering
- GitHub
- VS Code
- Python

## Analytics
- Learning Analytics
- Medallion Architecture
- Behavioral Analytics

---

# Bronze Layer Characteristics

The Bronze layer follows Medallion Architecture principles:

- raw ingestion
- append-oriented structure
- minimal transformations
- source-aligned schema
- ingestion metadata included

---

# Ingestion Metadata

The notebook adds operational metadata fields such as:

- _ingestion_timestamp
- _source_system
- _source_url
- _dataset_name
- _pipeline_layer

These fields support:

- governance
- observability
- lineage
- traceability
- operational monitoring

---

# Main Columns

The ingested dataset contains educational and behavioral metrics such as:

- student_id
- age
- gender
- gaming_hours
- study_hours
- sleep_hours
- attendance
- gaming_genre
- social_activity
- addiction_score
- stress_level
- grades

---

# Output Schema

Schema:
- learning_analytics

---

# Output Table

Bronze Table:

```txt
learning_analytics.bronze_gaming_academic_performance
```

---

# Observability Support

The Bronze layer is integrated with future monitoring and observability notebooks.

The table supports:

- row count monitoring
- freshness validation
- pipeline health checks
- operational dashboards

---

# Future Pipeline Flow

```txt
Bronze Layer
        ↓
Silver Transformations
        ↓
Gold KPIs
        ↓
Dashboard Layer
        ↓
Semantic Views
        ↓
Genie AI
```

---

# Business Value

This notebook demonstrates foundational Analytics Engineering practices including:

- raw ingestion
- Spark processing
- governance metadata
- GitHub integration
- semantic organization
- enterprise-oriented data architecture

The Bronze layer serves as the operational foundation for the entire Learning Analytics platform.
