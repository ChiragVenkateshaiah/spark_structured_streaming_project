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
├── 01_Streaming_Simulator.ipynb
│   # Generates random weather data and simulates a streaming source.
│
├── 02_Reading_Streams_With_Autoloader.ipynb
│   # Reads streaming data using Databricks Auto Loader.
│
├── 03_Microbatch_Size.ipynb
│   # Demonstrates micro-batch configuration in Structured Streaming.
│
├── 04_Schema_Inference_and_Evolution.ipynb
│   # Handles schema inference and evolution in streaming pipelines.
│
├── 05_Time_Based_Aggregations_and_Watermarking.ipynb
│   # Performs window aggregations and applies watermarking.
│
├── 06_Writing_Streams.ipynb
│   # Writes streaming data to Delta and other sinks.
│
├── 07_Trigger_Intervals.ipynb
│   # Shows different trigger interval configurations for streaming queries.
│
├── 08_Delta_Table_Streaming_Reads_and_Writes.ipynb
│   # Reads and writes Delta tables using Structured Streaming.
│
├── README.md
│   # Project documentation.
│
└── (additional folders such as configs/, data/, or src/ can be added as the project expands)

