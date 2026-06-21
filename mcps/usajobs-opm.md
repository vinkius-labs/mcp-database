# USAJOBS (OPM) MCP Server

Search and analyze federal job opportunities directly from USAJOBS. Access active listings, historic data, and detailed job requirements.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/usajobs-opm)

## Overview
**Category:** industry-titans
**Tools Count:** 4

## Description
Connect to the official **USAJOBS** (Office of Personnel Management) database to explore federal career opportunities through your AI agent. This server provides comprehensive access to the federal hiring ecosystem.

### What you can do

- **Active Job Search** — Query live job announcements using keywords, locations, salary ranges, and hiring paths (e.g., Veterans, Students, Public).
- **Historic Data Retrieval** — Access bulk data for current and past job opportunity announcements (JOAs) for trend analysis or research.
- **Detailed Job Analysis** — Fetch full text for specific announcements, including detailed summaries, duties, and qualification requirements.
- **Reference Data** — Retrieve valid codes for occupational series, agency subelements, pay plans, and more to refine your searches.

### How it works

1. Subscribe to this server
2. Enter your USAJOBS API Key and User Agent (email address)
3. Start searching for federal roles directly from Claude, Cursor, or any MCP client

### Who is this for?

- **Job Seekers** — Find specific federal roles that match your skills and location without navigating complex search filters manually.
- **Career Counselors** — Help clients identify federal career paths and understand specific qualification requirements.
- **Data Analysts** — Analyze federal hiring trends using historic JOA data and occupational series codes.


## Available Tools
- **get_announcement_text**: for historic JOAs.

Retrieve long text fields for current and past job postings
- **get_code_list**: No auth required.

Retrieve valid values and codes for filtering search results
- **get_historic_joas**: Supports pagination via continuationtoken.

Retrieve bulk data for current and past job postings
- **search_jobs**: You can filter by keyword, location, job category, and more.

Search for currently open job announcements on USAJOBS


## Installation & Usage

To install and use the **USAJOBS (OPM)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/usajobs-opm](https://vinkius.com/mcp/usajobs-opm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
