# BLS Jobs — Nonfarm Payrolls & Wages MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bls-jobs-nonfarm-payrolls-wages)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bls-jobs-nonfarm-payrolls-wages-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bls-jobs-nonfarm-payrolls-wages-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Access the definitive source for US employment growth. Query Nonfarm Payrolls, private sector job creation, and average hourly earnings tracked by the BLS Current Employment Statistics (CES) program.

## Description
Connect to the exact datasets used by Wall Street and the Federal Reserve to monitor US Job growth. The Bureau of Labor Statistics Jobs MCP gives your agent direct access to the Current Employment Statistics (CES) program.

### What you can do
- **Nonfarm Payrolls** — Fetch exactly how many jobs were added to the US economy each month.
- **Sector Breakdowns** — Drill down into tech, hospitality, or construction employment trends.
- **Wages & Earnings** — Query the average hourly earnings to monitor wage growth and labor tightness.

### How it works
1. Sign up for a free BLS Developer API Key
2. Provide the key in the settings
3. Ask your AI to parse nonfarm payroll additions or track total average hourly wages over the last 10 years.

### Who is this for?
- **Financial Analysts & Traders** — Build models off the monthly jobs report (NFP)
- **HR Professionals & Recruiters** — Monitor macro labor trends
- **Journalists** — Fact-check employment cycles instantly


## Available Tools
- **get_nonfarm_payrolls**: Key metric for forecasting Federal Reserve interest rate movements.

Get Total Nonfarm Payroll employment (CES0000000001)
- **query_bls**: Use this instead of specific endpoints if you intimately know the underlying numerical code. Up to 50 concurrent lookbacks allowed.

Generic BLS v2 api timeseries query. Requires explicit BLS Series IDs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BLS Jobs — Nonfarm Payrolls & Wages** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What was the total Nonfarm Payroll growth in the last quarter?"

**🤖 AI Agent:**
> 📊 **Nonfarm Payrolls (CES0000000001)**

- **Oct**: +150,000 jobs
- **Nov**: +199,000 jobs
- **Dec**: +216,000 jobs

Total added in Q4: **565,000 jobs**, showing accelerating momentum toward the end of the year.

---

**👤 You:**
> "Show me the average hourly earnings trend for all private workers."

**🤖 AI Agent:**
> 💵 **Average Hourly Earnings (CES0500000003)**

Average hourly earnings for all employees on private nonfarm payrolls rose to **$34.27**. Over the past 12 months, average hourly earnings have increased by **4.1%**, keeping wage growth solidly above the current inflation rate.

---

**👤 You:**
> "Which sector added the most jobs in December?"

**🤖 AI Agent:**
> 📊 **Sector Job Growth (Dec)**

1. **Government**: +52,000 jobs
2. **Leisure and Hospitality**: +40,000 jobs
3. **Health Care**: +38,000 jobs

These three sectors accounted for over 60% of all nonfarm payroll additions that month.


## Installation & Usage

To install and use the **BLS Jobs — Nonfarm Payrolls & Wages** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bls-jobs-nonfarm-payrolls-wages](https://vinkius.com/mcp/bls-jobs-nonfarm-payrolls-wages)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
