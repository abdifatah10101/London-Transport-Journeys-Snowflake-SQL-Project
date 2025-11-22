# London Transport Journeys — Snowflake SQL Analysis

This project analyzes public transport usage in London using a modified dataset from Transport for London (TfL). All data is stored in a Snowflake database called `TFL`, containing a single table named `JOURNEYS`. The dataset includes monthly journey volumes across modes such as the Underground, DLR, buses, trams, river services, and more.

## Dataset Structure

**Table:** `TFL.JOURNEYS`

| Column              | Description                                          | Type     |
|---------------------|------------------------------------------------------|----------|
| MONTH               | Month number (1–12)                                  | INTEGER  |
| YEAR                | Year of record                                       | INTEGER  |
| DAYS                | Number of days in the month                          | INTEGER  |
| REPORT_DATE         | Date the data was reported                           | DATE     |
| JOURNEY_TYPE        | Transport method used                                | VARCHAR  |
| JOURNEYS_MILLIONS   | Monthly journeys in millions (decimal values)        | FLOAT    |

## Project Objectives

The goal of this project was to write SQL queries in Snowflake to answer key questions about London’s transport usage:

- Identify the most popular transport types by total journeys.
- Determine the five most active months and years for Emirates Airline.
- Find the five lowest-volume years for Underground & DLR journeys.

## Skills Practiced

- Aggregations with `SUM()`
- Rounding numeric values using `ROUND()`
- Filtering with `WHERE`
- Sorting with `ORDER BY`
- Limiting results using `LIMIT`
- Grouping data using `GROUP BY`
- Understanding Snowflake’s uppercase object conventions
- Analyzing real-world public transport data for insights

## Summary

This project showcases how SQL can be used in Snowflake to analyze large public datasets and extract meaningful insights. It demonstrates practical data engineering skills and analytical thinking through exploration of transport journey trends across London.
