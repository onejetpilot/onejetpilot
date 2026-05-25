# Михаил Ражин

**Data Engineer**  
📍 Москва · 🟢 Open to work

Строю data pipelines и AI-сервисы: обработка данных, автоматизация, orchestration и production deployment.


### Контакты

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/mikhail-razhin)
[![Kaggle](https://img.shields.io/badge/Kaggle-20BEFF?style=flat-square&logo=kaggle&logoColor=white)](https://www.kaggle.com/mikhailrazhin)
[![Telegram](https://img.shields.io/badge/Telegram-26A5E4?style=flat-square&logo=telegram&logoColor=white)](https://t.me/RazhinMS)
[![CV](https://img.shields.io/badge/CV-PDF-red?style=flat-square&logo=adobeacrobatreader&logoColor=white)](https://github.com/onejetpilot/onejetpilot/blob/main/RMS_CV.pdf)



### Стек

![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-003B57?style=flat-square&logo=sqlite&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white)
![ClickHouse](https://img.shields.io/badge/ClickHouse-FFCC01?style=flat-square&logo=clickhouse&logoColor=black)
![Apache Kafka](https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white)
![Apache Spark](https://img.shields.io/badge/Spark-E25A1C?style=flat-square&logo=apachespark&logoColor=white)
![Airflow](https://img.shields.io/badge/Airflow-017CEE?style=flat-square&logo=apacheairflow&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![ChromaDB](https://img.shields.io/badge/ChromaDB-7B61FF?style=flat-square)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)


## Проекты

### Data Engineer Interview Bot с аналитическим event pipeline
https://github.com/onejetpilot/de-bot

> Telegram-бот для подготовки к DE-собеседованиям с отдельным аналитическим пайплайном событий

- **Пайплайн:**: сбор событий бота, запись raw events в PostgreSQL, инкрементальная загрузка в ClickHouse через Airflow DAG
- **Архитектура:** Telegram/API → PostgreSQL → Airflow ETL → ClickHouse, batch processing с watermark-контролем и защитой от повторной обработки
- **Хранилища:** SQLite для состояния бота и истории интервью, PostgreSQL для raw event storage, ClickHouse для аналитического слоя
- **Инфраструктура:** Docker Compose, PostgreSQL, ClickHouse, Airflow Webserver/Scheduler, FastAPI-сервис
- **Аналитика:** raw/enriched таблицы событий, подготовка данных для анализа активности пользователей, тем, качества ответов и времени реакции
- **Стек:** Python · SQL · PostgreSQL · ClickHouse · Apache Airflow · Docker Compose · FastAPI · SQLite

### Airflow ETL-пайплайн построения Sales DWH в PostgreSQL
https://github.com/onejetpilot/airflow-sales-dwh

> ETL-проект для генерации, загрузки и трансформации данных о продажах в PostgreSQL с оркестрацией через Apache Airflow

- **Пайплайн:** генерация raw-данных в CSV/JSON/XML, загрузка в staging-таблицы PostgreSQL, построение core-слоя и аналитических marts
- **Архитектура:** layered DWH pipeline (raw → staging → core → marts), orchestration через Airflow DAG, последовательные task dependencies и контроль max_active_runs
- **Инфраструктура:** PostgreSQL и Apache Airflow в Docker Compose, Airflow UI, подключение к БД через Airflow Connection, volume mounts для DAGs, SQL, scripts и data
- **Аналитика:** витрины mart_daily_sales, mart_customer_ltv, mart_product_performance, проверки качества данных и SQL-запросы с агрегациями, CTE и оконными функциями
- **Стек:** Python · Pandas · Apache Airflow · PostgreSQL · SQLAlchemy · Docker Compose · SQL

### ETL-пайплайн загрузки валютных курсов из API в PostgreSQL  
https://github.com/onejetpilot/api-to-postgres-etl

> ETL-проект для загрузки исторических валютных курсов из публичного REST API в PostgreSQL

- **Пайплайн:** extraction JSON-данных из внешнего API, очистка и нормализация данных через Pandas, загрузка в staging/core таблицы PostgreSQL  
- **Архитектура:** modular ETL pipeline (extract → transform → load), дедупликация данных, upsert через `ON CONFLICT DO UPDATE`  
- **Инфраструктура:** PostgreSQL в Docker Compose, локальный orchestration через Python entrypoint, конфигурация через environment variables  
- **Аналитика:** аналитические SQL-запросы с CTE, оконными функциями (`LAG`), агрегациями и расчетом дневной динамики валютных курсов  
- **Стек:** Python · Pandas · PostgreSQL · SQLAlchemy · Docker · SQL · REST API


### Yandex Practicum — Data Projects 
https://github.com/onejetpilot/data-science

> Портфолио учебных проектов по анализу и обработке данных

- **Data Processing:** SQL, pandas, data cleaning, exploratory data analysis  
- **Задачи:** аналитика данных, построение ETL-пайплайнов, обработка табличных данных, временные ряды  
- **Инструменты:** Python, PostgreSQL, pandas, Jupyter Notebook
