# Qichacha / 企查查 MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/qichacha)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/qichacha-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/qichacha-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Leading enterprise data platform in China — search companies, check industrial info, and monitor risks via AI.

## Description
Empower your AI agent to orchestrate your business intelligence and due diligence with **Qichacha** (企查查), the premier enterprise data platform in China. By connecting Qichacha to your agent, you transform complex industrial research, ownership auditing, and risk monitoring into a natural conversation. Your agent can instantly search for companies, retrieve detailed registration metadata, browse shareholder structures, and monitor industrial abnormalities without you ever needing to navigate the comprehensive Qichacha portal. Whether you are conducting B2B lead research or auditing potential partners, your agent acts as a real-time business intelligence assistant, keeping your data accurate and your decisions informed.

### What you can do

- **Enterprise Orchestration** — Fuzzy search for companies and retrieve detailed basic and industrial metadata.
- **Ownership Auditing** — Browse shareholder lists and outward investments to identify corporate structures.
- **Personnel Monitoring** — List main staff and executives to identify key decision-makers within an enterprise.
- **Risk Management** — Retrieve risk indicators, court cases, and industrial abnormalities for any registered company.
- **IP Tracking** — Browse registered trademarks, patents, and copyrights to audit intellectual property assets.

### How it works

1. Subscribe to this server
2. Enter your Qichacha OpenAPI App Key and Secret Key
3. Start managing your business intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales & B2B Leads** — search for potential clients and identify key executives through natural language queries.
- **Legal & Compliance** — conduct due diligence and monitor corporate risks directly from your AI-powered workspace.
- **Business Analysts** — retrieve comprehensive corporate data for market research and competitive analysis.
- **Qichacha Power Users** — integrate your existing industrial research workflows into your AI-driven daily routines.


## Available Tools
- **fuzzy_search**: Enterprise fuzzy search
- **get_account_status**: Get OpenAPI account status
- **get_basic_info**: Get enterprise basic info
- **get_full_details**: Get full enterprise details
- **list_branches**: List company branches
- **list_investments**: List outward investments
- **list_ip**: List intellectual property
- **list_risks**: List enterprise risk info
- **list_shareholders**: List company shareholders
- **list_staff**: List main staff/executives


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Qichacha / 企查查** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for companies named 'Xiaomi' in Qichacha."

**🤖 AI Agent:**
> I've retrieved the search results for 'Xiaomi'. There are several matches, including 'Xiaomi Communications Co., Ltd.' and 'Xiaomi Inc.'. Which one would you like the basic information for?

---

**👤 You:**
> "Show me the shareholder structure for 'Tencent'."

**🤖 AI Agent:**
> I've listed the shareholders for Tencent. The primary owners include MIH TC Holdings and various institutional investors. Would you like a list of Tencent's outward investments as well?

---

**👤 You:**
> "Check for any risk information regarding 'Ant Group'."

**🤖 AI Agent:**
> I've retrieved the risk indicators for Ant Group. There are no critical industrial abnormalities, but there are 3 recent court cases listed. Should I retrieve the details for these cases?


## Installation & Usage

To install and use the **Qichacha / 企查查** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/qichacha](https://vinkius.com/mcp/qichacha)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
