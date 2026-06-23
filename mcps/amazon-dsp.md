# Amazon DSP MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/amazon-dsp)
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


## Available Tools (7)
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


## ❓ FAQ

**Q: How do I find my Amazon DSP API credentials?**
You need to create a 'Login with Amazon' application in the Amazon Developer Console to get your Client ID and Client Secret. Then, you generate a Refresh Token. You also need your Advertiser ID.

**Q: How do I choose the correct region?**
Select the region that matches your target marketplace: **NA** (North America - US, CA, MX, BR), **EU** (Europe - UK, DE, FR, IT, ES, etc.), or **FE** (Far East - JP, AU, SG).

**Q: Why do reports take time to generate?**
Amazon Ads reporting API is asynchronous. When you request a report, it returns a `reportId`. You must wait a few moments and use the check status tool to download the data once it's ready.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/amazon-dsp](https://vinkius.com/mcp/amazon-dsp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Amazon DSP** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `amazon-dsp` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Amazon DSP** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "amazon-dsp": {
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
