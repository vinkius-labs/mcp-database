# OSTI (DOE Scientific Research) MCP Server

Access Department of Energy research, datasets, and scientific publications. Search records, retrieve metadata, and manage DOI registrations.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/osti-doe-scientific-research)

## Overview
**Category:** knowledge-management
**Tools Count:** 6

## Description
Connect to the **Office of Scientific and Technical Information (OSTI)** to query the US Department of Energy's vast research output. This MCP server allows AI agents to navigate millions of research records and datasets through natural conversation.

### What you can do

- **Research Search** — Query OSTI.GOV for publications, reports, and conference papers using authors, titles, or specific identifiers.
- **Dataset Discovery** — Search the DOE Data Explorer specifically for scientific datasets and retrieve detailed metadata for data-driven insights.
- **Record Inspection** — Fetch comprehensive bibliographic data and full-text availability for specific records using unique OSTI IDs.
- **DOI Management** — Reserve and submit Digital Object Identifiers (DOIs) via the E-Link API for DOE-funded scientific research and data.
- **Advanced Filtering** — Narrow down results by sponsoring organization, research organization, or specific publication date ranges.

### How it works

1. Subscribe to this server
2. (Optional) Enter your OSTI E-Link Token for DOI reservation and submission features
3. Start searching and analyzing scientific data directly from Claude, Cursor, or any MCP client

### Who is this for?

- **Researchers & Academics** — quickly find relevant DOE-funded literature and datasets without manual portal searching
- **Data Scientists** — discover and inspect metadata for scientific datasets to fuel analysis and modeling
- **Grant Administrators** — manage DOI registrations and verify record submissions for funded projects


## Available Tools
- **get_data_explorer_record**: Get a single DOE Data Explorer record by ID
- **get_osti_record**: Get a single OSTI.GOV record by ID
- **reserve_doi**: Requires minimal metadata.

Reserve a DOI via E-Link API
- **search_data_explorer_records**: Search DOE Data Explorer records (datasets)
- **search_osti_records**: Search OSTI.GOV records
- **submit_record**: Submit/Update a record and register DOI via E-Link API


## Installation & Usage

To install and use the **OSTI (DOE Scientific Research)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/osti-doe-scientific-research](https://vinkius.com/mcp/osti-doe-scientific-research)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
