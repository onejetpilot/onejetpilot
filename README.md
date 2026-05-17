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

### ETL-пайплайн загрузки валютных курсов из API в PostgreSQL  
https://github.com/onejetpilot/api-to-postgres-etl

> ETL-проект для загрузки исторических валютных курсов из публичного REST API в PostgreSQL

- **Data Pipeline:** extraction JSON-данных из внешнего API, очистка и нормализация данных через Pandas, загрузка в staging/core таблицы PostgreSQL  
- **Архитектура:** modular ETL pipeline (extract → transform → load), дедупликация данных, upsert через `ON CONFLICT DO UPDATE`  
- **Infrastructure:** PostgreSQL в Docker Compose, локальный orchestration через Python entrypoint, конфигурация через environment variables  
- **Analytics:** аналитические SQL-запросы с CTE, оконными функциями (`LAG`), агрегациями и расчетом дневной динамики валютных курсов  
- **Стек:** Python · Pandas · PostgreSQL · SQLAlchemy · Docker · SQL · REST API

### Telegram-бот для подготовки к собеседованиям по Data Engineering  
https://github.com/onejetpilot/de-bot

> Telegram-бот для тренировки собеседований по Data Engineering и проверки ответов пользователей

- **Data Pipeline:** обработка базы вопросов, хранение результатов интервью и истории пользователей  
- **Архитектура:** stateful interview flow, случайная выборка вопросов, автоматический feedback по ответам  
- **Infrastructure:** Telegram Bot API integration, Docker deployment, конфигурация через environment variables  
- **LLM Integration:** анализ ответов и формирование рекомендаций через OpenRouter API  
- **Стек:** Python · aiogram · PostgreSQL · OpenRouter · Docker · Linux

### AI-консультант по инженерной сантехнике на базе RAG
https://github.com/AI-agent-team-2/data-science-

> AI/RAG сервис для консультации пользователей по товарному каталогу (инженерная сантехника)

- **Data Pipeline:** ingestion TXT-документов, chunking, embeddings pipeline, retrieval через ChromaDB  
- **Архитектура:** deterministic routing (RAG → product lookup → web fallback), модульные инструменты (rag_search, product_lookup, web_search)  
- **Infrastructure:** Docker, systemd, VPS deployment, GitHub Actions CI/CD, Telegram Bot API integration  
- **Observability:** Langfuse tracing, structured logging, мониторинг вызовов LLM и tool pipeline  
- **Стек:** Python · PostgreSQL · ChromaDB · LangChain · OpenRouter · aiogram · Docker · Linux


### Yandex Practicum — Data Projects 
https://github.com/onejetpilot/data-science

> Портфолио учебных проектов по анализу и обработке данных

- **Data Processing:** SQL, pandas, data cleaning, exploratory data analysis  
- **Задачи:** аналитика данных, построение ETL-пайплайнов, обработка табличных данных, временные ряды  
- **Инструменты:** Python, PostgreSQL, pandas, Jupyter Notebook
