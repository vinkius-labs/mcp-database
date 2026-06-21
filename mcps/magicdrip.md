# MagicDrip MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/magicdrip)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/magicdrip-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/magicdrip-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Run LinkedIn outreach campaigns on autopilot with connection requests, follow-ups, and message sequences that feel personal.

## Description
Connect your **MagicDrip** (magicdrip.com) account to any AI agent and take full control of your LinkedIn sales orchestration and automated outreach through natural conversation. MagicDrip provides a powerful platform for scaling B2B social selling, and this integration allows you to retrieve lead metadata, trigger automated connection requests, and monitor campaign performance directly from your chat interface.

### What you can do

- **Lead & Prospect Orchestration** — List all managed leads and retrieve detailed profile metadata programmatically to ensure your sales funnel is always synchronized.
- **Campaign Lifecycle Management** — Access and monitor your automated LinkedIn campaigns and retrieve detailed performance metadata directly from the AI interface.
- **Outreach & Message Intelligence** — Send automated connection requests and direct messages via natural language to drive better engagement and conversion rates.
- **Analytics & Quota Oversight** — Retrieve aggregated account statistics and monitor your available slots and limits using simple AI commands.
- **Operational Monitoring** — Track system responses and manage webhook metadata to ensure your social selling workflows are always optimized.

### How it works

1. Subscribe to this server
2. Enter your MagicDrip Access Token from your dashboard settings
3. Start managing your LinkedIn outreach from Claude, Cursor, or any MCP-compatible client

No more manual connection sending in LinkedIn. Your AI acts as a dedicated sales development rep (SDR) or social selling assistant.

### Who is this for?

- **SDRs & BDRs** — quickly retrieve lead summaries and coordinate follow-ups without switching apps.
- **Growth Managers** — automate the retrieval of campaign metadata and track sequence progress via natural conversation.
- **Founders & Sales Teams** — streamline the ingestion of new leads and monitor organizational growth directly within the chat.


## Available Tools
- **add_linkedin_lead**: Add a new lead to a campaign
- **check_api_health**: Verify The Magic Drip API status
- **get_campaign_performance**: Retrieve campaign analytics
- **get_lead_outreach_details**: Get details for a specific prospect
- **get_authenticated_user_profile**: Get authenticated account info
- **get_account_outreach_stats**: Get overall account performance
- **list_outreach_campaigns**: List LinkedIn automation campaigns
- **list_outreach_leads**: List prospects from outreach campaigns
- **get_available_slots_quota**: Check account daily limits
- **list_configured_webhooks**: g., new reply).

List active webhooks
- **send_linkedin_invite**: Send a connection request
- **send_direct_linkedin_message**: Send a direct LinkedIn message


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MagicDrip** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active sales campaigns in MagicDrip."

**🤖 AI Agent:**
> I've retrieved your campaigns. You have 3 active sequences including 'Q4 Enterprise' and 'Inbound Outreach'. Which one would you like to see lead counts for?

---

**👤 You:**
> "Show me the overall stats for my LinkedIn outreach."

**🤖 AI Agent:**
> I've retrieved your overall analytics. You have sent 450 connection requests this month with a 35% acceptance rate. Would you like to see the response rate for your follow-up messages?

---

**👤 You:**
> "Add 'Sarah Chen' from 'sarah@acme.corp' as a new lead."

**🤖 AI Agent:**
> Sarah Chen has been added as a lead to your database. Which outreach campaign should I assign her to?


## Installation & Usage

To install and use the **MagicDrip** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/magicdrip](https://vinkius.com/mcp/magicdrip)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
