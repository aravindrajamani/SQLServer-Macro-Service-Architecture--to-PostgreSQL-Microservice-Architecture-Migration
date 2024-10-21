# SQLServer-Macro-Service-Architecture--to-PostgreSQL-Microservice-Architecture-Migration
This project demonstrates the migration of an e-learning platform from a monolithic (macro services) architecture to microservices, using SQL Server to PostgreSQL migration via Azure Data Factory.

## Project Overview

- **Platform:** E-learning 
- **Architecture:** Migrated from macro services (shared database) to microservices (individual databases for each client)
- **Database:** Migrated from SQL Server to PostgreSQL
- **Tools:** Azure Data Factory (ADF), SQL Server, PostgreSQL
- **Total Clients:** 456
- **Focus:** Data isolation, scalability, minimal downtime

## Architectural Diagram




## Responsibilities

- Designed and implemented separate databases for each client in the new microservices architecture.
- Migrated data for 456 clients from SQL Server to PostgreSQL using ADF.
- Configured and optimized ADF pipelines to efficiently handle large-scale data transfer.
- Developed error-handling and validation processes to ensure accurate data migration.
- Ensured data integrity, security compliance, and minimal downtime during the migration process.

## Key Features

1. **Azure Data Factory Pipelines**:
   - Handled large-scale data transfer between SQL Server and PostgreSQL.
   - Included error handling and validation for data accuracy.
   - Optimized for performance and scalability.

2. **Microservices Architecture**:
   - Each client has its own isolated database.
   - Ensured scalability and easy maintenance.

3. **PostgreSQL Optimization**:
   - Worked with DBAs to configure PostgreSQL for each client environment.
   - Focused on security and performance tuning.

## How It Works

### 1. Macro to Microservices Migration
- **Old Model:** All clients shared a single database.
- **New Model:** Each client now has their own PostgreSQL database in the microservices architecture.

### 2. Data Migration
- **SQL Server** → **PostgreSQL** using **ADF** pipelines.
- Data was transferred in phases to minimize downtime.
- Validation checks were run post-migration to ensure data integrity.

## Repository Structure

```plaintext
├── azure-data-factory-pipelines/
│   └── adf_pipeline_config.json   # JSON config files for ADF pipelines
└── README.md                      # Project documentation

