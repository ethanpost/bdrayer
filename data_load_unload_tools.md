## Data Load/Unload Tools Overview

### Oracle Tools
- Data Pump Export (expdp)
  - Exports to proprietary binary dump files
  - High-performance for large datasets
  - Supports parallel processing
  - Outputs .dmp files
- Data Pump Import (impdp)
  - Imports from .dmp files
  - Supports schema/database remapping
  - Parallel import capability
- SQL*Loader
  - Loads data from flat files
  - Requires control file (.ctl)
  - High-speed bulk loading
  - Error logging for bad records
- UTL_FILE Package
  - Programmatic file access
  - Requires directory objects
  - Flexible but slower than SQL*Loader
- External Tables
  - Maps flat files to virtual tables
  - Useful for ETL processes
  - No physical data movement for querying

### SQL Server Tools
- BCP (Bulk Copy Program)
  - High-performance bulk operations
  - Command-line tool
  - Supports format files
- SSIS (SQL Server Integration Services)
  - GUI-based ETL tool
  - Advanced transformations
  - Complex workflow support
- Import/Export Wizard
  - User-friendly GUI
  - Built into SSMS
  - Limited scalability
- OPENROWSET/BULK INSERT
  - T-SQL based loading
  - High-speed operations
  - Requires format files

### PostgreSQL Tools
- COPY
  - Fast and efficient
  - Built into PostgreSQL
  - Supports CSV, text, binary
- \copy (psql)
  - Client-side version of COPY
  - Runs on client machine
  - Same syntax as COPY
- pg_dump
  - Exports to SQL scripts
  - Supports compression
  - Primarily for backups
- pg_restore
  - Restores from pg_dump archives
  - Supports parallel restore
  - Used for migrations

### MySQL Tools
- mysqldump
  - Exports to SQL scripts
  - Supports compression
  - Can include data or schema only
- SELECT ... INTO OUTFILE
  - Exports query results
  - File created on server
  - Requires FILE privilege
- LOAD DATA INFILE
  - High-speed bulk loading
  - Configurable options
  - Error handling support
- mysqlimport
  - Command-line import tool
  - Wrapper for LOAD DATA INFILE
  - Supports parallel imports

### Terms
- Data Pump - Oracle's high-performance export/import utility for database objects and data
- SQL*Loader - Oracle's tool for loading data from flat files into database tables
- BCP - SQL Server's Bulk Copy Program for high-performance data transfer
- SSIS - SQL Server Integration Services, a comprehensive ETL platform
- COPY - PostgreSQL's built-in command for efficient data import/export
- mysqldump - MySQL's utility for database backup and export
- LOAD DATA INFILE - MySQL's command for bulk loading data from files
- ETL - Extract, Transform, Load process for data integration
- Control File - Configuration file defining data format for SQL*Loader
- Format File - Configuration file defining data structure for BCP and BULK INSERT

///

## What is the primary purpose of Oracle's Data Pump Export (expdp)?

---

A) Loading data from flat files

B) Exporting database objects to binary dump files

C) Creating virtual tables from flat files

D) Executing PL/SQL scripts

---

Exporting database objects to binary dump files

///

## Which SQL Server tool is best suited for complex ETL processes?

---

A) BCP

B) Import/Export Wizard

C) SSIS

D) BULK INSERT

---

SSIS

///

## What is a key feature of PostgreSQL's COPY command?

---

A) Requires a control file

B) Only works with binary formats

C) Fast and efficient data transfer

D) Limited to small datasets

---

Fast and efficient data transfer

///

## Which MySQL tool requires the FILE privilege to operate?

---

A) mysqldump

B) LOAD DATA INFILE

C) SELECT ... INTO OUTFILE

D) mysqlimport

---

SELECT ... INTO OUTFILE

///

## What is the main difference between Oracle's SQL*Loader and UTL_FILE Package?

---

A) SQL*Loader is faster but less flexible

B) UTL_FILE Package supports parallel processing

C) SQL*Loader requires directory objects

D) UTL_FILE Package is better for large datasets

---

SQL*Loader is faster but less flexible

///

## Which tool is NOT directly used for flat file operations in Oracle?

---

A) SQL*Loader

B) External Tables

C) Data Pump

D) UTL_FILE Package

---

Data Pump

///

## What is a key consideration when using BCP in SQL Server?

---

A) It only works with CSV files

B) It requires a GUI interface

C) It needs format files for complex mappings

D) It cannot handle large datasets

---

It needs format files for complex mappings

///

## Which PostgreSQL tool is primarily used for database migrations?

---

A) COPY

B) \copy

C) pg_dump

D) psql

---

pg_dump

///

## What is a limitation of MySQL's mysqldump?

---

A) Cannot handle compressed files

B) Slow for very large databases

C) Only works with binary formats

D) Requires GUI interface

---

Slow for very large databases

///

## Which tool allows querying flat files as if they were database tables?

---

A) Oracle External Tables

B) SQL Server BCP

C) PostgreSQL COPY

D) MySQL LOAD DATA INFILE

---

Oracle External Tables

