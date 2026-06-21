# Countly MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/countly)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Manage product analytics via Countly — track user sessions, record custom events, and query deep behavioral metrics directly from your AI agent.

## Description
Connect your **Countly** analytics instance to any AI agent to monitor user behavior and application performance through natural conversation.

### What you can do

- **Session Management** — Start, update, and end user sessions to track engagement duration and active users in real-time.
- **Event Tracking** — Record specific user actions with custom keys, counts, and segmentation data to understand feature usage.
- **User Profiling** — Update user details including names, emails, and custom properties to build comprehensive user journeys.
- **Analytics Querying** — Retrieve aggregated metrics for sessions, users, and countries, or fetch detailed data for specific event keys.
- **Advanced Segmentation** — Utilize the Drill API (Enterprise Edition) to perform complex filtering and deep-dive analysis into your data.

### How it works

1. Subscribe to this server
2. Provide your Countly Server URL and API credentials (App Key, API Key, App ID)
3. Start querying your product data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Product Managers** — monitor KPIs and feature adoption rates without navigating complex dashboards.
- **Data Analysts** — perform quick segmentations and event audits using natural language queries.
- **Growth Teams** — track conversion events and user profile updates to optimize marketing funnels.


## Available Tools (8)
- **begin_session**: Starts a new session for a user
- **end_session**: Ends the current session
- **read_drill**: Perform advanced segmentation and filtering (Enterprise Edition)
- **read_events**: Retrieve data for specific custom events
- **read_metrics**: Retrieve standard metrics like sessions, users, or countries
- **record_events**: Records specific actions within the app
- **update_session**: Extends an existing session
- **update_user_details**: Updates information about a specific user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Countly** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Fetch the session metrics for my application."

**🤖 AI Agent:**
> I've retrieved the session metrics. In the last period, there were 1,250 total sessions with an average duration of 4 minutes and 12 seconds per user.

---

**👤 You:**
> "Record a 'purchase' event for device ID 'user_99' with a sum of 49.99."

**🤖 AI Agent:**
> The 'purchase' event has been successfully recorded for device 'user_99' with the specified value. Countly has acknowledged the data point.

---

**👤 You:**
> "Update user details for device 'dev_123' setting the email to 'test@example.com'."

**🤖 AI Agent:**
> I have updated the profile for device 'dev_123'. The email address is now set to 'test@example.com' in your Countly user database.


## ❓ FAQ

**Q: How can I retrieve aggregated data like total sessions or user counts?**
You can use the `read_metrics` tool. Simply specify the method (e.g., 'sessions' or 'users') to get the aggregated analytics data from your Countly instance.

**Q: Can I record custom user actions with metadata?**
Yes! Use the `record_events` tool. You can provide a device ID and an array of event objects containing keys, counts, and segmentation details to track specific interactions.

**Q: Does this server support advanced filtering for Enterprise users?**
Yes, if you have the Enterprise Edition, you can use the `read_drill` tool to perform complex queries and segmentation using the Drill API.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/countly](https://vinkius.com/mcp/countly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Countly** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `countly` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Countly** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "countly": {
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
