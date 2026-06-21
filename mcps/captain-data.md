# Captain Data MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/captain-data)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/captain-data-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/captain-data-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Automate web data extraction via Captain Data — find and enrich people and company profiles directly from any AI agent.

## Description
Connect your **Captain Data** account to any AI agent and orchestrate your lead generation, market research, and data enrichment workflows through natural conversation.

### What you can do

- **People Discovery** — Find specific professionals by name and company, or search by job titles and locations.
- **Profile Enrichment** — Retrieve detailed LinkedIn profile data, including contact information and career history, using UIDs or URLs.
- **Company Research** — Find companies by name or domain and retrieve deep firmographic data.
- **Automation Oversight** — List and monitor automation jobs and workflows directly from your workspace.
- **Quota Management** — Retrieve real-time API quotas and usage statistics to ensure your operations are on track.
- **Data Retrieval** — Access extracted data from previous jobs using natural language.

### How it works

1. Subscribe to this server
2. Enter your Captain Data API Key
3. Start extracting market intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales & SDR Teams** — quickly find and enrich lead data without manual scraping or dashboard work.
- **Growth Marketers** — automate market research and competitor analysis straight from their workflow tools.
- **Data Analysts** — gather structured intelligence on companies and professionals using natural language.


## Available Tools
- **enrich_company**: Get deep firmographic data for a company
- **enrich_person**: Get detailed profile data for a person using their UID or LinkedIn URL
- **find_company**: Find a company by name or domain
- **find_people**: Find a specific person by full name and optionally company name
- **get_account_info**: Retrieve core account information
- **get_job_details**: Get status and extracted data for a specific job
- **get_api_quotas**: Retrieve current API quotas and usage
- **list_automation_jobs**: List all automation jobs
- **list_workflows**: List all configured workflows
- **search_companies**: Search for companies by industry, size, or location
- **search_people**: Search for people based on criteria like job title or location


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Captain Data** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find people with the name 'Satya Nadella' at 'Microsoft'."

**🤖 AI Agent:**
> I've found the professional profile for Satya Nadella at Microsoft. UID: pers_123. Would you like to enrich this profile to see more details?

---

**👤 You:**
> "Search for companies in the 'Software' industry located in 'California'."

**🤖 AI Agent:**
> Retrieving companies... I found several software companies in California, including 'Google' (Mountain View) and 'Salesforce' (San Francisco).

---

**👤 You:**
> "Enrich the company profile for the domain 'vinkius.com'."

**🤖 AI Agent:**
> Enrichment complete for Vinkius. They are a high-growth tech company specialized in AI and Edge computing, with 50-100 employees.


## Installation & Usage

To install and use the **Captain Data** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/captain-data](https://vinkius.com/mcp/captain-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
