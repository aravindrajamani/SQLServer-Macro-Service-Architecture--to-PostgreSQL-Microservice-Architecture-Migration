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

https://viewer.diagrams.net/?tags=%7B%7D&lightbox=1&highlight=0000ff&edit=_blank&layers=1&nav=1&title=Untitled%20Diagram.drawio#R%3Cmxfile%3E%3Cdiagram%20name%3D%22Page-1%22%20id%3D%22OE4zK6PtYcE2mj9xmKT8%22%3E7Vlbc%2Bo2EP41zOQ8hLHxBXjklvbMJG06nJnTPmWELWy1skVlccuv78qWbGRDSBqT0OnhAUvr1XW%2Fb3cld5xJsvuJo1X8wEJMOz0r3HWcaafXsz2%2FDw8p2RcS1%2FULQcRJqJQqwZw8YyW0lHRNQpwZioIxKsjKFAYsTXEgDBninG1NtSWj5qgrFOGGYB4g2pR%2BJ6GIC%2BnAsyr5z5hEsR7ZttSbBGllJchiFLLtgciZdZwJZ0wUpWQ3wVRunt6Xot3dibflxDhOxWsabO3R5hfGwmg%2Fnv3KVmPKN3%2Ffql42iK7Vgjs9n0J%2F4wWHUiRLExiAIwqmCUF1%2Fts9%2FE%2BRQAuU4Y4ctN5gyaBojfLRJ5RA80wrhWSjtQ7b3dWFIDJU8w0Ue20VkuRmG6NsVRh9SXYwO2cci4RC1YbiihE5MOh74443ldqURCkIApgR5vlEU6EgZ4M9xqrbKUkimAAlC%2FhHz2uO5baGasmwljvYhCe9Bd1sE5Vz3GAu8O6khezS7kAYzBIs%2BB5UdAONHcUV21X1bYW8oRLFh6DTEEMK7FHZdYUHKChIvAEeTgMeI7kdCgDwuEOBYHKgOgaakpt5EOME3YLRciCpHkpFrfeNozQDCAGBCEsPAFFqfLk6PMi1PKm9aA8PTr%2BGB89u4mHQxIOWtQ4H97S30LaZ7cBXBIKk0THLlQ5BOhIwFVmSAN6hZAUv00UmHwUuagbGIXhlVWVcxCxiKaKzSjrmbJ2G0uZTC2qVzj1jK4WAP7EQe2VftBbMxIf0cvvfZfuuZfe14I9c4OnqdKcGKGr7w9oj5gT2WSIpFxaLkDN%2F2f6wULbmAT7vpgXiERbn%2BNrEE8cUyLQx59E6Oryms0hCFmRXx9bch5X%2B%2B%2BmRZSLiWPr0OebA2PYY7A9MBvebDt09QmDfvZCJ%2FIaJHjmjkoU%2FrHTgZ%2F1PNlO%2FYab7b18fSBoKjvEPQ5WG6rnDzzXU4HxAvGcoPB0NtYe0sjIaHkmowyJVAhMyqYphx5CQWVhYpuGfGC9vIWA6ZYRUAXPoXjJkviPEqaaPkhAVslx7cDzV0l0UIVq1Ojxl1Try%2B%2F2u07PKX8%2Fs1hpAcuENy59vjlIE%2BMYoI87R%2FkBNsfn1q3Gtc5N%2BSV9yPJ9BRZRy5%2F89d4bv5c5B6Pqv06dnm%2FTx7YtmnO3Tx%2FdNx2zVTqSvp4%2FfHQ57p%2BgzHHad11GmLZTqeygTpsaBpcDcx4vewhUjf3iZLVexvLOUbearH81Zq3ZG7AMHPveUqG5rzp4S%2B234gLfGJK%2Fvmi7CeTkmNfTVrcZFY5J97D60hrNsSxKKUgmoDLZa58yVLd%2BV4rqeseojN4Clbz3McJ2LXQHavat1gC15zgeWQiIh4twf3jyggBc%2Bh29IgLMvMkvnQUwEHK7yu89jDraGEbC%2FMF1H47glUUICREfqRULCsPBSOCPPaEE1qI4c3cAxZeqklqOQs7%2FwhFEmfUrKcmguCaU1UQvovNXfPRQ8Bw10lkA00HkxcDYvqD%2BYr37tzv4KCHv0lvYqeHdBUZ3TBFisKVxj8M3XjEGkyz9ClLfR%2BvpC8v1%2FTHDXM%2BNPk%2BCu3Q7BoVp9%2Byzid%2FUF2Zn9Aw%3D%3D%3C%2Fdiagram%3E%3C%2Fmxfile%3E




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

