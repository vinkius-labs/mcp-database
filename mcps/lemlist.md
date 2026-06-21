# Lemlist MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lemlist)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/lemlist-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/lemlist-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Equip your AI agent with direct access to Lemlist — manage cold email campaigns, track lead engagement, and automate outreach without opening the Lemlist dashboard.

## Description
Connect **Lemlist** to your AI agent and manage your cold email outreach and lead engagement pipeline conversationally.

### What you can do

- **Campaign Management** — List, create, and monitor email campaigns with open rates, click rates, and reply metrics.
- **Lead Tracking** — Add leads to campaigns, check engagement statuses, and manage lead lists programmatically.
- **Sequence Analytics** — Pull step-by-step performance data for multi-touch email sequences.
- **Activity Feed** — Monitor recent opens, clicks, replies, and bounces across all campaigns.

### How it works

1. Subscribe to the Lemlist integration on the marketplace.
2. Generate an API key from your Lemlist account (Profile → Settings → Integrations → API section → Generate).
3. Ask your AI agent to manage campaigns, track leads, or pull engagement analytics.

### Who is this for?

- **SDR Teams** — Monitor outreach performance and lead engagement without switching between tools.
- **Growth Marketers** — Optimize email sequences based on real-time open, click, and reply data.
- **Agency Owners** — Track multi-client campaign performance from a single conversational interface.


## Available Tools
- **list_campaigns**: List all campaigns
- **get_campaign**: Get campaign details
- **list_leads**: List campaign leads
- **add_lead**: Add lead to campaign
- **delete_lead**: Delete lead from campaign
- **pause_lead**: Pause a lead
- **resume_lead**: Resume a lead
- **get_team**: Get team info


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lemlist** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's the performance of my 'Q2 Outreach' campaign?"

**🤖 AI Agent:**
> Campaign 'Q2 Outreach': 450 leads contacted, 67% open rate, 12% click rate, 8% reply rate, 2% bounce rate. Top performing step: Email #2 (82% open rate). 36 positive replies received.

---

**👤 You:**
> "Add lead sarah@startup.io to the 'Series A Founders' campaign."

**🤖 AI Agent:**
> Lead added: sarah@startup.io → 'Series A Founders' campaign. She will receive the first email in the sequence based on your campaign schedule. Current position: Step 1 of 5.

---

**👤 You:**
> "Who replied to my emails this week?"

**🤖 AI Agent:**
> You received 14 replies this week across 3 campaigns. Positive replies: 9 (64%). Top responders: Mark at Acme Corp (interested in demo), Lisa at DataFlow (requesting pricing), and 7 others.


## Installation & Usage

To install and use the **Lemlist** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lemlist](https://vinkius.com/mcp/lemlist)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
