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

spark_structured_streaming_project/
- │
- ├── 01_Streaming_Simulator.ipynb
- ├── 02_Reading_Streams_With_Autoloader.ipynb
- ├── 03_Microbatch_Size.ipynb
- ├── 04_Schema_Inference_and_Evolution.ipynb
- ├── 05_Time_Based_Aggregations_and_Watermarking.ipynb
- ├── 06_Writing_Streams.ipynb
- ├── 07_Trigger_Intervals.ipynb
- ├── 08_Delta_Table_Streaming_Reads_and_Writes.ipynb
- └── README.md


