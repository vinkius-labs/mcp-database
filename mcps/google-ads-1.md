# Google Ads MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-ads-1)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Equip your AI agent with direct access to Google Ads — manage search, display, and shopping campaigns, track conversions, and optimize ad spend without opening the Google Ads console.

## Description
Connect **Google Ads** to your AI agent and manage the world's largest advertising platform conversationally.

### What you can do

- **Campaign Management** — List, create, update, and pause search, display, shopping, video, and performance max campaigns.
- **Performance Analytics** — Pull impressions, clicks, CTR, CPC, conversions, conversion value, ROAS, quality score, and search impression share.
- **Keyword Management** — Add, pause, and optimize keywords with bid adjustments, negative keywords, and match type changes.
- **Audience & Targeting** — Manage audience segments, location targeting, demographic adjustments, and remarketing lists.

### How it works

1. Subscribe to the Google Ads integration on the marketplace.
2. Create OAuth credentials in Google Cloud Console (console.cloud.google.com → APIs & Services → Credentials → Create OAuth Client ID).
3. Get your Google Ads Developer Token from your Manager account.
4. Ask your AI agent to manage campaigns, pull reports, or optimize bids.

### Who is this for?

- **PPC Managers** — Monitor and optimize Google Ads campaigns with real-time conversational analytics.
- **E-commerce Brands** — Track shopping campaign ROAS, product group performance, and conversion attribution.
- **Agencies** — Manage multiple client Google Ads accounts from one unified interface.


## Available Tools
- **list_campaigns**: List all Google Ads campaigns
- **get_campaign**: Get campaign performance details
- **list_ad_groups**: List ad groups in a campaign
- **list_ads**: List ads in an ad group
- **list_keywords**: List keywords in a campaign
- **get_account_budget**: Get account budget info
- **get_performance_report**: Get daily performance report
- **list_conversion_actions**: List conversion tracking actions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google Ads** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's my Google Ads spend and ROAS this month?"

**🤖 AI Agent:**
> This month: Total spend: $24,800. Clicks: 38,200. CTR: 4.2%. Avg CPC: $0.65. Conversions: 1,420. Conv value: $98,400. ROAS: 3.97x. Top campaign: 'Brand Search' (12.4x ROAS). Worst: 'Broad Match Discovery' (1.1x).

---

**👤 You:**
> "Which keywords have the lowest quality score?"

**🤖 AI Agent:**
> 5 keywords with quality score below 5: 'cheap software' (QS: 3, CPC: $2.40), 'buy online tool' (QS: 4, CPC: $1.90), 'best app' (QS: 3, CPC: $3.10), 'platform pricing' (QS: 4, CPC: $2.20), 'tool comparison' (QS: 4, CPC: $1.75). Recommendation: improve landing page relevance or pause.

---

**👤 You:**
> "Pause all shopping campaigns with ROAS below 2x."

**🤖 AI Agent:**
> Found 2 shopping campaigns below 2x ROAS. Paused: 'Electronics Clearance' (ROAS: 1.3x, $4,200 spend) and 'Accessories Broad' (ROAS: 1.7x, $1,800 spend). Estimated daily savings: ~$450.


## ❓ FAQ

**Q: How do I get my Google Ads API credentials?**
You need three things:

**1. OAuth Client ID & Secret:**
- Go to **console.cloud.google.com**.
- Navigate to **APIs & Services → Credentials**.
- Click **Create Credentials → OAuth Client ID**.
- Select **Web Application**, add redirect URIs, and copy the **Client ID** and **Client Secret**.

**2. Developer Token:**
- Log in to your Google Ads **Manager Account** (MCC).
- Go to **Tools & Settings → Setup → API Center**.
- Copy your **Developer Token** (start with a test token while pending approval).

**3. Customer ID:**
- Your 10-digit Google Ads account number (visible in the top right of the Google Ads console, formatted as XXX-XXX-XXXX).

Paste all values below.

**Q: Can I manage multiple ad accounts from one agent?**
Yes. If you use a Google Ads Manager account (MCC), your AI agent can access all linked accounts. Simply switch between customer IDs to manage different accounts conversationally.

**Q: Can I optimize keyword bids through my AI agent?**
Yes. Your agent can increase or decrease keyword bids, add negative keywords, change match types, and pause underperforming keywords — giving you full bid management from a single conversation.

**Q: What campaign types are supported?**
All Google Ads campaign types: Search, Display, Shopping, Video (YouTube), App, Discovery, Performance Max, and Smart campaigns. Your AI agent can create and manage any of these types.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-ads-1](https://vinkius.com/mcp/google-ads-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Google Ads** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `google-ads-1` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Google Ads** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "google-ads-1": {
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
