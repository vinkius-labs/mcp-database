# Franchimp MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/franchimp)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/franchimp-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/franchimp-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Access franchise intelligence, lead gen data, and FDD metadata via AI agents with Franchimp.

## Description
Connect your **Franchimp** account to any AI agent to automate your franchise market research and B2B lead generation through the Model Context Protocol (MCP). Franchimp provides access to an extensive database of franchisors and franchisees, including financial requirements, investment ranges, and contact details for over 450,000+ units. This MCP server enables you to retrieve granular franchise metadata and oversee your data credits directly through natural conversation.

### What you can do

- **Franchise Discovery** — Search for franchisors by name or keywords and fetch detailed metadata including status and investment range.
- **Lead Generation** — Access and list franchisee contact information, including emails and phone numbers, to fuel your outreach sequences.
- **FDD Metadata** — List and retrieve metadata for Franchise Disclosure Documents (FDDs) to understand legal and operational structures.
- **Multi-Unit Insights** — Identify and list multi-unit franchisors managing several units across different brands.
- **Credit Management** — Monitor your account status and remaining document download credits directly from your chat interface.
- **Intelligence Research** — Fetch financial stats and investment requirements to benchmark different franchise opportunities.
- **Real-time Monitoring** — Search for specific franchisees by email to verify records or enrich your internal CRM data.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Franchimp API Key (request via admin@franchimp.com)
3. Start managing your franchise intelligence from Claude, Cursor, or any MCP client

### Who is this for?

- **Sales & B2B Marketers** — quickly pull franchisee contact lists or verify leads without leaving your primary agent.
- **Market Researchers** — get a real-time overview of franchisor investment requirements and financial benchmarks.
- **Business Consultants** — automate the gathering of FDD metadata and franchise stats for client advisory reports.


## Available Tools
- **get_account_info**: Get account attributes
- **get_fdd_metadata**: Get FDD information
- **get_investment_stats**: Get investment data
- **get_franchise_details**: Get franchisor metadata
- **get_franchisee_details**: Get franchisee contact info
- **list_available_credits**: Check document credits
- **list_fdd_documents**: List disclosure documents
- **list_franchisees**: List specific franchisees
- **list_franchises**: List all franchisors
- **list_multi_unit_operators**: List multi-unit franchisors
- **find_franchisee_by_email**: Search franchisee by email
- **search_franchisors**: Search franchisor database


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Franchimp** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all franchisors in the database and their investment status."

**🤖 AI Agent:**
> Retrieving franchisors... I found a comprehensive list including brands like 'McDonald\'s' and 'Subway'. Would you like the specific investment requirements for any of them?

---

**👤 You:**
> "Search for franchisees with the email 'john.owner@example.com'."

**🤖 AI Agent:**
> Searching database... I found a franchisee record for John Owner. He manages 2 units in the Florida region. Would you like his phone number?

---

**👤 You:**
> "Show me the investment stats for '7-Eleven'."

**🤖 AI Agent:**
> Retrieving financial data... For 7-Eleven, the total investment range is between $37K and $1.6M, with a net worth requirement of $50K - $250K. Would you like more details?


## Installation & Usage

To install and use the **Franchimp** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/franchimp](https://vinkius.com/mcp/franchimp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
