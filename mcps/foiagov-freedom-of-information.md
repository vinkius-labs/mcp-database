# FOIA.gov (Freedom of Information) MCP Server

Access US government FOIA data — list agency components, retrieve request forms, and fetch annual reports directly from FOIA.gov.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/foiagov-freedom-of-information)

## Overview
**Category:** knowledge-management
**Tools Count:** 4

## Description
Connect to the **FOIA.gov** API to streamline access to Freedom of Information Act data. This MCP server allows AI agents to navigate the complex structure of US government agencies and their specific FOIA requirements through natural conversation.

### What you can do

- **Agency Discovery** — List all FOIA agency components and filter by specific fields like titles and abbreviations.
- **Component Details** — Fetch deep metadata for specific agency components using their unique UUIDs.
- **Request Forms** — Retrieve the exact structure and fields required for FOIA request forms for any specific component.
- **Annual Reports** — Access NIEM-standard XML annual reports for agencies by year to analyze transparency metrics.

### How it works

1. Subscribe to this server
2. Enter your FOIA.gov API Key
3. Start querying government transparency data from your AI assistant

### Who is this for?

- **Journalists & Researchers** — quickly identify which agency components handle specific types of records.
- **Legal Professionals** — automate the retrieval of request form structures to ensure compliance with agency-specific requirements.
- **Data Analysts** — pull annual report data in XML format for large-scale transparency analysis.


## Available Tools
- **get_agency_component_request_form**: Fetch the FOIA request form structure for a specific component
- **get_agency_component**: Fetch a specific agency component by UUID
- **get_annual_report_xml**: Fetch an agency annual report in XML format
- **list_agency_components**: Supports JSON API sparse fieldsets and includes.

List all FOIA agency components


## Installation & Usage

To install and use the **FOIA.gov (Freedom of Information)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/foiagov-freedom-of-information](https://vinkius.com/mcp/foiagov-freedom-of-information)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
