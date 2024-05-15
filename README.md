# Diversity in Tech Pipeline

This project implements an ETL (Extract, Transform, Load) process for the Diversity in Tech Companies dataset. It is built using Apache Airflow for workflow management.

## Introduction

This project aims to demonstrate how to use Apache Airflow to automate the ETL process for the Diversity in Tech Companies dataset. It includes tasks for data extraction, cleaning, transformation, and loading.

## Getting Started

### Prerequisites

Make sure you have the following software installed:

- Python 3.x
- Apache Airflow
- pandas

### Installation

1. Clone this repository to your local machine:

    ```bash
    git clone https://github.com/yourusername/diversity-in-tech-pipeline.git
    ```

2. Install the required Python packages:

    ```bash
    pip install -r requirements.txt
    ```

### Usage

1. Start Apache Airflow:

    ```bash
    airflow webserver -p 8080
    airflow scheduler
    ```

2. Access the Airflow web interface at [http://localhost:8080](http://localhost:8080).
   
3. Navigate to the "diversity_in_tech_pipeline" DAG and trigger it to start the ETL process.

### DAG Configuration

- **DAG Name:** diversity_in_tech_pipeline
- **Description:** ETL process for Diversity in Tech Companies dataset
- **Schedule Interval:** Daily
- **Start Date:** January 1, 2024
- **Catchup:** False

### Task Details

- **Task ID:** etl_process
- **Python Callable:** etl_process function
- **Description:** Extracts data from the specified URL, cleans it, performs transformations, and prints the results.