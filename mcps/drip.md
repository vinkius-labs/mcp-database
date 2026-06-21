# Drip MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/drip)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/drip-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/drip-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Automate e-commerce marketing via Drip — manage subscribers, trigger workflows, track custom events, and audit campaigns directly from any AI agent.

## Description
Connect your **Drip** account to any AI agent and take full control of your e-commerce CRM and marketing automation through natural conversation.

### What you can do

- **Subscriber Management** — List and search for subscribers to retrieve emails, tags, custom fields, lead scores, and lifecycle stages natively
- **Provisioning & Tagging** — Create or update subscriber profiles and apply or remove tags strictly to drive your automation and segmentation logic
- **Workflow Orchestration** — List all automation workflows and trigger absolute response routing to start subscribers onto an executing node loop
- **Campaign Auditing** — Retrieve explicit arrays detailing specific email series campaigns, including statuses and subscriber counts
- **Event Tracking** — Inject raw telemetry logs to record custom events (like 'Purchased' or 'Visited') generating hard tracking bindings for your automation
- **Categorical Tagging** — Identify precise active tag arrays spanning your account to manage your organizational segmentation boundaries
- **Activity Monitoring** — Analyze specific localized profiles decoding activity history to understand customer behavior limitlessly

### How it works

1. Subscribe to this server
2. Enter your Drip API Token (found in Settings > User Settings) and Account ID (found in Settings > General Info)
3. Start managing your marketing automation from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Marketers** — trigger workflows and manage subscriber tags without leaving the chat or CRM interface
- **CRM Managers** — audit campaign performance and monitor subscriber lead scores using natural language
- **Growth Engineers** — record custom events and test automation triggers through natural conversation
- **Support Teams** — quickly look up subscriber profiles and tag relationships to resolve customer inquiries in real-time


## Available Tools
- **list_subscribers**: Returns emails, tags, custom fields, and lifecycle stage.

List Drip subscribers. Drip is an e-commerce CRM/email platform
- **get_subscriber**: Returns full profile, tags, custom fields, lead score, and activity history.

Get a Drip subscriber by email or ID
- **create_subscriber**: Modifies `/v2/{account_id}/subscribers` resolving exact tags mapping.

Create or update a Drip subscriber
- **tag_subscriber**: Tags drive automation and segmentation.

Apply a tag to a Drip subscriber
- **remove_tag**: Drops the raw data tag relationship bypassing the standard UI triggers.

Remove a tag from a Drip subscriber
- **list_campaigns**: Returns campaign IDs, names, statuses, and subscriber counts.

List Drip email series campaigns
- **list_workflows**: Returns workflow IDs, names, and statuses (active/paused/draft).

List Drip automation workflows
- **start_workflow**: Starts a subscriber onto an executing node loop.

Start a subscriber on a Drip automation workflow
- **record_event**: Events trigger automations.

Record a custom event for a Drip subscriber
- **list_tags**: List all tags in your Drip account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Drip** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for subscriber info for: hello@example.com"

**🤖 AI Agent:**
> I found the profile for hello@example.com! Tags: 'Customer', 'Newsletter'. Lead Score: 45. Lifecycle Stage: 'Subscriber'. Most recent activity: 'Opened Welcome Email' 2 hours ago. Would you like to add a new tag to this user?

---

**👤 You:**
> "Add tag 'Vip-Customer' to user: user@drip.com"

**🤖 AI Agent:**
> Tag applied! I've added 'Vip-Customer' to user@drip.com. This user will now be included in your VIP segments and any related automation triggers.

---

**👤 You:**
> "List all active automation workflows"

**🤖 AI Agent:**
> Retrieving workflows... I found 5 active automations including 'Post-Purchase Upsell', 'Abandoned Cart Recovery', and 'Welcome Series'. Would you like the ID for any of these to start a subscriber on them?


## Installation & Usage

To install and use the **Drip** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/drip](https://vinkius.com/mcp/drip)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
