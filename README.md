# PostgreSQL Time-Series Optimization

[cite_start]This project demonstrates how to optimize Time-Series queries in PostgreSQL, achieving up to **59x faster query performance** using Partitioning[cite: 623].

## Project Overview

[cite_start]This project involved a practical performance analysis of storing 10 million sensor records in PostgreSQL[cite: 447, 509]. [cite_start]We compared the performance of a single large table against a partitioned table structure (partitioned by month)[cite: 444].

[cite_start]The key metrics for comparison were query `Execution Time` and disk `I/O` (Buffers read), measured using `EXPLAIN (ANALYZE, BUFFERS)`[cite: 444, 445].

## Key Achievements

* [cite_start]**Query 1 (Single Day):** Achieved a **40x speed improvement** (from 1748ms down to 44ms)[cite: 452, 512, 623].
* [cite_start]**Query 2 (Monthly Aggregation):** Achieved a **2x speed improvement** (from 2199ms down to 1196ms)[cite: 492, 548, 623].
* [cite_start]**Query 3 (Device-Specific Month):** Achieved a **59x speed improvement** (from 1538ms down to 26ms)[cite: 500, 590, 623].

## Key Technologies
* PostgreSQL
* Advanced SQL
* [cite_start]Table Partitioning (Range Partitioning) [cite: 508]
* Query Performance Tuning
* [cite_start]Indexing (B-Tree) [cite: 448]
* [cite_start]`EXPLAIN ANALYZE` [cite: 445]

## Report
The full technical analysis, methodology, and query results are available in the `پروژه کارگاه SQL.pdf` file in this repository.
