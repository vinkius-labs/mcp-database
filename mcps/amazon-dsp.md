# Amazon DSP MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/amazon-dsp)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/amazon-dsp-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/amazon-dsp-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Demand-Side Platform orchestration — manage display campaigns, audiences, and creatives via AI.

## Description
Connect your **Amazon DSP** (Demand-Side Platform) account to your AI agent to unlock professional programmatic advertising orchestration. From managing display and video campaigns to auditing audience segments and tracking performance reports, your agent handles your programmatic strategy through natural conversation.

### What you can do

- **Campaign Orchestration** — List and manage DSP campaigns (formerly Orders) and monitor their budgets and delivery statuses
- **Ad Group Oversight** — Retrieve details for ad groups (Line Items) to verify targeting and pacing settings
- **Creative Management** — List and audit creative assets associated with your campaigns to ensure brand compliance
- **Audience Targeting** — Retrieve custom audiences and segments used for precise programmatic targeting
- **Performance Reporting** — Request and monitor asynchronous performance reports to analyze impressions, reach, and conversions

### How it works

1. Subscribe to this server
2. Enter your Amazon DSP Client ID, Client Secret, Refresh Token, Region, and Advertiser ID
3. Start managing your programmatic campaigns and monitoring performance through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Programmatic Traders** — automate campaign audits and monitor pacing across multiple DSP ad groups
- **Media Buyers** — retrieve granular performance reports to optimize bidding strategies and maximize reach
- **Marketing Analysts** — generate and fetch asynchronous DSP reports for external data visualization
- **Agency Account Managers** — quickly check campaign delivery statuses and creative assignments directly from chat


## Available Tools
- **list_campaigns**: List DSP campaigns
- **get_campaign_details**: Get campaign metadata
- **list_ad_groups**: List DSP ad groups
- **list_creatives**: List creatives
- **list_audiences**: List audiences
- **request_report**: Request performance report
- **get_report_status**: Check report status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Amazon DSP** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my Amazon DSP campaigns."

**🤖 AI Agent:**
> I've retrieved your advertising campaigns. You have 3 campaigns active. Which campaign's ad groups would you like to review?

---

**👤 You:**
> "Show me the active ad groups for campaign ID '123456'."

**🤖 AI Agent:**
> I've listed the active ad groups for that campaign. There are 2 running ad groups.

---

**👤 You:**
> "Request a DSP performance report for yesterday."

**🤖 AI Agent:**
> I have successfully requested the DSP report for yesterday. Because Amazon generates reports asynchronously, it is currently processing. Would you like me to check its status now?


## Installation & Usage

To install and use the **Amazon DSP** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/amazon-dsp](https://vinkius.com/mcp/amazon-dsp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
