# Salary.com API MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/salarycom-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/salarycom-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/salarycom-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Access salary benchmarks — audit compensation and jobs via AI.

## Description
Empower your AI agent to orchestrate your entire compensation research and career auditing workflow with **Salary.com**, the authoritative source for salary data. By connecting the Salary.com API to your agent, you transform complex benchmark lookups into a natural conversation. Your agent can instantly retrieve salary ranges for thousands of job titles, audit market trends, and search for open positions without you ever touching a technical portal. Whether you are managing payroll budgets or planning your next career move, your agent acts as a real-time compensation analyst, ensuring your data is always grounded in verified, high-quality market records.

### What you can do

- **Compensation Auditing** — Retrieve high-resolution salary benchmarks for any job title and location, including base salary and percentile metadata.
- **Job Oversight** — Search for open job positions and retrieve detailed descriptions and requirements to maintain a clear view of the market.
- **Trend Intelligence** — Query salary market trends to understand the trajectory of compensation for specific roles instantly.
- **Career Discovery** — List all available job categories in the Salary.com catalog to identify relevant paths for your research.
- **Operational Monitoring** — Check API status to ensure your compensation research workflow is always operational.

### How it works

1. Subscribe to this server
2. Enter your Salary.com API Key
3. Start managing your compensation intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **HR Managers & Recruiters** — monitor salary benchmarks and retrieve competitive metadata straight from your workflow.
- **Compensation Analysts** — verify market trends and audit job distributions without manual database searches.
- **Job Seekers** — perform rapid audits of salary ranges and identify high-paying roles through natural language.
- **Operations Leads** — automate compensation data querying to orchestrate cross-functional people teams smoothly.


## Available Tools
- **check_api_status**: com API is operational.

Check if the Salary.com API is operational
- **get_job_details**: Get full details for a specific job ID
- **get_salary_benchmark**: Get salary benchmarks for a job title and location
- **get_salary_market_trends**: Get market salary trends for a specific job title
- **list_job_categories**: List all available job categories
- **search_jobs**: Search for open jobs by keyword and location


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Salary.com API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the average salary for a 'Product Manager' in 'Austin, TX' using Salary.com?"

**🤖 AI Agent:**
> I've retrieved the salary benchmark for a Product Manager in Austin. The median base salary is approximately $120,000. Would you like the full percentile breakdown or market trends for this role?

---

**👤 You:**
> "Find open 'Software Engineer' jobs in 'San Francisco'."

**🤖 AI Agent:**
> I've identified 10 open Software Engineer roles in San Francisco. Companies hiring include major tech firms and innovative startups. Would you like the specific requirements for the top matches?

---

**👤 You:**
> "Show salary trends for 'Data Scientist' roles."

**🤖 AI Agent:**
> I've retrieved the market trends for Data Scientists. Salaries have seen a steady increase of 5% over the last year due to high demand. I can provide the trajectory metadata for different experience levels if you'd like.


## Installation & Usage

To install and use the **Salary.com API** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/salarycom-api](https://vinkius.com/mcp/salarycom-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
