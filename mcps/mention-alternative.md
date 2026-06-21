# Mention MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mention-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Monitor brand mentions across the web, social media, and news in real time to protect your reputation and spot trends early.

## Description
Connect your **Mention** account to any AI agent and manage brand monitoring through natural conversation.

### What you can do

- **Brand Monitoring** — Track mentions across social media, blogs, and news
- **Alert Management** — Create and configure keyword monitoring alerts
- **Sentiment Analysis** — Analyze the sentiment (positive/negative) of mentions
- **Social Listening** — Browse recent mentions and filter by source or language
- **Competitor Tracking** — Monitor competitor share of voice

### How it works

1. Subscribe to this server
2. Enter your Mention Access Token and Account ID
3. Start monitoring your brand from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **PR Teams** — track media coverage and brand reputation
- **Marketing** — monitor campaign hashtags and social engagement
- **Customer Support** — identify unhappy customers complaining online


## Available Tools (12)
- **create_monitoring_alert**: Add new alert
- **remove_monitoring_alert**: Delete an alert
- **favorite_mention**: Mark as favorite
- **get_alert_details**: Get alert info
- **get_my_profile**: Get account info
- **get_mention_content**: Read mention details
- **get_alert_statistics**: Check reach metrics
- **list_monitoring_alerts**: List your alerts
- **list_recent_mentions**: List findings
- **list_active_webhooks**: Get event configs
- **mark_mention_as_read**: Mark as seen
- **search_mentions_by_keyword**: Find mentions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mention** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show recent mentions for the 'Vinkius Launch' alert."

**🤖 AI Agent:**
> Alert 'Vinkius Launch': 145 mentions in 24h. Sources: Twitter (89), News (34), Blogs (22). Sentiment: 78% Positive 🟢, 20% Neutral ⚪, 2% Negative 🔴. Top mention: TechCrunch article ('Vinkius redefines AI agents').

---

**👤 You:**
> "List all active alerts and their mention volumes."

**🤖 AI Agent:**
> Active Alerts: 4. 1) 'Brand Name' (1,240 mentions/week). 2) 'Competitor X' (3,400 mentions/week). 3) '#IndustryConf2024' (890 mentions). 4) 'CEO Name' (45 mentions). Total volume: 5,575. Unread mentions: 342.

---

**👤 You:**
> "Show negative mentions from the last 2 days."

**🤖 AI Agent:**
> Found 12 negative mentions. 1) @user (Twitter): 'Support is taking too long to reply.' 2) Reddit (/r/saas): 'Pricing update is confusing.' 3) Blog review: 'Great features, but UX needs work.' Would you like to read the full Reddit thread?


## ❓ FAQ

**Q: Can I monitor specific keywords and brands?**
Yes. Create alerts with boolean queries to track specific brand names, competitors, or industry hashtags.

**Q: How does Mention authentication work?**
Mention requires both an **Access Token** (Bearer) and an **Account ID** against `api.mention.net/api/v1`.

**Q: Does Mention provide sentiment analysis?**
Yes. Mentions are automatically tagged with positive, negative, or neutral sentiment scores.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mention-alternative](https://vinkius.com/mcp/mention-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mention** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mention-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mention** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mention-alternative": {
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
