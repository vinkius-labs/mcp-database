# Onpipeline MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/onpipeline)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/onpipeline-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/onpipeline-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Track deals through your sales pipeline with a visual CRM that focuses on activity-based selling and revenue forecasting.

## Description
Connect your **Onpipeline** account to any AI agent and take full control of your sales orchestration and pipeline management through natural conversation. Onpipeline is a powerful and intuitive CRM designed for high-velocity sales teams, and this integration allows you to retrieve deal metadata, update customer records, and monitor organization history directly from your chat interface.

### What you can do

- **Deal & Opportunity Orchestration** — List all managed deals and retrieve detailed status metadata programmatically to ensure your sales pipeline is always synchronized.
- **Contact & CRM Intelligence** — Access and monitor your centralized database of persons and organizations directly from the AI interface to maintain high-fidelity customer profiles.
- **Pipeline Discovery** — Search through your sales stages and retrieve deal history via natural language to drive better forecasting efficiency.
- **Lead Management Control** — Create new deals, persons, and organization records using simple AI commands to reduce manual data entry.
- **Operational Monitoring** — Track system responses and manage organization-wide activity to ensure your sales workflows are always optimized.

### How it works

1. Subscribe to this server
2. Enter your Onpipeline API Token from your account settings
3. Start managing your sales CRM from Claude, Cursor, or any MCP-compatible client

No more jumping between browser tabs to update a deal's status. Your AI acts as a dedicated sales coordinator or CRM lead.

### Who is this for?

- **Sales Representatives** — quickly retrieve deal summaries and update prospect info without switching apps.
- **Sales Managers** — automate the retrieval of pipeline health metrics and track team activity via natural conversation.
- **Operations Teams** — streamline the retrieval of organization metadata and monitor organizational CRM health directly within the chat.


## Available Tools
- **create_crm_deal**: Create a new deal
- **create_crm_organization**: Create a new organization
- **create_crm_contact**: Create a new contact
- **get_deal_details**: Get details for a specific deal
- **get_contact_details**: Get details for a specific contact
- **list_activities**: List all CRM activities
- **list_crm_deals**: List all sales deals
- **list_crm_events**: List calendar events
- **list_crm_organizations**: List CRM organizations (companies)
- **list_crm_contacts**: List CRM contacts (persons)
- **list_pipelines**: List all sales pipelines


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Onpipeline** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my current deals in Onpipeline."

**🤖 AI Agent:**
> I've retrieved your deals. You have 5 active opportunities including 'Acme Expansion' and 'Global Solutions'. Which one would you like to see the next activity for?

---

**👤 You:**
> "Show me all sales pipelines and their current stage breakdown."

**🤖 AI Agent:**
> You have 2 active pipelines. "B2B Enterprise" has 34 deals across 5 stages: Qualified (8), Discovery (12), Proposal (7), Negotiation (4), and Closing (3). Total pipeline value: $2.4M. "SMB Inbound" has 67 deals across 4 stages with a total value of $890K. Your weighted forecast for this quarter is $1.1M.

---

**👤 You:**
> "Get the full details and activity history for deal ID d_4521."

**🤖 AI Agent:**
> Deal d_4521 "Acme Corp Enterprise License" is in the Proposal stage with a value of $185,000. Owner: Sarah Johnson. Contact: Mark Davis (CTO). Created 23 days ago with 12 logged activities: 4 emails, 3 calls, 2 meetings, and 3 notes. Next scheduled activity: Follow-up call on May 15th at 10 AM.


## Installation & Usage

To install and use the **Onpipeline** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/onpipeline](https://vinkius.com/mcp/onpipeline)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
