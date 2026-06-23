# TopOn / Mobvista MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/topon-mobvista)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Ad mediation and monetization platform for mobile games — monitor revenue, manage waterfalls, and optimize eCPM via AI.

## Description
Empower your AI agent to orchestrate your mobile game monetization with **TopOn / Mobvista**, the leading global platforms for ad mediation and programmatic buying. By connecting TopOn and Mobvista (Mintegral) to your agent, you transform complex performance auditing and waterfall management into a natural conversation. Your agent can instantly list your apps, retrieve real-time revenue reports, analyze eCPM trends, and even audit your placement waterfalls for optimization opportunities without you needing to navigate multiple dashboards. Whether you are an indie developer or part of a large studio, your agent acts as a real-time monetization manager, ensuring your ad revenue is always maximized.

### What you can do

- **Unified Reporting** — Get performance summaries and detailed revenue reports from both TopOn and Mintegral instantly.
- **Waterfall Management** — Browse ad placements and audit waterfall configurations to identify low-performing ad networks.
- **Performance Auditing** — Check the 'health' of your placements and receive AI-driven recommendations for waterfall optimization.
- **Campaign Insights** — Monitor Mintegral offers and app-level statistics to track your user acquisition and monetization synergy.
- **Revenue Trends** — Visualize daily revenue trends and eCPM fluctuations to stay on top of market changes.

### How it works

1. Subscribe to this server
2. Enter your TopOn API Key and Mintegral Skey
3. Start managing your game monetization through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Game Developers** — monitor and optimize your game's ad revenue directly from your AI-powered workspace.
- **Ad Ops Managers** — audit waterfalls and analyze network performance through natural language queries.
- **Product Managers** — track monetization KPIs and eCPM trends across multiple games and regions.
- **UA Specialists** — monitor the synergy between Mintegral campaigns and organic monetization performance.


## Available Tools (8)
- **get_mintegral_app_stats**: Get Mintegral app statistics
- **list_topon_apps**: List TopOn applications
- **list_topon_placements**: List TopOn ad placements
- **get_mintegral_reporting**: Get Mintegral performance reporting
- **get_monetization_summary**: Get overall monetization summary
- **get_topon_reporting**: Get TopOn performance reporting
- **get_topon_waterfall**: Get TopOn placement waterfall
- **list_mintegral_offers**: List Mintegral offers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TopOn / Mobvista** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show my monetization summary for today."

**🤖 AI Agent:**
> Your overall monetization is looking strong today! Total revenue is approximately $1,240.50, up 5% from yesterday. Mintegral contributed the most to this growth. Would you like a breakdown by app?

---

**👤 You:**
> "Check the waterfall health for placement 'ad-unit-772'."

**🤖 AI Agent:**
> I've audited the waterfall for 'ad-unit-772'. The health score is 92/100. All networks are responding well, but I recommend testing Mintegral at the top of the waterfall for your Tier-1 regions to potentially boost eCPM.

---

**👤 You:**
> "List my ad placements for app 'Galaxy Quest'."

**🤖 AI Agent:**
> I found 4 active ad placements for 'Galaxy Quest': 'Main_Menu_Interstitial', 'Rewarded_Double_Coins', 'Level_End_Banner', and 'Offer_Wall'. Which one would you like to analyze?


## ❓ FAQ

**Q: How do I find my TopOn API Key?**
Log in to your TopOn dashboard, go to the [API Tools] section, and you will find your Management and Reporting API keys there.

**Q: Can I audit my waterfalls using this agent?**
Yes! You can use the `check_waterfall_health` tool for a specific placement ID to get an AI-driven audit of your fill rates, latency, and optimization recommendations.

**Q: Is reporting available for both TopOn and Mintegral?**
Yes, this server integrates both TopOn Reporting and Mintegral Reporting V2, allowing you to pull performance data from both sources in one place.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/topon-mobvista](https://vinkius.com/mcp/topon-mobvista)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TopOn / Mobvista** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `topon-mobvista` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TopOn / Mobvista** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "topon-mobvista": {
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
