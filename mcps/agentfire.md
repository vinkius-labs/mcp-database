# AgentFire MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/agentfire)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/agentfire-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/agentfire-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Build high-converting real estate websites, manage property listings, and capture leads for your brokerage with ease.

## Description
Connect your **AgentFire** account to any AI agent and take full control of your real estate website and automated lead capture workflows through natural conversation.

### What you can do

- **Lead Portfolio Orchestration** — List and manage all captured property inquiries programmatically, retrieving detailed lead profile metadata and contact tags
- **Web Engagement Intelligence** — Programmatically monitor property clicks and access engagement metadata to coordinate your sales follow-up strategy
- **Property Graph Monitoring** — Access real-time updates for active listings and track user interaction duration directly through your agent for instant reporting
- **Metadata Management** — Programmatically retrieve interest signals and search history to maintain a perfectly coordinated CRM record
- **Operational Monitoring** — Verify account-level API connectivity and monitor lead capture volume directly through your agent for perfectly coordinated service scaling

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your AgentFire dashboard (Integrations > REST API)
3. Start orchestrating your real estate growth from Claude, Cursor, or any MCP client

No more manual logging into WordPress or missing critical property inquiries. Your AI acts as your dedicated marketing coordinator and real estate architect.

### Who is this for?

- **Real Estate Agents** — instantly retrieve lead summaries and monitor property interest using natural language commands
- **Marketing Leads** — verify individual lead engagement and track web conversions without leaving your workspace
- **Developers** — integrate high-speed AgentFire data into custom automation workflows through simple AI queries


## Available Tools
- **check_agentfire_status**: Verify AgentFire API connectivity
- **create_lead**: Email is required.

Create a new lead
- **get_lead**: Get lead details
- **get_listing**: Get listing details
- **get_profile**: Get your AgentFire profile
- **list_contacts**: List all contacts
- **list_leads**: List all leads
- **list_listings**: List all property listings
- **search_listings**: Search property listings
- **update_lead**: Only provided fields are changed.

Update a lead


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AgentFire** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all new leads captured in AgentFire this week."

**🤖 AI Agent:**
> I've retrieved your leads. You currently have 10 new profiles, including 'John Doe' and 'Jane Client'. Would you like the detailed engagement metadata for any of them?

---

**👤 You:**
> "Show the property interest for lead ID 'lead_123'."

**🤖 AI Agent:**
> Engagement intelligence orchestrated! For lead 123, I've verified that they clicked on 'Modern Villa' (ID: prop_789) 5 times today. I've retrieved the search history for your review. Need help preparing a property walkthrough?

---

**👤 You:**
> "Check for any active listings with zero engagement this month."

**🤖 AI Agent:**
> Listing directory orchestrated! I've identified 3 active listings with zero clicks this month, including 'Condo B' and 'Industrial Loft'. I've retrieved the technical status for your review. Shall I check for any pending content updates for these listings?


## Installation & Usage

To install and use the **AgentFire** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/agentfire](https://vinkius.com/mcp/agentfire)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
