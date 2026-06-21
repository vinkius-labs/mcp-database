# MaestroQA MCP Server

Access quality assurance reviews, QA scores, and export performance data via the MaestroQA API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/maestroqa)

## Overview
**Category:** customer-support
**Tools Count:** 7

## Description
Connect your **MaestroQA** account to any AI agent to automate your customer service quality assurance and performance reporting. This MCP server enables your agent to list tickets, monitor QA scores, request detailed data exports, and sync external CSAT scores directly from natural language interfaces.

### What you can do

- **Score Monitoring** — List support tickets and retrieve real-time Internal Quality Scores (IQS) and grading statuses
- **Automated Exporting** — Initialize asynchronous raw data exports for deep analysis of rubric answers and performance
- **Agent Oversight** — List all support agents and available evaluation rubrics to organize your QA process
- **CSAT Synchronization** — Push external customer satisfaction scores into MaestroQA to correlate them with internal QA grades
- **Detailed Auditing** — Retrieve complete metadata and scoring breakdowns for any individual ticket

### How it works

1. Subscribe to this server
2. Enter your MaestroQA (Rippit) API Token
3. Start managing your support quality from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **QA Managers** — Monitor support quality trends and export grading data via simple natural language commands
- **Support Leads** — Quickly audit agent performance and identify tickets awaiting review from your dev tools
- **Operations Teams** — Automate the synchronization of CSAT data and maintain accurate quality reporting effortlessly


## Available Tools
- **list_qa_agents**: List all agents tracked in MaestroQA
- **get_export_download_links**: Retrieve links for a requested export
- **get_ticket_qa_details**: Get QA details for a specific ticket
- **push_csat_scores**: Sync external CSAT scores into MaestroQA
- **request_qa_data_export**: Requires start_date and end_date.

Initialize a raw QA data export (Async)
- **list_qa_rubrics**: List all available evaluation rubrics
- **list_qa_tickets**: Use optional params for filtering.

List tickets and their QA statuses


## Installation & Usage

To install and use the **MaestroQA** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/maestroqa](https://vinkius.com/mcp/maestroqa)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
