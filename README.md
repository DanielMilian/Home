# Hi, I'm Daniel Milián

**Business engineer building data products**, from raw source to the decision it informs.

Barcelona · [LinkedIn](https://www.linkedin.com/in/daniel-milian-30865a29/) · danielmilian@outlook.com

## Projects

### 🏠 Barcelona Housing Affordability (2015–2023)
End-to-end pipeline answering one question: how affordable is renting in each of Barcelona's 10 districts, and how has that changed? Public INE and Housing Ministry data flows through Airflow and dbt into Postgres, then is served by a FastAPI API and a Streamlit dashboard.
- **Stack:** Python, Airflow, dbt, PostgreSQL, FastAPI, Streamlit, Docker Compose
- 55 dbt nodes with tests passing, idempotent DAG reruns, API-key auth, rate limiting and a CSV fallback for the dashboard
- [Live dashboard](https://barcelona-housing-2015-2023.streamlit.app/) · [Repo](https://github.com/DanielMilian/barcelona-housing)

### 🚲 Barcelona Bicing Analytics
Event-streaming pipeline over Barcelona's public bike-sharing API, with a deployed analytics dashboard.
- **Stack:** Python, Kafka, PostgreSQL, dbt, Supabase, Streamlit, Docker
- Kafka producer/consumer with duplicate protection and manual offset commits; dbt staging → intermediate → marts with data quality tests
- [Live dashboard](https://barcelona-bicinganalytics.streamlit.app/) · [Repo](https://github.com/DanielMilian/Bicing_Analytics)

### 🛒 E-commerce Revenue & Inventory Pipeline
Airflow pipeline (extract → transform → load → validate) over the DummyJSON API, modeled as a star schema in Postgres, with a Streamlit dashboard on revenue concentration and stock-out risk.
- **Stack:** Python, Airflow, PostgreSQL, Streamlit, Docker Compose
- Validation reconciles warehouse revenue against the raw source; it caught a silent ~9,500 revenue undercount from dropped duplicate lines
- [Repo](https://github.com/DanielMilian/dummyjson-pipeline)

### 📈 Demand Forecasting with LSTM
Pooled multi-series LSTM (PyTorch, store/SKU embeddings) forecasting weekly demand across 1,155 series.
- Beats a naive baseline: **MAE 16.85 vs 18.89**, RMSE 38.50 vs 40.27
- Documents the dataset switch after EDA and the negative results (single-series overfitting, dropout experiment)
- [Repo](https://github.com/DanielMilian/DemandForecastingLSTM)

## Skills

| | |
|---|---|
| **Languages** | Python, SQL, Bash |
| **Data engineering** | Airflow, dbt, Kafka, PostgreSQL, Docker, pandas, FastAPI |
| **ML & AI** | PyTorch, scikit-learn, LangGraph |
| **Cloud & tools** | Oracle Cloud (OCI), Supabase, Streamlit, Git/GitHub, Linux |
| **Analytics & BI** | Tableau, Plotly, Excel, Streamlit |

## Certifications
- Oracle Cloud Infrastructure 2025 Certified Data Science Professional
- Docker Foundations Professional Certificate
- Databricks Fundamentals and Generative AI Fundamentals
