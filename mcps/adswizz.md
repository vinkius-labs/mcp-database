# AdsWizz MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/adswizz)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/adswizz-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/adswizz-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Audio advertising platform — manage campaigns, inventory, and targeting via AI.

## Description
Connect your **AdsWizz** account to your AI agent to orchestrate your digital audio advertising ecosystem. From managing programmatic audio campaigns to auditing publisher inventory and setting up precise targeting, your agent handles the AudioServe and AudioMatic workflows through natural conversation.

### What you can do

- **Campaign Orchestration** — List, retrieve, and monitor audio advertising campaigns across your network
- **Inventory Management** — Audit active zones and publisher placements to ensure optimal ad delivery
- **Targeting Oversight** — Retrieve and verify targeting parameters (geo, device, behavioral) for specific campaigns
- **Reporting & Analytics** — Access aggregated performance reports including impressions, listens, and completion rates
- **Creative Verification** — List ad creatives and verify companion banner configurations for interactive audio ads

### How it works

1. Subscribe to this server
2. Enter your AdsWizz Instance URL and API Key
3. Start managing your audio ad ecosystem through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Ad Ops Managers** — automate audio campaign audits and inventory health checks
- **Programmatic Audio Buyers** — monitor DSP performance and optimize targeting strategies instantly
- **Podcast Networks & Publishers** — audit zone fill rates and SSP monetization performance
- **Marketing Analysts** — retrieve audio engagement metrics for cross-channel reporting


## Available Tools
- **list_campaigns**: List audio ad campaigns
- **get_campaign**: Get campaign details
- **list_zones**: g. podcasts, streams).

List ad zones/inventory
- **get_audio_performance**: Filterable by date.

Get audio ad metrics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AdsWizz** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active audio campaigns."

**🤖 AI Agent:**
> I've retrieved your campaigns. You currently have 8 active audio campaigns, including 'Summer Streaming Promo' and 'Podcast Sponsorship A'. Which one would you like to inspect?

---

**👤 You:**
> "Retrieve the targeting details for campaign ID 45678."

**🤖 AI Agent:**
> I've fetched the details for campaign 45678. It is currently targeting users in North America and Europe, specifically on iOS devices, with a frequency cap of 3 ads per user per day.

---

**👤 You:**
> "List the ad zones available for my publisher account."

**🤖 AI Agent:**
> I've retrieved your ad zones. You have 12 active zones configured, primarily pre-roll and mid-roll slots for your main podcast network. Would you like to check the fill rate for any specific zone?


## Installation & Usage

To install and use the **AdsWizz** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/adswizz](https://vinkius.com/mcp/adswizz)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
