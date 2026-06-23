# Clerk MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clerk)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Manage authentication and users via Clerk — track active sessions, monitor organizations, and manage invitations directly from any AI agent.

## Description
Connect your **Clerk** account to any AI agent and take full control of your authentication and user management through natural conversation. Streamline how you monitor your user base and B2B organizations natively.

### What you can do

- **User Oversight** — List and retrieve details for all users in your application, including metadata and status natively
- **Session Intelligence** — Access and monitor all active user sessions across your platforms flawlessly
- **Organization Logistics** — List and manage B2B organizations and their member rosters securely
- **Invitation Tracking** — Access and review all pending and completed user invitations flawlessly
- **Allowlist Management** — List identifiers like emails and domains on your authentication allowlist flawlessly
- **Dashboard Visibility** — Retrieve a high-level summary of user counts and system health directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Clerk Secret Key (obtained from your dashboard API Keys)
3. Start managing your authentication from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — monitor user signups and verify session status using natural language
- **Customer Support** — quickly look up user profiles and organization memberships without opening the dashboard
- **Product Managers** — audit invitation success rates and active user counts straight from their chat interface
- **Operations Teams** — verify authentication allowlists and system health


## Available Tools (8)
- **get_auth_dashboard_summary**: Retrieve a summary of user counts and system health
- **get_user_auth_details**: Get detailed information for a specific user
- **list_auth_allowlist**: List identifiers (emails, domains) on the authentication allowlist
- **list_clerk_clients**: List all tracking clients (browser/device instances)
- **list_sent_invitations**: List all pending and completed user invitations
- **list_clerk_organizations**: List all organizations (B2B) in the application
- **list_active_sessions**: List all active user sessions
- **list_clerk_users**: List all users in your Clerk application


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Clerk** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my users in Clerk."

**🤖 AI Agent:**
> Retrieving your user list... I found 150 total users. The most recent signup was John Doe (john@example.com) yesterday. Would you like to see more details?

---

**👤 You:**
> "Show me the dashboard summary for my auth system."

**🤖 AI Agent:**
> Analyzing auth dashboard... You have 150 total users, 12 active sessions right now, and 5 pending invitations. The system health is optimal.

---

**👤 You:**
> "Check the status of invitation ID 'inv_12345'."

**🤖 AI Agent:**
> Checking invitation inv_12345... This invitation was sent to sarah@example.com and is currently 'Pending'. It has not been accepted yet.


## ❓ FAQ

**Q: Can I see how many users are currently logged in?**
Yes! Use the `list_active_sessions` tool. The agent will return a list of all current sessions, allowing you to gauge real-time platform activity.

**Q: How do I check if a specific user belongs to an organization?**
Use the `list_clerk_organizations` tool to find the organization and then review its members, or use `get_user_auth_details` to see the user's specific organization memberships.

**Q: Where do I find my Clerk Secret Key?**
Log in to your Clerk Dashboard, select your application, and navigate to **API Keys**. You can find your Secret Key starting with `sk_` there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clerk](https://vinkius.com/mcp/clerk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Clerk** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `clerk` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Clerk** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "clerk": {
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
