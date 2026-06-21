# FeedBlitz MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/feedblitz)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage mailing lists, RSS feeds, and email marketing campaigns through AI.

## Description
### What you can do
- Retrieve detailed publisher user profiles and account metrics.
- Manage syndications, feeds, and active mailing lists effortlessly.
- Monitor engagement metrics for any selected syndication.
- Add, retrieve, or remove subscribers dynamically with AI Agents.

### How it works
1. Subscribe to FeedBlitz and configure your lists.
2. Obtain your API Key from the developer settings.
3. Provide the key to the AI Agent to securely automate your email marketing.

### Who is it for?
Designed for email marketers, content creators, and growth hackers who rely on FeedBlitz to automate and scale their communications. Perfect for those using Claude or Cursor to build custom marketing workflows.


## Available Tools
- **add_subscriber**: Add a subscriber to a syndication in FeedBlitz
- **get_subscriber**: Get a specific subscriber from FeedBlitz
- **get_syndication**: Get details for a specific syndication in FeedBlitz
- **get_user**: Get user details from FeedBlitz
- **list_metrics**: List metrics for a syndication in FeedBlitz
- **list_subscribers**: Optionally filter by status.

List subscribers for a syndication in FeedBlitz
- **list_syndications**: List syndications (feeds/lists) in FeedBlitz
- **remove_subscriber**: Remove or unsubscribe a subscriber from FeedBlitz


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FeedBlitz** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my syndications in FeedBlitz."

**🤖 AI Agent:**
> I've fetched your syndications. You currently have 3 active lists: 'Main Newsletter', 'Blog RSS Feed', and 'Product Updates'.

---

**👤 You:**
> "Add newuser@example.com to syndication ID 123."

**🤖 AI Agent:**
> Successfully added newuser@example.com to the syndication with ID 123.

---

**👤 You:**
> "Show me the metrics for syndication ID 123."

**🤖 AI Agent:**
> Here are the metrics for syndication 123: 500 active subscribers, 12 recent unsubscriptions, and an open rate of 42%.


## ❓ FAQ

**Q: Can the AI Agent send bulk email campaigns directly?**
No, the agent currently focuses on managing lists, syndications, and subscribers. Campaigns are typically dispatched automatically via RSS by FeedBlitz.

**Q: Does the FeedBlitz MCP support filtering subscribers by status?**
Yes, you can instruct the AI to filter subscribers by providing a specific status like active or unsubscribed when querying a syndication.

**Q: Are metrics retrieved in real-time?**
Metrics reflect the latest data available in FeedBlitz's systems, providing near real-time insights into your syndication's performance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/feedblitz](https://vinkius.com/mcp/feedblitz)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FeedBlitz** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `feedblitz` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FeedBlitz** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "feedblitz": {
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
