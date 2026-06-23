# Airship MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/airship)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Mobile engagement orchestration — manage push notifications, segments, and channels via AI.

## Description
Connect your **Airship (formerly Urban Airship)** account to your AI agent to unlock professional mobile and web engagement orchestration. From sending targeted push notifications to auditing subscriber segments and managing named user associations across multiple channels, your agent handles your multi-channel communication strategy through natural conversation.

### What you can do

- **Push Orchestration** — Send and monitor push notifications to specific audiences, segments, or all users
- **Segmentation Oversight** — List and retrieve criteria for your audience segments, including tags and attributes
- **Channel Management** — List and audit communication channels (iOS, Android, Web, Email) and retrieve technical metadata
- **User Association** — Manage named users to map multiple devices and channels to a single customer profile
- **Engagement Insights** — Quickly identify active segments or audit delivery statuses directly from your chat interface

### How it works

1. Subscribe to this server
2. Enter your Airship App Key, Master Secret, and Region (US or EU)
3. Start managing your mobile engagement and monitoring delivery through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Managers** — automate high-priority push sends and monitor audience segmentation effortlessly
- **Mobile Product Owners** — audit channel configurations and verify user associations on the fly
- **Growth Specialists** — research segment criteria and manage multi-channel tags for lifecycle marketing
- **Operations Leads** — monitor delivery statuses and manage static lists using simple commands


## Available Tools (10)
- **send_push_notification**: Send a push alert
- **list_segments**: List audience segments
- **get_segment_details**: Get segment criteria
- **list_named_users**: List named users
- **associate_named_user**: Link device to user
- **list_channels**: List app channels
- **get_channel_details**: Get device metadata
- **list_static_lists**: g. CSV uploads) in your account.

List static audiences
- **list_tags**: List audience tags
- **get_push_status**: Check push delivery


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Airship** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a push notification to all users with alert 'Big Sale starting now!'."

**🤖 AI Agent:**
> I've triggered the push notification to all users. The operation ID is 'abc-123-def'. Your message is now being delivered across iOS, Android, and Web channels. Would you like to check the delivery status in a moment?

---

**👤 You:**
> "List all audience segments in my EU project."

**🤖 AI Agent:**
> I've retrieved your segments from the EU region. You have 15 active segments, including 'Premium Subscribers', 'Inactive 30 Days', and 'iOS Users'. Would you like to see the criteria for 'Premium Subscribers'?

---

**👤 You:**
> "Show details for channel ID '12345678-90ab-cdef-1234-567890abcdef'."

**🤖 AI Agent:**
> I've retrieved the metadata for channel 12345678-90ab... It is an Android device registered yesterday. The user is associated with tags 'news_alerts' and 'sports_fan'. Opt-in status is currently 'True'.


## ❓ FAQ

**Q: How do I find my Airship App Key and Master Secret?**
Log in to the Airship dashboard, go to **Settings** > **APIs & Integrations**, and select **Tokens**. You will find your App Key and can generate/view your Master Secret there.

**Q: Which region should I choose?**
Choose **US** if your project is hosted on `go.urbanairship.com` or **EU** if it is hosted on `go.airship.eu`. Using the wrong region will result in authentication failures.

**Q: Can I target specific users by their email?**
Yes! Use the `send_push_notification` tool and specify the `named_user` in the audience. If your user's email is mapped as their Named User ID, Airship will deliver the push to all their associated devices.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/airship](https://vinkius.com/mcp/airship)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Airship** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `airship` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Airship** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "airship": {
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
