# AirMatch Pro MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/airmatch-pro)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/airmatch-pro-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/airmatch-pro-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Match candidates to job openings with AI-powered recruitment scoring and talent pipeline management for faster hiring.

## Description
Connect your **AirMatch Pro** account to any AI agent and take full control of your HVAC sales engineering and automated proposal workflows through natural conversation.

### What you can do

- **Lead & Proposal Orchestration** — List and manage your entire HVAC sales pipeline programmatically, retrieving detailed technical proposals and customer status
- **Financial Intelligence Sync** — Programmatically monitor and sync sales data with QuickBooks to maintain a perfectly coordinated audit trail for your HVAC business
- **Project Architecture** — Access your complete directory of HVAC installations and maintenance projects to oversee your organizational resource allocation in real-time
- **Engagement Monitoring** — Access real-time lead interaction metadata and track proposal acceptance directly through your agent for instant operational reporting
- **Operational Monitoring** — Verify account-level API connectivity and monitor sales volume directly through your agent for perfectly coordinated firm scaling

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your AirMatch Pro dashboard (Settings > Integrations)
3. Start orchestrating your HVAC sales from Claude, Cursor, or any MCP client

No more manual toggling between sales tools or missing critical follow-ups. Your AI acts as your dedicated sales coordinator and HVAC architect.

### Who is this for?

- **HVAC Business Owners** — instantly retrieve sales recaps and monitor proposal statuses using natural language commands
- **Sales Technicians** — generate and verify HVAC proposals without leaving your creative workspace
- **Operations Leads** — automate the synchronization of sales data with QuickBooks through simple AI queries


## Available Tools
- **check_airmatch_status**: Verify AirMatch Pro API connectivity
- **create_proposal**: Optionally link to an existing customer.

Create a new proposal
- **get_lead**: Get lead details
- **get_profile**: Get your AirMatch Pro profile
- **get_proposal**: Get proposal details
- **list_customers**: List all customers
- **list_estimates**: List all estimates
- **list_jobs**: List all jobs
- **list_leads**: List all leads
- **list_proposals**: List all proposals


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AirMatch Pro** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active proposals for 'John Smith'."

**🤖 AI Agent:**
> I've retrieved the proposals. For John Smith, you currently have 2 active quotes, including 'Central AC Install' (ID: prop_123). Would you like the detailed technical metadata for either of them?

---

**👤 You:**
> "Check the QuickBooks sync status for yesterday's sales."

**🤖 AI Agent:**
> Financial sync orchestrated! I've verified that all 5 sales from yesterday were successfully transmitted to QuickBooks. I've retrieved the transaction IDs for your audit trail. Need help with today's records?

---

**👤 You:**
> "Retrieve the last 5 leads captured in AirMatch Pro."

**🤖 AI Agent:**
> Accessing lead architecture... I've identified the last 5 recent contacts, including @user1 and @user2. All are now active in your sales pipeline. Shall I retrieve the detailed profile metadata for the most recent one?


## Installation & Usage

To install and use the **AirMatch Pro** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/airmatch-pro](https://vinkius.com/mcp/airmatch-pro)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
