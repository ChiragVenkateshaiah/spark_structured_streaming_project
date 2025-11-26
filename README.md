# spark_structured_streaming_project


# Project Summary:
This project demonstrates real-time data engineering using Spark Structured Streaming by generating random weather data, ingesting it as a continuous stream, transforming it using Spark’s near–real-time processing engine, and writing the processed output into Delta Lake storage. The pipeline follows an incremental processing model with exactly-once guarantees, using cloud-friendly file streams as the source and Delta Lake as the sink. This project highlights key concepts like streaming reads/writes, checkpointing, schema enforcement, and fault-tolerant stream processing.

- **Fault tolerance**  
- **End-to-end recovery**  
- **Exactly-once processing guarantees**


## 🎯 Key Features

- Generate **continuous random weather data**
- Read streaming data using **Spark Structured Streaming**
- Apply streaming transformations (cleaning, parsing, enrichment)
- Write processed data to:
  - **Delta Lake tables**
  - Cloud/Object storage (optional)
- Uses **checkpointing** for fault tolerance and recovery
- Supports **auto schema handling** and incremental processing


## 📚 Architecture

**Data Source → Spark Structured Streaming → Transformations → Delta Sink**

- **Source:** Random weather data generator (simulates IoT/sensor feeds)  
- **Engine:** Spark Structured Streaming incremental execution model  
- **Sink:** Delta Lake table with ACID transactions

🛠️ Technologies Used

- Databricks / Apache Spark
- Spark Structured Streaming
- Delta Lake
- Python / PySpark

## Project Structure
spark_structured_streaming_project/
│
├── (root)/
│   ├── README.md                   # Project documentation (this file)
│   ├── (notebooks and/or streaming scripts)  # your stream-simulator & processing notebooks / scripts
│
├── 01 Streaming Simulator Notebook # notebook simulating random weather data generation :contentReference[oaicite:2]{index=2}
├── 02 Reading Streams with Auto Loader # notebook for reading streams using Auto Loader :contentReference[oaicite:3]{index=3}
├── 03 Micro-batch Size             # notebook focusing on micro-batch config for streaming :contentReference[oaicite:4]{index=4}
├── 04 Schema Inference and Evolution # notebook about handling schema changes in streaming data :contentReference[oaicite:5]{index=5}
├── 05 Time Based Aggregations and Watermarking # notebook for time-window based aggregations & watermarking :contentReference[oaicite:6]{index=6}
├── 06 Writing Streams              # notebook demonstrating writing streams out (e.g. to files / Delta) :contentReference[oaicite:7]{index=7}
├── 07 Trigger Intervals            # notebook showing how to configure trigger intervals for streaming :contentReference[oaicite:8]{index=8}
├── 08 Delta Table Streaming Reads and Writes # notebook covering streaming-read/write with Delta Lake sink/source :contentReference[oaicite:10]{index=10}

