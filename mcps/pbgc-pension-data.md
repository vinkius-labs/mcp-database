# PBGC Pension Data MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pbgc-pension-data)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pbgc-pension-data-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pbgc-pension-data-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access official US Pension Benefit Guaranty Corporation data — query single and multiemployer plans, ERISA 4044 rates, and financial assistance records.

## Description
Connect to the **PBGC (Pension Benefit Guaranty Corporation)** open data repository and empower your AI agent to analyze US pension plan health and regulatory metrics through natural conversation.

### What you can do

- **Single-Employer Plans** — List and filter active plans by EIN, Plan Number, or State to monitor corporate pension landscapes.
- **Multiemployer Plans** — Retrieve comprehensive lists of active multiemployer plans insured by the PBGC.
- **ERISA 4044 Rates** — Access critical interest assumptions (select and ultimate rates) used for determining the present value of annuities.
- **Financial Assistance** — Track and analyze financial assistance payments made by the PBGC to multiemployer plans by fiscal year.

### How it works

1. Subscribe to this server
2. Enter your PBGC Open Data API Key (or public token)
3. Start querying pension datasets directly from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Financial Analysts** — quickly gather data on pension plan premiums and financial assistance trends.
- **Actuaries & Legal Professionals** — retrieve ERISA 4044 interest assumptions for valuation and compliance without manual spreadsheet lookups.
- **Policy Researchers** — analyze the distribution of pension plans across different states and fiscal years.


## Available Tools
- **list_erisa_4044_rates**: Get ERISA 4044 Interest Assumptions
- **list_financial_assistance**: List financial assistance payments
- **list_multiemployer_plans**: List active multiemployer pension plans
- **list_single_employer_plans**: List active single-employer pension plans


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PBGC Pension Data** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active single-employer pension plans in California."

**🤖 AI Agent:**
> I've retrieved the active single-employer plans for California. There are several plans listed, including [Plan Name] (EIN: [Number]). Would you like to see the full list or details for a specific EIN?

---

**👤 You:**
> "What are the ERISA 4044 interest rates for 2023, Q4?"

**🤖 AI Agent:**
> For Q4 2023, the ERISA 4044 select interest rate was [Rate]% and the ultimate rate was [Rate]%. These are used for determining the present value of annuities in terminations.

---

**👤 You:**
> "Show me multiemployer plans insured by PBGC."

**🤖 AI Agent:**
> I've fetched the list of active multiemployer plans insured by PBGC. I found [Number] plans. Notable entries include [Plan A] and [Plan B]. Do you need details on a specific plan?


## Installation & Usage

To install and use the **PBGC Pension Data** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pbgc-pension-data](https://vinkius.com/mcp/pbgc-pension-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
