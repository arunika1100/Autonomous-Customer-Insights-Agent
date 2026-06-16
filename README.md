# Autonomous AI Data Analytics Agent
An AI-powered customer insights agent built using Botpress, Generative AI, and analytics workflows. It analyzes customer behavior, feedback, engagement metrics, and business data to generate actionable insights and support data-driven decision making.

## 🚀 What Makes This Project Unique (Value Proposition)
Unlike traditional static chatbots or basic hardcoded decision trees, this system utilizes a fully autonomous execution loop driven by an LLM core:
*   **Dynamic Schema Contextualization**: The agent self-evaluates incoming data schemas via live data tables without hardcoded configurations.
*   **Closed-Loop Execution**: Implements structural error recovery to ensure generated programmatic data pipelines are flawless before outputting.
*   **Dual-Layer Capability**: Seamlessly switches between generating advanced database manipulation frameworks (SQL) and local analytical transformation scripts (Python/Pandas).

---

## 🏗️ Technical Architecture & Workflow Loop

1.  **Ingestion & Permission Syncing**: Live datasets are mounted to native relational data tables with granular role-based permissions (Create, Read, Update, Delete operations enabled).
2.  **Autonomous Analysis Core**: An advanced LLM processing node evaluates user requests against the underlying data catalog.
3.  **Tool Belt Routing**: The agent dynamically orchestrates execution calls between:
    *   *Data Engineering Tools*: Executing record filtering, deduplication algorithms, and type-casting scripts.
    *   *Visualization Nodes*: Mapping complex multi-variate trends to dynamic UI charts (Scatter Plots, Bar Charts, and Trend Lines).
4.  **Exit Optimization**: Conditional exit logic validates user satisfaction or program delivery, preventing costly infinite looping cycles.

---

## 📊 Live System Case Study: Customer Insights Processing

### The Problem:
Ingesting a raw customer dataset containing critical inconsistencies: duplicate identifiers (`user_id`), unformatted country codes (`usa`, `india`), and unpopulated temporal fields (`signup_date`).

### The Autonomous Action & Resolution:
When queried in plain language to audit the system, the agent successfully executed a schema lookup, targeted specific operational gaps, and instantly delivered structured, localized analytics along with clean execution blocks:

```python
# Generated Autonomously by the AI Data Agent to handle empty signup_dates
import pandas as pd

# Pipeline step: Purge broken temporal links
df_cleaned = df.dropna(subset=['signup_date'])
