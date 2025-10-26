# PostgreSQL Time-Series Optimization

This project demonstrates how to optimize Time-Series queries in PostgreSQL, achieving up to **59x faster query performance** using Partitioning.

## Project Overview

This project involved a practical performance analysis of storing 10 million sensor records in PostgreSQL. We compared the performance of a single large table against a partitioned table structure (partitioned by month).

The key metrics for comparison were query `Execution Time` and disk `I/O` (Buffers read), measured using `EXPLAIN (ANALYZE, BUFFERS)`.

## Key Achievements

* **Query 1 (Single Day):** Achieved a **40x speed improvement** (from 1748ms down to 44ms).
* **Query 2 (Monthly Aggregation):** Achieved a **2x speed improvement** (from 2199ms down to 1196ms).
* **Query 3 (Device-Specific Month):** Achieved a **59x speed improvement** (from 1538ms down to 26ms).

## Key Technologies
* PostgreSQL
* Advanced SQL
* Table Partitioning (Range Partitioning)
* Query Performance Tuning
* Indexing (B-Tree)
* `EXPLAIN ANALYZE`

## Report
The full technical analysis, methodology, and query results are available in the `پروژه کارگاه SQL.pdf` file in this repository.
