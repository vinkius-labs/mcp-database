# iZooto MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/izooto)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Re-engage website visitors with browser push notifications that bring traffic back and boost page views without email lists.

## Description
Connect your **iZooto** account to any AI agent and take full control of your push notification orchestration and audience efficiency through natural conversation. iZooto provides a powerful platform for web and mobile push engagement, and this integration allows you to retrieve audience metadata, dispatch automated notification campaigns, and monitor real-time performance statistics directly from your chat interface.

### What you can do

- **Campaign & Push Orchestration** â€” Send push notifications to all subscribers or specific segments programmatically to ensure your marketing reach is always synchronized.
- **Audience & Segment Intelligence** â€” Access and monitor your defined audience segments and retrieve detailed reach metadata directly from the AI interface to track growth trends.
- **Engagement & Performance Oversight** â€” Retrieve granular details for campaign clicks, impressions, and CTR using simple AI commands to maintain high-visibility marketing transparency.
- **UTM & Asset Control** â€” Configure UTM parameters and manage notification content via natural language to drive better conversion tracking and asset consistency.
- **Operational Monitoring** â€” Track system responses and manage push schedules to ensure your customer engagement workflows are always optimized.

### How it works

1. Subscribe to this server
2. Enter your iZooto API Token from your general settings
3. Start managing your push notifications from Claude, Cursor, or any MCP-compatible client

No more manual logging into the dashboard for basic campaign checks. Your AI acts as a dedicated marketing coordinator or push notification analyst assistant.

### Who is this for?

- **Marketing Managers** â€” quickly retrieve campaign summaries and monitor audience growth without switching apps.
- **Content Creators** â€” automate the dispatch of new post notifications and track engagement via natural conversation.
- **E-commerce Owners** â€” streamline the retrieval of promotional campaign stats and monitor customer reach directly within the chat.


## Available Tools
- **check_izooto_status**: Verify iZooto API connectivity
- **create_segment**: Create an audience segment
- **get_notification**: Get notification details
- **get_stats**: Get push analytics
- **get_subscriber_count**: Get total subscriber count
- **list_audiences**: List audience overview
- **list_notifications**: List sent notifications
- **list_segments**: List all segments
- **send_push**: Send a push notification
- **send_segment_push**: Send push to a segment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **iZooto** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a push notification: 'Flash Sale — 50% off all items today!'"

**🤖 AI Agent:**
> Push notification sent to 45,200 subscribers. Title: 'Flash Sale'. CTR tracking is live — would you like me to check the delivery stats in a few minutes?

---

**👤 You:**
> "Show push analytics for this month."

**🤖 AI Agent:**
> This month: 28 notifications sent, 1.2M total impressions, 34,500 clicks (2.8% avg CTR). Best performing: 'Weekend Sale' with 4.1% CTR. Would you like to see subscriber growth trends?

---

**👤 You:**
> "How many push subscribers do I have?"

**🤖 AI Agent:**
> You currently have 45,200 active subscribers across all platforms. Desktop: 28,100, Mobile: 17,100. Growth rate: +3.2% this month. Would you like to see segment breakdown?


## ❓ FAQ

**Q: How do I send a push notification via AI?**
Use the `send_push` tool with a title, message body, and optional landing URL. Your notification is delivered instantly to all subscribers.

**Q: Can I target specific audience segments?**
Yes. Use `send_segment_push` to target a specific segment, or create new segments with `create_segment` using custom targeting rules.

**Q: How do I check notification performance?**
Use `get_stats` for aggregate analytics or `get_notification` with an ID to see impressions, clicks, and CTR for a specific notification.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/izooto](https://vinkius.com/mcp/izooto)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **iZooto** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `izooto` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **iZooto** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "izooto": {
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
