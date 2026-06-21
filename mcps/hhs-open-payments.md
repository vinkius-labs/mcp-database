# HHS Open Payments MCP Server

Access the HHS Open Payments database to search for physicians, teaching hospitals, and financial relationships in the healthcare industry.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/hhs-open-payments)

## Overview
**Category:** government-public-data
**Tools Count:** 6

## Description
Connect to the **HHS Open Payments** database to explore financial transparency in healthcare. This server allows you to query datasets, search for specific physicians or teaching hospitals, and analyze payments made by drug and device companies.

### What you can do

- **Dataset Discovery** — List all available Open Payments datasets and inspect their metadata, including column definitions and update timestamps.
- **Physician & Hospital Search** — Search for specific healthcare providers or teaching hospitals by name to find their associated records.
- **Advanced Querying** — Use Socrata Query Language (SoQL) to filter, sort, and limit data for precise financial analysis.
- **Data Export** — Download specific datasets in CSV, JSON, or XML formats for external processing or reporting.
- **Metadata Inspection** — Fetch detailed information about specific datasets to understand the underlying data structure.

### How it works

1. Subscribe to this server
2. Enter your HHS/Socrata API Key (optional but recommended for higher rate limits)
3. Start auditing healthcare financial data directly from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers & Journalists** — Uncover financial ties between the medical industry and healthcare professionals for investigative reporting.
- **Compliance Officers** — Monitor and verify the accuracy of reported financial transfers within healthcare organizations.
- **Healthcare Consumers** — Check for potential conflicts of interest or financial relationships of their medical providers.


## Available Tools
- **download_dataset**: JSON is recommended for programmatic access.

Download a specific Open Payments dataset
- **get_dataset**: Get metadata for a specific Open Payments dataset
- **list_datasets**: List all available Open Payments datasets
- **query_dataset**: Query specific records within a dataset using SoQL
- **search_hospitals**: Search for specific teaching hospitals
- **search_physicians**: Search for specific physicians


## Installation & Usage

To install and use the **HHS Open Payments** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hhs-open-payments](https://vinkius.com/mcp/hhs-open-payments)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
