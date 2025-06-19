# 📊 Meteorological Data Analysis in Morocco with Big Data Tools

This project focuses on extracting, processing, and visualizing meteorological data from six major Moroccan cities using a Big Data architecture. We combine **web scraping**, **distributed storage**, **parallel data processing**, and a simple **web interface** to demonstrate the power of end-to-end data engineering and analysis workflows.

---

## 📌 Project Overview

- 🔍 **Data Extraction**: Scraping weather data from online sources using `BeautifulSoup`.
- 🗂 **Storage**: Storing the collected data in a **Hadoop Distributed File System (HDFS)**.
- ⚙️ **Processing**: Transforming and analyzing the data using **Apache Spark**.
- 🌐 **Visualization**: Creating a simple and interactive web dashboard using **Flask**.

---

## 🏙️ Target Cities

The analysis includes meteorological data from the following Moroccan cities:
- Casablanca
- Laâyoune
- Ifrane
- Ouarzazate
- Tétouan

## 🛠️ Technologies Used

| Component         | Tool/Library              |
|------------------|---------------------------|
| Web Scraping     | BeautifulSoup (Python)    |
| Storage          | Hadoop HDFS               |
| Processing       | Apache Spark (PySpark)    |
| Backend / API    | Flask                     |
| Language         | Python                    |
| Deployment (opt) | Docker / VirtualBox       |

---

## 🧱 Architecture

```text
            ┌────────────────────┐
            │  BeautifulSoup     │
            │  (Scraping Data)   │
            └────────┬───────────┘
                     ↓
           ┌──────────────────────┐
           │  Hadoop HDFS         │
           │  (Data Lake Storage) │
           └────────┬─────────────┘
                    ↓
           ┌──────────────────────┐
           │  Apache Spark        │
           │  (Data Processing)   │
           └────────┬─────────────┘
                    ↓
           ┌──────────────────────┐
           │  Flask API           │
           │  (Web Dashboard)     │
           └──────────────────────┘
