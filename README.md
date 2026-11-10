# SmartHome Database System

**Microsoft SQL Server | Relational Database Design | T-SQL | Business Intelligence**

A relational database design and implementation project developed for a fictional smart-home company, Smart Homes. The project focuses on database architecture, data relationships, business operations, SQL querying, automated business rules and analytical reporting.

## Project Overview

The system is designed to support the operational and administrative activities of a smart-home installation business.

It brings together customer management, properties, smart-home devices, installations, staff allocation, suppliers, inventory, orders, invoices and payments within a relational database structure.

The implementation explores relational database principles alongside practical SQL development, with particular attention to data consistency, normalisation, referential integrity and business-rule enforcement.

![DB Layout](./screenshots/DB%20Layout.png)

## Technical Stack

- **Microsoft SQL Server** – Relational database management.
- **T-SQL** – Database queries, procedures and triggers.
- **Visual Paradigm** – Entity Relationship Diagram design.
- **SQL Server Management Studio (SSMS)** – Database implementation and query execution.
- **Dashboard & Data Visualisation** – Business performance and operational insights.

## Database Design

The database was designed using an Entity Relationship Diagram (ERD), identifying entities, attributes, primary keys, foreign keys and relationships.

Key database components include:

- CLIENTS & PROPERTIES – Customer and property records.
- STAFF & TEAMS – Employee information and installation team allocation.
- DEVICES & CONTROLLERS – Smart-home equipment and compatibility information.
- INSTALLATIONS & DESIGNS – Installation records and customer-specific designs.
- SUPPLIERS & STOCK – Supplier relationships and inventory management.
- ORDERS & DEVICE_ORDERS – Procurement and device ordering.
- INVOICES & PAYMENTS – Financial transaction management.
- SENSOR_READINGS & DATACENTER – Device readings and data records.
- MAINTENANCE_CALLOUTS – Maintenance and service management.

## Database Principles

The implementation incorporates:

- First, Second and Third Normal Form (1NF, 2NF, 3NF).
- Functional dependency analysis.
- Primary and foreign key constraints.
- Composite keys and relational associations.
- Referential integrity.
- Data type selection and field constraints.
- One-to-many and many-to-many relationships.

## SQL Implementation

The project includes several queries and database operations demonstrating practical T-SQL development.

| Implementation | Functionality |
|---|---|
| Client_Cost_Total | Identifies highest and lowest customer design expenditure. |
| WiFi_Order_Status | Analyses Wi-Fi device orders by supplier and order status. |
| Weekly_Availability | Identifies staff availability within the upcoming seven-day period. |
| Double_Booking_Avoidance | Implements a database trigger to prevent conflicting staff allocations. |
| Installation_Costs | Calculates installation costs using weekly, monthly and quarterly date parameters. |
| Dashboard | Presents business performance and operational trends. |

### Advanced SQL Concepts

- Multi-table JOIN operations.
- Aggregate functions and conditional COUNT expressions.
- GROUP BY and HAVING.
- Date manipulation using GETDATE() and DATEADD().
- Stored procedures and input parameters.
- Window functions and PARTITION BY.
- Database triggers.
- Transaction rollback and error handling.
- Composite keys and relational constraints.

## Design Decisions & Development Challenges

During implementation, several refinements were made to the original database design to accommodate operational requirements and query functionality.

Examples include:

- Introducing additional installation date fields to support date-based queries.
- Extending device records with controller compatibility and inventory information.
- Revising team identification and key structures.
- Implementing a custom staff allocation trigger to address overlapping installations.

The implementation also involved evaluating alternative data types, nullable fields, database constraints and the practical implications of schema modifications.

These decisions form part of the project's development process and demonstrate the importance of translating conceptual database designs into functional implementations.

## Dashboard & Business Intelligence

The dashboard explores business performance through:

- Customer and design installation trends.
- Device variety and installation activity.
- Customer expenditure.
- Financial and operational insights.
- Potential business opportunities and customer trends.

The objective is to transform relational database information into meaningful business insights that can support operational and strategic decisions.

## Project Documentation

The repository includes:

- Database design and ER diagrams.
- Functional dependency documentation.
- Query examples and results.
- Database screenshots.
- Dashboard visualisations.
- Project demonstration video (where available).

## Project Background

Originally developed as part of an academic module at university.

This repository presents the independently developed database design, SQL implementation and technical documentation as part of a personal software development portfolio.

**Microsoft SQL Server | T-SQL | Database Engineering | Relational Modelling | Business Intelligence**

## Data Visualisation & Analysis

**Tableau** was connected to the Microsoft SQL Server database to create visualisations, analyse query results and present key business insights.

**SQL Queries:**
- Double Booking Avoidance
- Installation Costs
- Weekly Availability
- Wi-Fi Order Status

**Tableau Dashboards & Visualisations:**
- Installations Over Time
- Client Expenditure
- Design Installations Over Time
- Device Types Installed
- Installations by City

Video Demonstration Available on Request of the whole project

Copyright & Usage

Copyright © 2026 Laszlo Major. All rights reserved.

This repository is publicly available for portfolio and educational demonstration purposes.

The source code is provided for viewing and evaluation. No licence is granted for copying, modifying, redistributing, or commercially using this project without prior written permission from the copyright holder.

Third-party libraries and dependencies remain subject to their respective licences.
