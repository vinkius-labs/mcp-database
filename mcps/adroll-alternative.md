# AdRoll MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/adroll-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Retarget customers, launch display ad campaigns, and measure conversion performance across web and social channels.

## Description
Connect your **AdRoll** account to any AI agent and take full control of your digital advertising operations and retargeting workflows through natural conversation.

### What you can do

- **Campaign Orchestration** — List and manage all your advertising campaigns programmatically, retrieving detailed budget settings and high-fidelity operational status in real-time
- **Ad Group & Creative Intelligence** — Access your complete directory of ad groups and creative assets to coordinate your visual marketing strategy across multiple channels
- **Performance Reporting** — Programmatically retrieve real-time metrics including clicks, impressions, and high-fidelity spend data to optimize your ROI directly through your agent
- **Audience Segmentation** — Access and manage your retargeting segments to ensure perfectly coordinated audience targeting and high-fidelity personalized experiences
- **Infrastructure Monitoring** — Access advertisable profile metadata and verify account-level settings directly through your agent for instant operational reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** or **Personal Access Token** from the AdRoll Developer Portal
3. Start managing your advertising performance from Claude, Cursor, or any MCP client

No more manual toggling between complex ad tables or missing spend spikes. Your AI acts as your dedicated ad operations coordinator and performance analyst.

### Who is this for?

- **Marketing Managers** — instantly retrieve campaign performance recaps and monitor spend using natural language commands
- **Growth Advertisers** — orchestrate audience segments and verify creative status without leaving your creative workspace
- **Media Buyers** — automate the retrieval of structured advertising metrics for internal reporting through simple AI queries


## Available Tools
- **get_campaign**: Get campaign details
- **get_report**: Pass report criteria as a JSON string.

Get performance report
- **list_adgroups**: List ad groups for a campaign
- **list_ads**: List all ads for an advertisable
- **list_advertisables**: List all advertisable profiles
- **list_campaigns**: List campaigns for an advertisable
- **list_segments**: List audience segments


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AdRoll** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active advertising campaigns for profil EID '123'."

**🤖 AI Agent:**
> I've retrieved your campaigns. For EID 123, you currently have 5 active campaigns, including 'Spring Sale' and 'Retargeting Global'. Would you like the detailed budget metadata for any of these?

---

**👤 You:**
> "Show the performance report (clicks and spend) for last week."

**🤖 AI Agent:**
> Fetching analytics... Last week, your account reached 120,000 impressions with 1,500 clicks and a total spend of $2,400.00. Shall I retrieve the high-fidelity breakdown by campaign?

---

**👤 You:**
> "List the audience segments for advertisable '123'."

**🤖 AI Agent:**
> Accessing audience graph... I found 10 active segments, including 'Cart Abandoners' and 'VIP Customers'. I've retrieved their current reach and user counts for you. Need help managing any of these targets?


## ❓ FAQ

**Q: How do I find my AdRoll API credentials?**
Log in to the AdRoll Developer Portal, navigate to your dashboard, and generate a Personal Access Token or register an app to obtain your API Key.

**Q: Can I retrieve spend metrics via AI?**
Yes! The `get_report` tool allows your agent to retrieve high-fidelity spend and performance data by providing a JSON criteria object.

**Q: How do I check my advertisable profiles?**
Use the `list_advertisables` tool to retrieve your complete directory of websites and brands managed within your AdRoll account programmatically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/adroll-alternative](https://vinkius.com/mcp/adroll-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AdRoll** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `adroll-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AdRoll** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "adroll-alternative": {
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
