# Netease Yunxin / 网易云信 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/netease-yunxin)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Massive scale RTC and IM platform — manage user accounts, chat groups, and messaging via AI.

## Description
Empower your AI agent to orchestrate your real-time communication infrastructure with **Netease Yunxin** (网易云信), the premier provider of IM and RTC services in China. By connecting Yunxin to your agent, you transform complex user account management, group/team orchestration, and historical message auditing into a natural conversation. Your agent can instantly create IM accounts, manage chat group memberships, send direct or batch messages, and browse historical sessions without you ever needing to navigate a technical dashboard. Whether you are building an automated community management system or auditing customer interactions, your agent acts as a real-time communication assistant, providing reliable and secure results from a single, unified source.

### What you can do

- **Account Orchestration** — Create, update, and refresh tokens for IM users with full support for unique accids.
- **Messaging Control** — Send direct P2P messages or high-volume batch messages between your user accounts.
- **Group/Team Management** — Create multi-user teams, add or kick members, and audit team configuration details.
- **History Auditing** — Retrieve and browse historical messages between users within specific time ranges.
- **System Monitoring** — Coordinate service status and monitor IM connectivity across your entire application.

### How it works

1. Subscribe to this server
2. Enter your Yunxin AppKey and AppSecret
3. Start managing your IM infrastructure through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Community Managers** — manage large chat groups and moderate user lists through natural language queries.
- **Support Teams** — automate account registration and monitor chat histories directly from your AI-powered workspace.
- **Developers** — integrate professional IM and RTC capabilities into your AI-driven daily routines.
- **Yunxin Power Users** — integrate your existing communication workflows into your AI-driven daily routines.


## Available Tools
- **add_team_member**: Add members to team
- **create_account**: Create IM account
- **create_team**: Create chat group/team
- **get_session_history**: Get chat history
- **get_team_detail**: Get team details
- **kick_team_member**: Remove member from team
- **refresh_user_token**: Refresh user IM token
- **send_batch_message**: Send batch messages
- **send_p2p_message**: Send P2P message
- **update_account**: Update IM account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Netease Yunxin / 网易云信** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a new IM account with accid 'user_8821'."

**🤖 AI Agent:**
> I've successfully created the IM account 'user_8821'. The account is now active and ready for real-time communication. Would you like to set a display name or custom token for this user?

---

**👤 You:**
> "Send a message from 'admin' to 'user_8821' saying 'Welcome to the platform!'."

**🤖 AI Agent:**
> Done! I've sent your P2P message to 'user_8821'. The message has been successfully delivered to the Yunxin IM system. Would you like to check the session history for this pair?

---

**👤 You:**
> "Create a chat team 'Project Alpha' with owner 'admin' and members 'user_01,user_02'."

**🤖 AI Agent:**
> I've created the chat team 'Project Alpha'. The Team ID (TID) is `12345678`. The owner and initial members have been added successfully. Should I send an invitation message to the group now?


## ❓ FAQ

**Q: How do I find my Yunxin AppKey and AppSecret?**
Log in to the [Yunxin Console](https://console.yunxin.163.com/), select your application from the dashboard, and you will find your AppKey and AppSecret in the application details overview.

**Q: What is an accid?**
An accid is a unique account identifier for a user in the Yunxin IM system. It is defined by you during account creation and used for all subsequent user-related operations.

**Q: How does the CheckSum authentication work?**
Yunxin requires a dynamic CheckSum in the HTTP header for every request. This server automatically calculates it for you using the SHA1(AppSecret + Nonce + CurTime) formula, ensuring secure authorized access.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/netease-yunxin](https://vinkius.com/mcp/netease-yunxin)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Netease Yunxin / 网易云信** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `netease-yunxin` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Netease Yunxin / 网易云信** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "netease-yunxin": {
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
