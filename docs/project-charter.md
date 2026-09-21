# Project Charter — Big Data Platform

**Project Title:** Mise en place d’une solution Big Data  
**Duration:** 2 months

## 1. Project Objective

The objective of this project is to **migrate data from an existing Data Warehouse (DWH) to a modern Big Data platform**. The solution will provide a scalable architecture for storing, managing, and processing analytical data using distributed data-processing technologies and an open table format.

## 2. Technology Stack

The proposed Big Data platform will be built using:

- **Apache Spark** — distributed data processing, transformation, and analysis.
- **Apache Iceberg** — table format for managing large analytical datasets with reliable data operations.
- **Garage** — S3-compatible object storage for storing the project's data.
- **Polaris** — catalog service for managing and discovering Iceberg tables.
- **Python and Java** — development and data-processing languages, as required by the project prerequisites.

The development environment will use **Docker** where appropriate to simplify the deployment and reproducibility of the platform components.

## 3. Dataset Target

The target data consists of data currently stored in the **existing Data Warehouse (DWH)**. The selected DWH dataset/domain and its relevant source tables will be identified during the initial data-analysis phase and subsequently migrated to the Big Data platform.

The migration will preserve the relevant data structure and content required for analytical processing.

## 4. Project Scope

The project will include:

1. Setting up the Big Data platform infrastructure.
2. Configuring Garage as the object-storage layer.
3. Configuring Polaris as the Iceberg catalog.
4. Integrating Apache Spark with Garage, Iceberg, and Polaris.
5. Migrating the selected DWH dataset to Iceberg tables.
6. Implementing data transformation and processing operations.
7. Validating the migrated data and the functioning of the complete platform.

## 5. Success Criteria

The project will be considered successfully implemented when:

- The Big Data platform components are correctly configured and operational.
- Spark can successfully read from and write to Iceberg tables.
- Iceberg tables are stored in Garage and registered through Polaris.
- The selected DWH dataset is successfully migrated.
- The migrated data can be queried and processed through Spark.
- Data validation confirms that the migration preserves the required data.
- The complete workflow can be reproduced from the project configuration and documentation.
- The architecture, configuration, and migration process are properly documented.
