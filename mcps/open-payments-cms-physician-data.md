# Open Payments (CMS Physician Data) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/open-payments-cms-physician-data)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/open-payments-cms-physician-data-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/open-payments-cms-physician-data-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Query official CMS Open Payments data to analyze financial relationships between the healthcare industry, physicians, and teaching hospitals.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Open Payments (CMS Physician Data)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available datasets in the Open Payments system."

**🤖 AI Agent:**
> I've retrieved the available datasets. There are several reporting cycles available, including 'General Payments 2023' (ID: pg6p-7v62) and 'Research Payments 2023' (ID: 5930-21xa). Which one would you like to explore?

---

**👤 You:**
> "Search for physicians with the specialty 'Cardiology' named 'Smith'."

**🤖 AI Agent:**
> Searching the physician database... I found 3 matches for 'Smith' in Cardiology. Would you like to see their NPI numbers or check for payments associated with one of them?

---

**👤 You:**
> "Query dataset 'pg6p-7v62' for payments where the amount is greater than 5000."

**🤖 AI Agent:**
> Executing query on dataset pg6p-7v62... I found 12 records matching that criteria. The largest payment was $25,000 made to a teaching hospital in Boston. Should I list the top 5 results?


## Installation & Usage

To install and use the **Open Payments (CMS Physician Data)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/open-payments-cms-physician-data](https://vinkius.com/mcp/open-payments-cms-physician-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
