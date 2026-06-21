# Amazon Redshift MCP Server

Equip your AI to directly query, analyze, and manage your petabyte-scale data warehouse via the serverless AWS Redshift Data API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/amazon-redshift)

## Overview
**Category:** industry-titans
**Tools Count:** 7

## Description
Connect your **Amazon Redshift** data warehouse securely to your AI agent utilizing the AWS Redshift Data API. This integration empowers your AI interface to natively run aggregations, explore massive schemas, and retrieve historical executing query logs asynchronously without requiring persistent DB connection pools, JDBC drivers, or complex networking configurations.

### What you can do

- **Execute Asynchronous SQL** — Direct the AI to execute standard SQL commands (`execute_sql`), including complex SELECT aggregations, table creation (DDL), or data mutation (DML). Since it uses the Data API, long-running queries will process in the background.
- **Poll & Retrieve Results** — Ask the agent to proactively monitor the execution lifecycle (`statement_status`) of dispatched query IDs and retrieve the dataset rows (`get_results`) securely into your terminal upon completion.
- **Schema & Table Discovery** — Understand the database structure dynamically by generating lists of available schemas (`list_schemas`) or looking up column metadata metrics for specific tables (`describe_table`).
- **Statement Histories** — Perform audits assessing previously submitted query structures and track analytical workloads running on your configured cluster (`list_statements`).

### How it works

1. Authorize the Amazon Redshift MCP plugin from your connected extension hub.
2. Configure your serverless integration using standard AWS IAM principles. Supply an Access Key ID & Secret targeting your cluster, identifying the specific endpoint, Database Name, and DB User.
3. Chat seamlessly with your AI to prompt queries like "Describe the metadata for the 'public.events' table" or "Execute a query counting all sales processed yesterday."

### Who is this for?

- **Data Analysts & Scientists** — Execute ad-hoc exploratory aggregations through natural language prompts. Pull specific dataset metrics and schemas instantly into chat without switching to external SQL IDEs like DBeaver.
- **Backend Developers** — Test schema migrations intuitively. Troubleshoot data integrations and check table state integrity interactively from the code editor during development.
- **Data Engineers** — Audit Redshift cluster loads and verify execution lifecycles asynchronously for large reporting workloads directly connected to your conversational toolkit.


## Available Tools
- **describe_table**: Retrieves column metadata for a table
- **execute_sql**: This is an asynchronous operation that returns a statement ID.

Executes a SQL statement using the Redshift Data API
- **get_results**: Retrieves the results of a completed SQL statement
- **statement_status**: Checks the execution status of a SQL statement
- **list_schemas**: Lists all database schemas in Redshift
- **list_statements**: Lists recent SQL statements executed in the cluster
- **list_tables**: Lists all tables in a specific schema


## Installation & Usage

To install and use the **Amazon Redshift** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/amazon-redshift](https://vinkius.com/mcp/amazon-redshift)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
