# College Scorecard API MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/college-scorecard-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/college-scorecard-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/college-scorecard-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access US college data — audit school performance and costs via AI.

## Description
Empower your AI agent to orchestrate your entire higher education research workflow with **College Scorecard API**, the authoritative source for United States school performance and cost data. By connecting the Department of Education's API to your agent, you transform complex college searches into a natural conversation. Your agent can instantly search for schools, audit enrollment metadata, and retrieve detailed program reports without you ever touching a government portal. Whether you are a student planning your future or a researcher monitoring academic trends, your agent acts as a real-time education consultant, ensuring your data is always grounded in official, government-verified records.

### What you can do

- **School Auditing** — Search for thousands of US colleges and universities by name and retrieve detailed metadata, including location and website links.
- **Enrollment Oversight** — Retrieve latest student body size and demographics to maintain a clear view of campus scale.
- **Geographic Discovery** — List schools by state, city, or near specific ZIP codes to identify regional academic hubs instantly.
- **Program Intelligence** — Query specific fields of study and program data to understand the academic offerings of different institutions.
- **Cost Analysis** — Retrieve data on tuition and costs to assist in financial planning for higher education.

### How it works

1. Subscribe to this server
2. Enter your Data.gov API Key
3. Start managing your education intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Students & Parents** — monitor college options and retrieve cost metadata straight from your workflow.
- **Academic Researchers** — verify enrollment trends and audit program distributions without manual database searches.
- **Guidance Counselors** — perform rapid audits of nearby schools and identify program markers through natural language.
- **Operations Leads** — automate education data querying to orchestrate cross-functional outreach teams smoothly.


## Available Tools
- **get_college_details**: Get full details for a specific college by ID
- **get_fields_of_study**: Get details for specific programs or fields of study
- **list_colleges_by_city**: List schools in a specific city
- **list_colleges_by_state**: List all schools in a specific state
- **list_colleges_by_zip**: List schools near a specific ZIP code
- **search_colleges**: Search for colleges and universities in the US


## 💬 Prompt Examples

Here are some examples of how you can interact with the **College Scorecard API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for schools named 'Harvard' using College Scorecard API."

**🤖 AI Agent:**
> I've retrieved several matches for Harvard. Notable entries include Harvard University in Cambridge, MA. Would you like the enrollment details or the official school website link?

---

**👤 You:**
> "List colleges in the state of 'NY'."

**🤖 AI Agent:**
> I've retrieved the list of schools in New York. Notable entries include NYU, Columbia, and Cornell. I can provide the specific ID and city for each if you'd like.

---

**👤 You:**
> "What is the student size for school ID 166027?"

**🤖 AI Agent:**
> I've identified school ID 166027 as Harvard University. The latest student body size is approximately 7,500 undergraduates. Would you like the full program and cost metadata for this school?


## Installation & Usage

To install and use the **College Scorecard API** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/college-scorecard-api](https://vinkius.com/mcp/college-scorecard-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
