# Adzuna MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/adzuna)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/adzuna-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/adzuna-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Search job listings and salary data — find vacancies and employment trends via AI.

## Description
Connect your **Adzuna** developer account to your AI agent to unlock a powerful job search and labor market intelligence engine. From finding the latest vacancies based on keywords and location to retrieving historical salary data and identifying top employers, your agent handles employment data through natural conversation.

### What you can do

- **Comprehensive Job Search** — Search for thousands of job listings across multiple countries using keywords, Postcodes, and categories
- **Salary Benchmarking** — Retrieve average salary data and distributions (histograms) for specific job roles and locations
- **Employment Trends** — Access historical salary data to monitor how compensation for specific skills changes over time
- **Market Insights** — List top hiring companies and explore geodata to identify regions with the highest job density
- **Career Auditing** — Quickly retrieve job details including descriptions, contract types, and redirect URLs directly from chat

### How it works

1. Subscribe to this server
2. Enter your Adzuna App ID and App Key
3. Start searching for jobs and analyzing salary trends through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Recruiters & HR Specialists** — monitor market salary rates and identify top competitors for talent
- **Job Seekers** — find relevant vacancies and research fair compensation for their skills
- **Economic Researchers** — retrieve historical employment data and salary trends for labor market analysis
- **Career Coaches** — support clients with real-time job market data and geographic salary insights


## Available Tools
- **search_jobs**: You must provide a valid 2-letter country code.

Search for thousands of job vacancies across multiple countries using keywords, Postcodes, and categories
- **get_salary_history**: Retrieve the historical average salary trends over time for a specific job title and country
- **get_salary_histogram**: Retrieve a histogram distribution of current average salaries for a specified search query
- **list_top_companies**: List the top hiring companies and employers based on a specific job category or keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Adzuna** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 'Python Developer' jobs in London."

**🤖 AI Agent:**
> I've found 150 Python Developer vacancies in London. Most roles offer between £60k and £90k. Would you like to see the latest 5 listings or check the salary distribution?

---

**👤 You:**
> "Show me the average salary history for 'Data Scientist' in the US."

**🤖 AI Agent:**
> I've retrieved the salary history for Data Scientists in the US. Over the last 12 months, the average salary has increased by 5%, reaching approximately $135,000. Would you like to see which companies are paying the most?

---

**👤 You:**
> "What are the top hiring companies for 'Sales' roles in Brazil?"

**🤖 AI Agent:**
> Based on current Adzuna data for Brazil, the top companies hiring for Sales roles include major retail chains and tech startups. I've listed the top 5 employers along with their active vacancy counts for you.


## Installation & Usage

To install and use the **Adzuna** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/adzuna](https://vinkius.com/mcp/adzuna)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
