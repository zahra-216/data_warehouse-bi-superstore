# Data Warehouse & Business Intelligence Solution

An end-to-end data warehousing and business intelligence project built on the **Superstore Sales** dataset. It covers the full pipeline from staging raw source data, through ETL and dimensional modelling, to an OLAP cube and interactive analytical dashboards.

## Overview

The project takes raw sales data and turns it into an analytics-ready solution:

- **Staging layer** - a multi-source staging area to land and prepare raw data
- **ETL pipelines** - built with SSIS to extract, clean, transform, and load data into the warehouse
- **Data warehouse** - a star schema with **Slowly Changing Dimensions (Type 2)** for historical tracking
- **OLAP cube** - an SSAS cube for multidimensional analysis (slice, dice, drill operations)
- **Dashboards** - interactive Power BI reports with drill-down, drill-through, and cascading slicers

## Star Schema

The warehouse is modelled as a star schema with a central fact table surrounded by dimension tables, using SCD Type 2 to preserve history.

![Star Schema](docs/star-schema.png)

## Power BI Dashboard

Interactive dashboards built on the cube, supporting drill-down, drill-through, and cascading slicers for exploring sales performance.

![Power BI Dashboard](docs/powerbi-dashboard.png)

> For all other screenshots - the SSIS data flows, the SSAS cube structure, additional dashboard pages, and the full explanation of each stage, see the complete report in the **Document** folder.

## Tech Stack

- **Database:** SQL Server
- **ETL:** SQL Server Integration Services (SSIS)
- **OLAP:** SQL Server Analysis Services (SSAS)
- **Reporting:** Power BI
- **Other:** Excel

## Repository Structure

- **CubeProject** - the SSAS cube project (multidimensional model for OLAP analysis)
- **DataWarehouse** - the data warehouse database backup (`.bak`), containing the star schema
- **Document** - the full project report with detailed screenshots and explanations of every stage
- **Excel** - Excel workbook demonstrating OLAP operations
- **PowerBIReports** - the Power BI dashboard file (`.pbix`)

## About

Individual project built for the Data Warehousing & Business Intelligence module (IT3021) at SLIIT, on the Superstore Sales dataset.
