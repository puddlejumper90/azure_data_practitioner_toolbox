# azure_data_practitioner_toolbox

2023 was a hard year for many data practitioners. Luckily, the data community is a friendly bunch finding actioanly insights for companies to get ahead--when they are employed and being fairly compensated. This is an open-source repository for the data practitioner themselves, to provide knowledge and guidance in an uncertain job market, managed by people who have never written a line of SQL code in their lives. This is repository to empower the individual.

Since I am an Azure Certified data engineer, this repository will start out, primarily being Microsoft Azure focused. If you have any ideas or information to contribute from other cloud platforms or would like to update old information, feel free to submit a pull request.

## Defined Terms and Key Concepts

### Normalization vs. Denormalization?

`Normalization` is the process of organizing data to reduce redundancy and improve data integrity by dividing a database into smaller, related tables. The goal is to eliminate duplicate data and ensure that each piece of data is stored only once. This is typically done through a series of "normal forms" (e.g., 1NF, 2NF, 3NF).

`Denormalization` is the opposite; it involves combining data from multiple tables into one, increasing redundancy to optimize read performance. Denormalization is often used when quick query performance is critical, such as in OLAP systems.

*Example Scenario*: Use normalization in OLTP (Online Transaction Processing) systems where data integrity and storage efficiency are important. Use denormalization in OLAP (Online Analytical Processing) systems where query speed is prioritized over storage.

### Streaming Process vs. Batch Process

`Streaming`: Involves real-time data processing as it comes in, providing immediate insights. This is suitable for time-sensitive applications where delays could impact decisions, like real-time analytics or monitoring systems.

`Batch Processing`: Involves processing large volumes of data in groups (batches) at scheduled intervals. It is useful for applications that don't require real-time processing, such as end-of-day reports, data backups, or historical data analysis.

*Example Scenario*: Use streaming for applications like fraud detection where immediate action is required. Use batch processing for scenarios like payroll processing or end-of-day sales reporting.

## Python Libraries

`Pandas`: For data manipulation and analysis; provides data structures and operations for manipulating numerical tables and time series.

`NumPy`: For numerical computing; useful for handling arrays and performing mathematical operations.

`SQLAlchemy`: For database connection and management; facilitates working with relational databases.

`PySpark`: For handling large-scale data processing; leverages Apache Spark for big data analytics.

`Dask`: For parallel computing; helps in scaling the Python data science stack to leverage distributed computing resources.

`Airflow`: For scheduling and orchestrating data pipelines; useful for workflow management.

## Table Structures and Related Concepts

`Fact Tables`: Contain the metrics, measurements, or facts of a business process. They are typically normalized and used in data warehouses.

`Dimension Tables`: Contain the descriptive attributes related to the facts (such as time, location, product details). They are denormalized and often used to provide context to the data in fact tables.

`Primary Key`: A unique identifier for a record in a table.

`Foreign Key`: A field (or collection of fields) in one table that uniquely identifies a row of another table.
