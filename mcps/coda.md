# Coda MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/coda)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/coda-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/coda-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Enable your AI agent to manage docs, tables, formulas, and rows via the Coda API.

## Description
Connect your AI to **Coda**, the collaborative document platform that brings together words, data, and teams.

### What you can do

- **Document Browsing** — List your recent docs and navigate their sections, tables, and pages.
- **Table Data** — Read rows from any Coda table, filter by column values, and update records.
- **Formula Values** — Retrieve the live value of any named formula in a doc for real-time reporting.

### How it works

1. Add the Coda integration to your AI toolset.
2. Provide your API Token (from Account Settings in Coda).
3. Manage your docs and data via natural language.

### Who is this for?

- **Product Managers** — Pull table data and formula results without opening the doc.
- **Operations Teams** — Update tracker tables and check statuses from chat.
- **Developers** — Automate data sync between Coda docs and other systems.


## Available Tools
- **delete_rows**: Delete one or more rows from a Coda table
- **get_doc_details**: Retrieve detailed information about a specific Coda document
- **get_formula_value**: Retrieve the current calculated value of a named formula
- **insert_rows**: Insert new rows into a Coda table
- **list_columns**: Retrieve a list of columns in a Coda table
- **list_docs**: Retrieve a list of Coda documents available to you
- **list_formulas**: Retrieve a list of named formulas in a Coda document
- **list_rows**: Retrieve rows from a specific table in a Coda document
- **list_tables**: Retrieve a list of tables within a specific Coda document
- **update_row**: Update an existing row in a Coda table


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Coda** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me my recent documents in Coda."

**🤖 AI Agent:**
> You have 8 docs:
1. 'Project Tracker' — last edited 1h ago, 3 tables
2. 'Q1 OKRs' — last edited yesterday, 2 tables
3. 'Sprint Board' — last edited 3 days ago, 5 tables
Would you like to read data from any of these?

---

**👤 You:**
> "Get the current value of formula 'TotalBudget' in doc 'doc-yyyy'."

**🤖 AI Agent:**
> Formula 'TotalBudget' in doc 'doc-yyyy': **$142,500.00**. Last recalculated: 3 minutes ago.

---

**👤 You:**
> "Check the status of task 'Q3 Launch' in our Sprint Board table."

**🤖 AI Agent:**
> Scanning the 'Sprint Board' table. Task 'Q3 Launch' is currently marked as 'In Progress'. It is assigned to Sarah and has a targeted delivery of this coming Friday.


## Installation & Usage

To install and use the **Coda** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coda](https://vinkius.com/mcp/coda)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
