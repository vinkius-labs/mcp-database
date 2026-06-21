# USAJOBS (OPM) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/usajobs-opm)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/usajobs-opm-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/usajobs-opm-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Search and analyze federal job opportunities directly from USAJOBS. Access active listings, historic data, and detailed job requirements.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **USAJOBS (OPM)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for active Software Engineer jobs in Washington, DC with a minimum salary of $100,000."

**🤖 AI Agent:**
> I found 12 active Software Engineer positions in Washington, DC meeting your criteria. Notable listings include a Lead Developer role at the Department of State and a Senior Engineer position at NASA. Would you like the details for any of these?

---

**👤 You:**
> "Get the full duties and qualifications for announcement number 784521900."

**🤖 AI Agent:**
> Retrieving announcement text... For JOA 784521900, the primary duties involve managing cloud infrastructure and ensuring cybersecurity compliance. Qualifications require at least one year of specialized experience at the GS-12 level. Shall I summarize the full text for you?

---

**👤 You:**
> "List the occupational series codes for Information Technology positions."

**🤖 AI Agent:**
> I've fetched the code list. For Information Technology, the primary series is 2210. Other related codes include 1550 (Computer Science) and 0854 (Computer Engineering).


## Installation & Usage

To install and use the **USAJOBS (OPM)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/usajobs-opm](https://vinkius.com/mcp/usajobs-opm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
