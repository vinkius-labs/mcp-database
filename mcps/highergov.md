# HigherGov MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/highergov)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/highergov-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/highergov-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Find and track government contracts, grants, and procurement opportunities with intelligence built for public sector vendors.

## Description
Connect your **HigherGov** account to any AI agent and take full control of your government market research and procurement tracking through natural conversation.

### What you can do

- **Opportunity Discovery** — Search for federal, state, and local government contract opportunities using precise keywords and filters
- **Award Analysis** — Analyze past contract and grant awards to understand market trends, competitor performance, and agency spending
- **Entity Research** — Research detailed profiles of awardees, government agencies, and key decision-makers programmatically
- **Document Extraction** — Access and retrieve opportunity documents, attachments, and solicitations directly through your agent
- **Market Monitoring** — Track upcoming solicitations and follow specific agencies or industries for real-time intelligence

### How it works

1. Subscribe to this server
2. Retrieve your API Key from the HigherGov dashboard (Settings > API)
3. Start uncovering government opportunities from Claude, Cursor, or any MCP client

No more manual searching through fragmented government portals. Your AI acts as your dedicated B2G market analyst.

### Who is this for?

- **Government Contractors** — instantly identify relevant RFPs and solicitations matching your core capabilities
- **Market Analysts** — perform deep-dive competitor research and agency spending analysis through automated queries
- **Business Development Leads** — track procurement pipelines and find key agency contacts without leaving your workspace


## Available Tools
- **get_agency**: Get agency details
- **get_awardee**: Get awardee details
- **get_contract**: Get contract award details
- **get_documents**: Get opportunity documents
- **get_grant**: Get grant award details
- **get_opportunity**: Get opportunity details
- **list_agencies**: List government agencies
- **list_awardees**: List awardees (companies/orgs)
- **list_contracts**: List government contract awards
- **list_grants**: List government grant awards
- **list_opportunities**: List government contract opportunities
- **search_by_id**: Search using a HigherGov Search ID


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HigherGov** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all current federal opportunities related to 'Cybersecurity' in Washington."

**🤖 AI Agent:**
> Searching federal solicitations... I found 3 active opportunities for 'Cybersecurity' in WA. The largest is a NIST solicitation for 'Zero Trust Architecture Support' (ID: NIST-2026-001). Would you like to see the document list for this RFP?

---

**👤 You:**
> "Show me recent contract awards for 'Lockheed Martin'."

**🤖 AI Agent:**
> Retrieving Lockheed Martin awards... In the last quarter, they were awarded 5 major contracts totaling $1.2B, primarily with the DoD. Notable projects include 'F-35 Sustainment' and 'Satellite Navigation Upgrades'. Should I detail the agency spend for these?

---

**👤 You:**
> "List all grant awards in the state of 'Florida' for 2026."

**🤖 AI Agent:**
> Scanning grant awards for Florida... I found 12 awarded grants so far in 2026. The most frequent agency is HHS, focusing on 'Community Health' and 'Infrastructure Development'. Would you like the list of recipient organizations?


## Installation & Usage

To install and use the **HigherGov** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/highergov](https://vinkius.com/mcp/highergov)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
