# AdButler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/adbutler-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Serve and manage display ads, track impressions, and optimize ad zones across your digital properties with precision.

## Description
Connect your **AdButler** account to any AI agent and take full control of your ad server orchestration and automated display advertising through natural conversation.

### What you can do

- **Campaign & Ad Portfolio Orchestration** — List and manage your entire high-fidelity portfolio of advertisers and campaigns programmatically, retrieving detailed technical metadata
- **Banner & Creative Intelligence** — Programmatically retrieve directories of banners and access complete high-fidelity asset metadata to coordinate your organizational broadcasting
- **Performance Architecture Monitoring** — Access real-time status updates for active banners and track impression/click metrics directly through your agent
- **Metadata Management** — Programmatically retrieve high-fidelity zone IDs and publisher metadata to maintain a perfectly coordinated ad inventory record
- **Operational Monitoring** — Verify account-level API connectivity and monitor orchestration volume directly through your agent for perfectly coordinated service scaling

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your AdButler dashboard (Settings > API Access)
3. Start orchestrating your ad growth from Claude, Cursor, or any MCP client

No more manual checking of individual banner performance or missing campaign expiration alerts. Your AI acts as your dedicated ad coordinator and inventory architect.

### Who is this for?

- **Ad Ops Managers** — instantly retrieve campaign summaries and monitor ad health using natural language commands
- **Publishers** — verify individual zone metadata and track inventory filling without leaving your creative workspace
- **Developers** — integrate high-speed AdButler data into custom dashboards and reporting tools through simple AI queries


## Available Tools
- **check_adbutler_status**: Verify AdButler API connectivity
- **get_advertiser**: Get advertiser details
- **get_campaign**: Get campaign details
- **get_stats**: Get ad serving statistics
- **list_advertisers**: List all advertisers
- **list_banners**: List ad items in a campaign
- **list_campaigns**: List all campaigns
- **list_placements**: List all placements
- **list_publishers**: List all publishers
- **list_zones**: List all ad zones


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AdButler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active advertisers in my AdButler account."

**🤖 AI Agent:**
> I've retrieved your advertisers. You currently have 10 active high-fidelity profiles, including 'Global Brands' and 'Local Retailer'. Would you like the detailed campaign metadata for any of them?

---

**👤 You:**
> "Show the performance for 'Banner A' from yesterday."

**🤖 AI Agent:**
> Ad intelligence orchestrated! For Banner A, I've identified 1,000 high-fidelity impressions and 50 clicks (CTR: 5%) from yesterday. I've retrieved the technical delivery metadata for your review. Need help auditing the conversion rate?

---

**👤 You:**
> "Check for any campaigns expiring this week."

**🤖 AI Agent:**
> Operational monitoring orchestrated! I've identified 2 high-fidelity campaigns expiring this week, including 'Summer Sale' on Friday. I've retrieved the advertiser contact metadata for your review. Shall I notify the ad ops team?


## ❓ FAQ

**Q: How do I find my AdButler API Key?**
Log in to your account, navigate to **Settings** > **API Access**, and copy your unique API Key from the credentials section.

**Q: Can I check ad performance via AI?**
Yes! The `get_stats` tool retrieves impression and click data for all your active banners and campaigns.

**Q: How do I list my advertisers?**
Use the `list_advertisers` tool to retrieve all advertiser profiles with their unique identifiers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/adbutler-alternative](https://vinkius.com/mcp/adbutler-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AdButler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `adbutler-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AdButler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "adbutler-alternative": {
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
