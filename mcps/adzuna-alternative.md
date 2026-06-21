# Adzuna MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/adzuna-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/adzuna-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/adzuna-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Search millions of job advertisements and access real-time labor market analytics, salary trends, and regional vacancy data.

## Description
Connect the **Adzuna** labor market engine to your AI agent to transform how you research careers and analyze employment data. This server provides comprehensive access to one of the world's largest job search engines.

### What you can do

- **Job Search** — Query millions of live job listings by keyword, location, salary, and contract type across global markets using `search_jobs`.
- **Salary Analytics** — Access historical salary data, vacancy trends, and distribution histograms to understand market value with `get_history` and `get_histogram`.
- **Regional Insights** — Drill down into geodata to see which regions have the highest demand for specific skills using `get_geodata`.
- **Employer Leaderboards** — Identify top-hiring companies in any sector or location with `get_top_companies`.
- **Salary Estimation** — Use the `get_jobsworth` tool to predict the market rate for any job title and description based on real-time data.

### How it works

1. Subscribe to this server
2. Enter your Adzuna App ID and App Key
3. Start querying job data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Recruiters & HR Professionals** — Benchmark salaries and track competitor hiring volume in real-time.
- **Job Seekers** — Find the best opportunities and estimate your market value based on current data.
- **Data Analysts & Economists** — Extract labor market trends and regional economic indicators directly into your workflow.


## Available Tools
- **get_categories**: List employment sectors (categories)
- **get_geodata**: Get regional job vacancy data
- **get_histogram**: Get salary histogram data
- **get_history**: Get historical salary and vacancy data
- **get_jobsworth**: Estimate salary for a job (Jobsworth)
- **get_top_companies**: Get top companies by vacancy count
- **get_version**: Get Adzuna API version
- **search_jobs**: Search for job advertisements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Adzuna** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 'Remote React Developer' jobs in the US."

**🤖 AI Agent:**
> I've found several listings for Remote React Developers in the US. The top results include positions at TechFlow and CloudScale, with salaries ranging from $120k to $160k. Would you like to see the full details for any of these?

---

**👤 You:**
> "What is the salary history for 'Data Scientist' in Great Britain?"

**🤖 AI Agent:**
> Accessing historical data for 'Data Scientist' in the GB market... I can see a steady 5% increase in average offered salaries over the last 12 months, with a current peak in vacancy volume in the London area.

---

**👤 You:**
> "Estimate the salary for a 'Senior DevOps Engineer' with skills in 'Kubernetes, AWS, Terraform' in the UK."

**🤖 AI Agent:**
> Based on the title and specific skills provided, the Jobsworth tool estimates a market salary of approximately £85,000 - £105,000 per year for this profile in the UK market.


## Installation & Usage

To install and use the **Adzuna** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/adzuna-alternative](https://vinkius.com/mcp/adzuna-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
