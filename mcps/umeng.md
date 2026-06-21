# Umeng / 友盟+ MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/umeng)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Leading mobile analytics and push notification platform in China — manage campaigns and audit performance via AI.

## Description
Empower your AI agent to orchestrate your mobile growth and engagement with **Umeng+** (友盟+), the premier mobile infrastructure provider in China. By connecting Umeng to your agent, you transform complex push notification campaigns and deep analytical auditing into a natural conversation. Your agent can instantly send targeted push messages, retrieve real-time delivery status, monitor user retention trends, and even provide high-level application performance summaries without you ever needing to navigate the comprehensive Umeng portal. Whether you are conducting a growth audit or coordinating a cross-functional marketing blast, your agent acts as a real-time mobile operations assistant, keeping your data accurate and your users engaged.

### What you can do

- **Push Orchestration** — Send template-based or custom push notifications and retrieve real-time delivery and click status.
- **User Growth Auditing** — Retrieve detailed metrics for active users, new registrations, and retention across any time period.
- **Behavioral Analysis** — Browse custom event data and session duration statistics to identify user engagement patterns.
- **Task Management** — List recent push tasks and cancel pending operations directly through the agent interface.
- **Performance Insights** — Access high-level application summaries to monitor the health and growth of your mobile ecosystem.

### How it works

1. Subscribe to this server
2. Enter your Umeng App Key and App Master Secret
3. Start managing your mobile operations through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Growth Managers** — monitor user retention and coordinate marketing pushes through natural language queries.
- **Product Operations** — manage push notification lifecycles and audit engagement metrics directly from your AI-powered workspace.
- **Data Analysts** — retrieve system-wide mobile metrics and perform event analysis via a unified AI interface.
- **Umeng Power Users** — integrate your existing mobile workflows into your AI-driven daily routines.


## Available Tools
- **cancel_push**: Cancel pending push task
- **get_active_users**: Get active user count
- **get_app_summary**: Get app analytics summary
- **get_duration_stats**: Get session duration stats
- **get_event_data**: Get custom event data
- **get_new_users**: Get new user registrations
- **get_push_status**: Check push task status
- **get_retention**: Get user retention stats
- **list_push_tasks**: List recent push tasks
- **send_push**: Send push notification


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Umeng / 友盟+** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a broadcast push saying 'Flash Sale starts now!' to all users."

**🤖 AI Agent:**
> I've initiated the broadcast push for you. The task ID is '8821'. I'll monitor the delivery status and let you know once the distribution reaches your user base.

---

**👤 You:**
> "Show me the active user metrics for today."

**🤖 AI Agent:**
> I've retrieved your analytics for today. You currently have 15,200 active users, with a 5% increase compared to yesterday. Your average session duration is 4.5 minutes.

---

**👤 You:**
> "What is the retention rate for users who joined last Monday?"

**🤖 AI Agent:**
> I've calculated the retention stats for that cohort. The Day-7 retention rate for users who joined last Monday is 28.5%, which is slightly above your project average of 25%.


## ❓ FAQ

**Q: How do I find my Umeng App Key and Master Secret?**
Log in to the [Umeng portal](https://www.umeng.com/), select your application from the dashboard, and you will find your App Key and App Master Secret in the application settings under 'App Info'.

**Q: Does Umeng require different keys for iOS and Android?**
Yes. Umeng typically uses separate App Keys for different platforms. Ensure you authorize the correct key depending on which platform's analytics or push notifications you wish to manage.

**Q: Can I cancel a push task through the agent?**
Yes! Use the `cancel_push` tool with the specific task ID. Your agent will communicate with Umeng to stop the delivery of any pending notification broadcast.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/umeng](https://vinkius.com/mcp/umeng)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Umeng / 友盟+** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `umeng` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Umeng / 友盟+** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "umeng": {
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
