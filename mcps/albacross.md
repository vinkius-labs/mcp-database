# Albacross MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/albacross)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/albacross-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/albacross-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

B2B intent and reveal intelligence — identify anonymous website visitors and manage leads via AI.

## Description
Connect your **Albacross** account to your AI agent to unlock professional B2B lead generation and intent data orchestration. From identifying anonymous companies visiting your website in real-time to auditing subscriber segments and monitoring automated workflows, your agent handles your account-based marketing strategy through natural conversation.

### What you can do

- **Company Reveal** — Identify detailed firmographic data for any anonymous website visitor using their IP address
- **Lead Management** — List and audit leads (identified companies) across your specific segments and visit dates
- **Segmentation Oversight** — List and retrieve details for your custom segments, including industry and revenue filters
- **Workflow Auditing** — Monitor your automated data exports (Webhooks, CRM sync) and check their operational status
- **Intent Insights** — Quickly identify high-intent visiting companies or identify traffic trends directly from your chat interface

### How it works

1. Subscribe to this server
2. Enter your Albacross API Key
3. Start identifying website visitors and managing your B2B leads through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Teams** — identify which accounts are researching your products and update CRM data for timely outreach
- **Marketing Managers** — audit lead quality and monitor the performance of your intent-based segments
- **Demand Generation Leads** — quickly retrieve lists of high-intent companies for targeted ad campaigns
- **Operations Specialists** — monitor workflow health and ensure identified leads are syncing correctly to your sales stack


## Available Tools
- **identify_company_by_ip**: Identify company by IP
- **list_segments**: List lead segments
- **list_leads**: List identified companies
- **get_lead_details**: Get lead metadata
- **list_workflows**: List active workflows
- **list_industries**: List industry sectors
- **get_account_info**: Get account metadata
- **get_usage_stats**: Get API usage limits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Albacross** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Identify the company for IP address '8.8.8.8'."

**🤖 AI Agent:**
> I've analyzed the IP address 8.8.8.8. It belongs to Google LLC, a technology company headquartered in Mountain View, CA. They have over 10,000 employees and operate in the Internet software and services industry.

---

**👤 You:**
> "List the last 10 leads identified in my 'High Intent' segment."

**🤖 AI Agent:**
> I've retrieved the latest 10 leads from your High Intent segment. Notable visiting companies include 'Innovation Corp' and 'Global Logistics'. Would you like to see the page visit history for any of them?

---

**👤 You:**
> "Check the status of my 'CRM Sync' workflow."

**🤖 AI Agent:**
> I've checked your workflows. The 'CRM Sync' (ID: 12345) is currently active and has successfully synced 15 leads to HubSpot in the last 24 hours. There are no reported errors.


## Installation & Usage

To install and use the **Albacross** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/albacross](https://vinkius.com/mcp/albacross)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
