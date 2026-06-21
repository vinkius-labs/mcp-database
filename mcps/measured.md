# Measured MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/measured)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-intelligence](../categories/business-intelligence.md)

Marketing performance and incrementality analytics via Measured — track ROAS and cross-channel impact.

## Description
Connect your **Measured** account to any AI agent and take full control of your marketing incrementality and performance data through natural conversation.

### What you can do

- **Incrementality Insights** — Access true causal impact scores across all your marketing channels
- **Performance Tracking** — Monitor spend, revenue, and ROAS metrics from over 300 managed integrations
- **Channel Orchestration** — List and inspect performance data for specific channels like Facebook, Google, or Amazon
- **Automated Reporting** — Retrieve performance summaries, insights, and automated reports instantly

### How it works

1. Subscribe to this server
2. Enter your Measured API Key
3. Start managing your marketing intelligence from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_campaign_performance**: Get performance for a specific campaign
- **get_incrementality_scores**: Get incrementality scores across channels
- **get_insights**: Get marketing insights
- **get_performance_by_channel**: Get performance metrics for a specific channel
- **get_performance_summary**: Get a unified performance summary
- **list_channels**: g. Facebook, Google Ads).

List all marketing channels tracked by Measured
- **list_integrations**: List managed integrations
- **list_reports**: List available performance reports


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Measured** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active marketing channels in Measured."

**🤖 AI Agent:**
> Retrieving channels... You have several channels integrated including Facebook Ads, Google Search, and Amazon Advertising.

---

**👤 You:**
> "Show performance for Facebook Ads last month."

**🤖 AI Agent:**
> Fetching performance metrics... For Facebook Ads, spend was $10k with a ROAS of 4.2x and an incrementality score of 0.85.

---

**👤 You:**
> "What are the latest marketing insights?"

**🤖 AI Agent:**
> Querying insights... Measured suggests shifting budget from Retargeting to Brand Search based on recent incrementality trends.


## ❓ FAQ

**Q: How do I find my Measured API Key?**
You can find your API Key in the Measured platform settings or by contacting your Measured Customer Success Manager (CSM).

**Q: What is an incrementality score?**
It measures the true causal impact of your ad spend on business outcomes, going beyond standard last-click attribution.

**Q: Is my marketing data secure?**
Absolutely. Your token is encrypted at rest and injected securely at runtime.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/measured](https://vinkius.com/mcp/measured)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Measured** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `measured` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Measured** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "measured": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
