# Adtelligent MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/adtelligent)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/adtelligent-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/adtelligent-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Adtech orchestration — manage DSP campaigns, creatives, and SSP reporting via AI.

## Description
Connect your **Adtelligent** account to your AI agent to unlock professional adtech orchestration. From managing DSP entities like agencies and advertisers to retrieving granular SSP performance statistics, your agent handles your advertising stack through natural conversation.

### What you can do

- **DSP Management** — List and audit agencies, advertisers, and campaigns within your Demand-Side Platform
- **Creative Oversight** — List and retrieve details for ad creatives, including video and static assets
- **SSP Reporting** — Retrieve granular performance reports (impressions, clicks, revenue) sliced by domain, country, or app
- **Segment Management** — Manage audience segments to ensure your targeting is always optimized
- **Real-time Insights** — Quickly identify delivery trends or inventory performance issues directly from chat

### How it works

1. Subscribe to this server
2. Enter your Adtelligent DSP Credentials or SSP Auth Token
3. Start managing your advertising ecosystem through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Ad Ops Specialists** — automate campaign setups and creative audits across multiple agencies
- **Digital Publishers** — monitor SSP inventory performance and revenue trends instantly
- **Marketing Analysts** — retrieve granular reporting data for cross-channel ROI analysis
- **Media Buyers** — audit DSP campaign delivery and manage audience segments using simple commands


## Available Tools
- **list_advertisers**: List DSP advertisers
- **list_campaigns**: List DSP campaigns
- **get_ssp_report**: Requires SSP Auth Token.

Get SSP performance statistics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Adtelligent** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active advertisers in my Adtelligent DSP."

**🤖 AI Agent:**
> I've retrieved the list of advertisers. You have 12 active advertiser accounts, including 'Premium Brand A', 'Tech Solutions', and 'Global Retail'. Would you like to check the active campaigns for any of them?

---

**👤 You:**
> "Show me an SSP performance report for yesterday by domain."

**🤖 AI Agent:**
> I've pulled the SSP statistics for yesterday. Your top-performing domains were 'news-site.com' (500k impressions) and 'blog-network.net' (300k impressions). Total revenue generated was $1,250.

---

**👤 You:**
> "List all audience segments for agency ID 12345."

**🤖 AI Agent:**
> I've retrieved the audience segments for agency 12345. There are 5 segments configured, including 'High Intent Tech Buyers' and 'Frequent Travelers'. Would you like to see the targeting rules for these segments?


## Installation & Usage

To install and use the **Adtelligent** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/adtelligent](https://vinkius.com/mcp/adtelligent)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
