# Inform Direct MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/inform-direct)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/inform-direct-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/inform-direct-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

File UK company documents with Companies House digitally and manage statutory records, share registers, and annual filings.

## Description
Connect your **Inform Direct** account to any AI agent and take full control of your UK company secretarial and statutory compliance workflows through natural conversation.

### What you can do

- **Company Portfolio Orchestration** â€” List and manage all companies in your portfolio programmatically, retrieving detailed metadata including company numbers and public URLs
- **Statutory Compliance Intelligence** â€” Programmatically access and monitor statutory registers for directors, shareholders, and PSCs to ensure perfectly coordinated compliance
- **Filings & Reporting Architecture** â€” Track confirmation statement deadlines and Companies House filing statuses to maintain a audit trail of corporate actions
- **Document Library Management** â€” Access and organize minutes, resolutions, and share certificates directly through your agent for perfectly coordinated corporate governance
- **Operational Monitoring** â€” Verify account-level API connectivity and monitor portfolio health directly through your agent for instant performance reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Inform Direct account (Account > Integrations)
3. Start orchestrating your corporate compliance from Claude, Cursor, or any MCP client

No more manual logging into Companies House or secretarial portals to check deadlines. Your AI acts as your dedicated corporate secretary and compliance architect.

### Who is this for?

- **Company Secretaries & Accountants** â€” instantly retrieve company summaries and monitor filing deadlines using natural language commands
- **Legal & Compliance Teams** â€” verify statutory registers and PSC details without leaving your workspace
- **Business Owners** â€” automate the management of their UK company portfolio through simple AI queries


## Available Tools
- **add_company**: Add a company
- **check_informdirect_status**: Verify Inform Direct API connectivity
- **get_account**: Get account info
- **get_company**: Get company details
- **get_filing_status**: Get filing deadlines
- **list_companies**: List all companies
- **list_directors**: List company directors
- **list_filings**: List company filings
- **list_shareholders**: List shareholders
- **remove_company**: This does not affect the company at Companies House.

Remove a company


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Inform Direct** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all companies in my Inform Direct account."

**🤖 AI Agent:**
> You have 8 companies linked. The most recent addition is 'Acme Ltd' (Company No. 12345678). Would you like to see directors or filing status for any of them?

---

**👤 You:**
> "Show me the directors for company 12345678."

**🤖 AI Agent:**
> Company 12345678 has 3 active directors: Jane Smith (appointed 2020-01-15), Robert Brown (2021-06-01), and Sarah Lee (2023-03-10). Would you like to check filing deadlines?

---

**👤 You:**
> "Check filing deadlines for company 12345678."

**🤖 AI Agent:**
> Company 12345678 has its next Confirmation Statement due on June 15, 2026, and Annual Accounts due on September 30, 2026. Both are on track. Would you like to check shareholders too?


## Installation & Usage

To install and use the **Inform Direct** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/inform-direct](https://vinkius.com/mcp/inform-direct)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
