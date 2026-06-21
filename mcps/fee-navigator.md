# Fee Navigator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fee-navigator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/fee-navigator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/fee-navigator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Analyze merchant statements via Fee Navigator — track potential savings, generate proposals, and manage audits directly through your AI agent.

## Description
Connect your **Fee Navigator** account to any AI agent and take full control of your merchant statement analysis and proposal workflow through natural conversation.

### What you can do

- **Merchant Orchestration** — List all managed merchants and fetch detailed profiles including current processing metadata natively
- **AI Statement Analysis** — Trigger instant AI-powered analysis for uploaded merchant statements to identify hidden fees flawlessly
- **Proposal Intelligence** — List, inspect, and track savings proposals to optimize your sales pipeline natively
- **Audit Management** — Access detailed statement audits to verify processing costs and potential overcharges synchronously
- **Industry Benchmarking** — Retrieve real-time industry statistics and savings benchmarks to validate your offers flawlessly
- **Document Flow** — Manage statement uploads and tracking statuses directly from the cloud without manual portal navigation
- **Identity Context** — Verify your API token user profile and account information through the agent flawlessly

### How it works

1. Subscribe to this server
2. Enter your Fee Navigator API Token (found in Developer Settings)
3. Start analyzing merchant statements from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Merchant Services ISOs** — automate the ingestion and analysis of statements to speed up the sales cycle
- **Sales Agents** — quickly check potential savings and proposal status while on the go using natural language
- **Payment Analysts** — pull granular fee data and industry benchmarks directly into your AI-powered auditing workflow


## Available Tools
- **analyze_statement**: Trigger AI analysis for an uploaded statement
- **get_account_info**: Get Fee Navigator account details
- **get_audit**: Get details for a specific audit
- **get_industry_stats**: Get merchant service industry savings benchmarks
- **get_me**: Get current API token identity info
- **get_merchant**: Get details for a specific merchant
- **get_proposal**: Get details for a specific proposal
- **list_audits**: List all statement audits
- **list_merchants**: List all merchants in your Fee Navigator account
- **list_proposals**: List all savings proposals
- **list_recent_activities**: List recent merchant analysis activities
- **upload_statement**: Upload a merchant statement for analysis


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fee Navigator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active merchants in my account."

**🤖 AI Agent:**
> I've retrieved your merchants. You have 15 active accounts including 'Joe's Coffee' (ID: m_123) and 'Tech Haven' (ID: m_456). Would you like to see the latest analysis status for joe's Coffee?

---

**👤 You:**
> "Show me the potential savings for proposal P-789."

**🤖 AI Agent:**
> Inspecting proposal P-789... Based on the latest statement analysis, the merchant can save approximately $450 per month by switching to your recommended interchange-plus plan.

---

**👤 You:**
> "Check the current industry savings benchmarks."

**🤖 AI Agent:**
> Retrieving industry stats... Current data shows an average savings of 18.5% across the retail sector and 22% for hospitality merchants when optimizing processing fees.


## Installation & Usage

To install and use the **Fee Navigator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fee-navigator](https://vinkius.com/mcp/fee-navigator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
