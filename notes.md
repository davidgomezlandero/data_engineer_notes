# First stack to learn

# Interview tips 

- Take notes 

# Stack overview

The required/common stack includes:

* Snowflake - SQL, Python
* Github / Workflows / Azure DevOps
* Openflow (Snowflake hosted would be beneficial)
* DBT - DBT Core / DBT Project (not Cloud)
* Cortex AI functions to process documentation and extract key information
* Contractual documentation extraction and reporting
* Data modelling (Star Schema)
* Power BI report creation (design, build and testing)

---

# Learning Priorities

Not all technologies have the same importance.

Priority order:

1. Snowflake
2. SQL
3. DBT
4. Data Modelling (Star Schema)
5. Cortex AI
6. GitHub Workflows / Azure DevOps
7. Power BI
8. Openflow

---

# Snowflake

## Goal

Understand the Snowflake ecosystem and be able to discuss it confidently during interviews.

## Core Concepts

### Architecture

Understand:

* Separation of Storage and Compute
* Cloud Services Layer
* Scalability
* Data Sharing

### Warehouses

Virtual compute clusters used to execute queries.

Learn:

* Warehouse sizing
* Auto suspend
* Auto resume

### Databases and Schemas

Hierarchy:

```text
Account
 └── Database
      └── Schema
           └── Tables
```

### Snowpark

Learn:

* Python support
* DataFrames
* Data processing inside Snowflake

### Cortex AI

Learn:

* Summarization
* Classification
* Information Extraction
* LLM integration

---

## Recommended Resources

### Snowflake in 100 Seconds

Quick overview.

### Snowflake Tutorial for Beginners

Complete beginner introduction.

### Snowflake Documentation

Focus on:

* Architecture
* Warehouses
* Snowpark
* Cortex

---

# SQL

## Topics

### Fundamentals

* SELECT
* WHERE
* GROUP BY
* ORDER BY
* HAVING

### Joins

* INNER JOIN
* LEFT JOIN
* RIGHT JOIN
* FULL JOIN

### Aggregations

* COUNT
* SUM
* AVG
* MIN
* MAX

### Window Functions

* ROW_NUMBER
* RANK
* DENSE_RANK
* LAG
* LEAD

### CTEs

Common Table Expressions.

### Performance

Basic query optimization.

---

# DBT

## Goal

Understand how modern data teams transform data.

## Core Concepts

### Sources

Raw input tables.

### Models

SQL transformations.

### Tests

Data quality checks.

### Documentation

Automatic lineage and documentation.

### Materializations

* View
* Table
* Incremental

---

## Typical Workflow

```text
Raw Data
    ↓
Snowflake
    ↓
DBT Models
    ↓
Analytics Tables
    ↓
Power BI
```

---

## Resources

* What is DBT?
* DBT Fundamentals
* DBT Documentation

---

# Data Modelling

## Goal

Understand analytical database design.

---

## Fact Tables

Store measurements.

Example:

```text
FactSales

sale_id
customer_id
product_id
amount
date
```

---

## Dimension Tables

Store descriptive information.

Example:

```text
DimCustomer

customer_id
name
country
```

```text
DimProduct

product_id
category
brand
```

---

## Star Schema

```text
           DimCustomer
                 |
                 |
DimProduct --- FactSales --- DimDate
                 |
                 |
            DimStore
```

Benefits:

* Fast analytics
* Easy reporting
* Simple BI integration

---

# Cortex AI

## Goal

Understand AI capabilities inside Snowflake.

### Use Cases

* Contract analysis
* Document extraction
* Classification
* Summarization
* Question answering

---

## Typical Flow

```text
PDF Contract
      ↓
Cortex AI
      ↓
Extract Entities
      ↓
Generate Structured Data
      ↓
Reporting Dashboard
```

---

# GitHub Workflows

## Goal

Understand CI/CD concepts.

### Topics

* Actions
* Workflows
* Triggers
* Jobs
* Runners

---

## Example

```text
Push
 ↓
Tests
 ↓
Build
 ↓
Deploy
```

---

# Azure DevOps

## Goal

Understand equivalent concepts.

### Topics

* Repositories
* Pipelines
* Boards
* Releases

---

# Power BI

## Goal

Understand reporting workflows.

### Learn

* Data Sources
* Dashboards
* Reports
* Visualizations
* Filters
* KPIs

---

## Typical Flow

```text
Snowflake
     ↓
DBT
     ↓
Power BI
     ↓
Business Dashboard
```

---

# HR Interview Preparation

The first interview is usually a screening interview, not a technical interview.

Main objectives:

* Validate communication skills
* Validate English level
* Discuss expectations
* Discuss availability
* Assess cultural fit
* Evaluate overall suitability

---

# Personal Introduction

Prepare a 60-90 second answer.

Template:

```text
My name is David.

I have a background in software development and machine learning.

Recently I have been focusing on ML projects, Python, Docker, FastAPI and learning MLOps and cloud technologies.

I enjoy building systems, learning new technologies and working on data and AI-related projects.
```

---

# Common Questions

## Tell me about yourself

Prepare a 1-minute answer.

---

## Why are you interested in this role?

Focus on:

* Data
* AI
* Automation
* Learning opportunities

---

## What experience do you have with Snowflake?

Never fake experience.

Example:

"I have not used Snowflake professionally yet, but I have been studying its architecture and ecosystem and I understand how it fits into modern data platforms."

---

## What are your strengths?

Examples:

* Fast learner
* Strong Python skills
* Project-oriented mindset
* Problem-solving ability

---

## Why should we hire you?

Focus on:

* Adaptability
* Motivation
* Technical foundation
* Learning speed

---

# Salary Discussion

Before giving numbers:

Ask:

"What is the compensation range budgeted for the role?"

If required to answer:

Provide a range instead of a fixed number.
range 25k-35 in getmanfred but i will ask 30k-35k

---

# English Speaking Preparation

## Method 1

Voice conversation with ChatGPT.

Prompt:

"Conduct a realistic HR interview for a Data Engineering role. Ask one question at a time and correct my English after each answer."

---

## Method 2

Record yourself answering:

* Tell me about yourself
* Why this role?
* Why should we hire you?
* What experience do you have with Snowflake?

---

## Method 3

Shadowing

Listen and repeat interview answers from YouTube.

Goal:

Improve fluency, confidence and pronunciation.

---

# Final Interview Goal

Do NOT try to look like a Senior Snowflake Engineer.

Instead:

Demonstrate:

* Strong technical foundations
* Ability to learn quickly
* Interest in Data Engineering
* Communication skills
* Professional attitude

The objective of the first interview is to advance to the technical stage.

# Star project explanations

