# Streaming Data Pipeline for Toll Plaza Traffic Using Kafka and MariaDB

## Project Overview
This project involves building a real-time streaming data pipeline that simulates the collection of vehicle traffic data from toll plazas. The traffic data is generated using Python, streamed through **Apache Kafka**, and stored in a **MariaDB** database for further analysis. The system ensures data is processed efficiently and can be used for real-time decision-making in traffic monitoring and toll plaza management.

---

## Objective

1. **Simulate Traffic Data Generation**  
   - Randomly generate data to represent vehicles passing through various toll plazas.

2. **Stream the Generated Data**  
   - Use **Apache Kafka** for ingestion and streaming of the data to various consumers.

3. **Store the Processed Data**  
   - Store the data in a **MariaDB** database for structured query and reporting.

4. **Ensure Data Integrity**  
   - Implement verifications that ensure the pipeline runs smoothly with correct data being processed.

---

## Tools and Technologies

- **Apache Kafka**  
   A distributed streaming platform used to publish and subscribe to streams of records.

- **MariaDB**  
   A MySQL-compatible relational database used to store the processed traffic data.

- **Python**  
   Scripting language for creating the Kafka producer/consumer and data generation logic.

- **WSL (Windows Subsystem for Linux)**  
   Used for running the necessary database and Kafka environment on Windows.

- **Faker**  
   A library used to generate realistic but random traffic data.

  ## Setup

### Prerequisites
Ensure the following components are installed before proceeding:

1. **Install MariaDB**

   On **Ubuntu (WSL)**, run the following commands:

   ```bash
   sudo apt update
   sudo apt install mariadb-server



2.  **Download and Set Up Apache Kafka 3.9.0**


    Change to the `/tmp` directory to download the Kafka package:
  
    ```bash
    cd /tmp
    ```

    Download the Kafka binary for Scala 2.13:

    ```bash
    wget https://downloads.apache.org/kafka/3.9.0/kafka_2.13-3.9.0.tgz
    ```
    
    Extract the downloaded Kafka archive:
    
    ```bash
    tar -xvzf kafka_2.13-3.9.0.tgz
    ```
    This will create a directory named kafka_2.13-3.9.0.

3. **Move Kafka to the `/opt` Directory**
   
   Move the extracted Kafka directory to `/opt`:

    ```bash
    sudo mv kafka_2.13-3.9.0 /opt/
    ```
    I will change **kafka_2.13-3.9.0** to **kafka** using the following command
   ```bash
   mv /opt/kafka_2.13-3.9.0 /opt/kafka
   ```

5. **Verify Kafka Installation**

    List the files in the `/opt` directory to confirm Kafka has been moved successfully:

    ```bash
    ls /opt
    ```

   from the above image, it is clear that kafka_2.13-3.9.0 successfully downloaded 



    


    



