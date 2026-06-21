# Salesforce Analytics & SOQL MCP Server

Run SOQL queries, execute reports, view dashboards, and analyze CRM data in real-time through natural conversation.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/salesforce-analytics-soql)

## Overview
**Category:** industry-titans
**Tools Count:** 6

## Description
The most powerful Salesforce integration — **raw SOQL access** to any data in your org.

### What you can do
- **SOQL** — Run any query against standard or custom objects
- **Reports** — List and execute Salesforce reports
- **Dashboards** — View dashboard components and data
- **Counts** — Get record counts for any object

### Who is this for?
- **Executives** — "What was our win rate last quarter?"
- **RevOps** — Instant data without waiting for BI
- **Analysts** — Ad-hoc queries through conversation


## Available Tools
- **sf_get_dashboard**: Each component includes its type, header, data values, and the source report. Dashboards provide pre-built visual summaries. Get the dashboard ID from sf_list_dashboards. Use when the user asks "show me the sales dashboard" or wants a visual summary of specific metrics.

Get all component data from a specific Salesforce dashboard — charts, metrics, and tables with their underlying data
- **sf_record_count**: Returns the total number of records. Use for quick data volume checks: "how many leads do we have?", "total number of accounts", or capacity planning. Accepts any standard or custom object API name.

Get the total record count for any Salesforce object — Account, Contact, Lead, Opportunity, Case, or any custom object
- **sf_list_dashboards**: Returns dashboard title, folder, last referenced date, and dashboard ID. Dashboards contain visual components (charts, tables, metrics) built from reports. Use to find dashboard IDs before fetching their component data with sf_get_dashboard.

List available Salesforce dashboards with title, folder, and last referenced date to discover visualization assets
- **sf_list_reports**: Returns report name, folder path, report format (Tabular/Summary/Matrix), last run date, and report ID. Use when the user asks about available reports, wants to find a specific one, or needs report IDs before running them with sf_run_report.

List available Salesforce reports with name, folder, format, and last run date to discover reporting assets
- **sf_run_report**: Get the report ID from sf_list_reports first. This is the read-only equivalent of clicking "Run Report" in the Salesforce UI. Returns up to 2000 rows. Use when the user asks for specific report data or wants to extract insights from a saved report.

Execute a specific Salesforce report by ID and return its full data — all rows, columns, and groupings
- **sf_run_soql**: This is the most powerful and flexible tool — you can query any standard or custom object, apply filters, use aggregate functions, and join related objects. Example: SELECT Id, Name, Amount, StageName FROM Opportunity WHERE StageName = 'Closed Won' AND Amount > 10000 LIMIT 10. Use when no other tool covers the specific data need, or when the user requests a custom query.

Execute a raw SOQL query against your Salesforce org to retrieve any data from standard or custom objects


## Installation & Usage

To install and use the **Salesforce Analytics & SOQL** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/salesforce-analytics-soql](https://vinkius.com/mcp/salesforce-analytics-soql)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
