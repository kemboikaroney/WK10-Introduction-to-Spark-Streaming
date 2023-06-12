# WK10-Introduction-to-Spark-Streaming
Real-Time Network Traffic Analysis for Telecommunications

# Real-Time Network Traffic Analysis

This project implements a real-time network traffic analysis system using Spark Streaming, Kafka, and Streamlit. The system ingests network traffic data, performs real-time analytics, and provides interactive visualizations for monitoring traffic patterns and identifying anomalies.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)

## Introduction

The Real-Time Network Traffic Analysis project leverages the power of Apache Spark Streaming, Kafka, and Streamlit to process and visualize network traffic data in real-time. It enables network operation teams to monitor traffic patterns, detect anomalies, and gain insights into the overall network performance.

## Features

- Ingestion of network traffic data using Kafka producer
- Real-time analytics using Spark Streaming
- Sliding window operation to identify traffic patterns
- Window-based transformation to detect anomalies
- Visualization of processed data using Streamlit
- Continuous updates of the visualization as new data arrives

## Requirements

To run this project, you need the following:

- Python 3.x
- Apache Spark
- Confluent Cloud account and access credentials
- Streamlit

## Installation

1. Clone the repository:
2. Install the required dependencies:
3. Set up the Kafka cluster and topics on Confluent Cloud. Refer to the documentation for detailed instructions
4. Configure the connection details in the producer and processing/visualization code files:

   - `bootstrap_servers`: The bootstrap servers for your Kafka cluster
   - `sasl_username`: The SASL username for authentication
   - `sasl_password`: The SASL password for authentication
   - `kafka_topic`: The Kafka topic for network traffic data
   - `processed_topic`: The Kafka topic for processed data

## Usage

1. Run the producer script to generate and publish network traffic data to the Kafka topic:
2. Execute the Spark Streaming code to consume data from the Kafka topic, perform analytics, and publish the processed data to the processed data topic:
3. Launch the Streamlit application to visualize the processed data:
4. Access the Streamlit application in your web browser by following the provided URL.

## Results

The real-time network traffic analysis system provides interactive visualizations of network traffic patterns and anomalies. The Streamlit application displays a line graph that represents the processed data, with the x-axis representing the event time and the y-axis representing the total bytes sent within each window. The graph updates dynamically as new data arrives, allowing users to monitor traffic trends and detect any issues in real-time.

## Contributing

Contributions to this project are welcome. If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request. We appreciate your contributions.
