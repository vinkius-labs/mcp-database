# Open Payments (CMS Physician Data) MCP Server

Query official CMS Open Payments data to analyze financial relationships between the healthcare industry, physicians, and teaching hospitals.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/open-payments-cms-physician-data)

## Overview
**Category:** data-analytics
**Tools Count:** 5

## Description
The **Open Payments** MCP server provides direct access to the Centers for Medicare & Medicaid Services (CMS) database. This transparency program publishes data about financial relationships between reporting entities (like drug and medical device companies) and covered recipients (physicians and teaching hospitals).

### What you can do

- **Physician Search** — Locate specific healthcare providers using NPI, name, or specialty via `search_physicians`.
- **Hospital Lookup** — Find teaching hospitals by name or address using `search_teaching_hospitals`.
- **Dataset Exploration** — List all available reporting cycles and payment categories with `list_datasets`.
- **Advanced Querying** — Perform deep dives into payment records using SQL-like filters ($where, $select) via `query_dataset`.
- **Metadata Retrieval** — Get technical details and column definitions for specific datasets using `get_dataset`.

### How it works

1. Subscribe to this server
2. Enter your Open Payments API Key (App Token)
3. Start auditing healthcare financial data from Claude, Cursor, or any MCP client

### Who is this for?

- **Compliance Officers** — verify financial disclosures and industry ties for medical staff.
- **Journalists & Researchers** — analyze trends in industry spending and identify potential conflicts of interest.
- **Healthcare Analysts** — aggregate payment data to understand market influence and provider relationships.


## Available Tools
- **list_datasets**: List all available datasets in the Open Payments system
- **get_dataset**: Get detailed metadata for a specific dataset
- **query_dataset**: Search records within a specific dataset
- **search_physicians**: Search for specific physicians
- **search_teaching_hospitals**: Search for specific teaching hospitals


## Installation & Usage

To install and use the **Open Payments (CMS Physician Data)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/open-payments-cms-physician-data](https://vinkius.com/mcp/open-payments-cms-physician-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
