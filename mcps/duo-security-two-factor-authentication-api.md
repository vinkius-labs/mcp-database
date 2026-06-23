# Duo Security (Two-Factor Authentication API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/duo-security-two-factor-authentication-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage Duo Security users, trigger 2FA authentication, and handle account administration directly from any AI agent.

## Description
Connect your **Duo Security** instance to your AI agent to streamline identity management and multi-factor authentication workflows.

### What you can do

- **User Lifecycle** — List, create, and modify users. Handle bulk creations and manage the user trash/restoration process.
- **Authentication Control** — Trigger Duo Push, SMS, Phone, or Passcode authentication requests directly from the chat.
- **Pre-authentication Checks** — Determine if a user is authorized to log in and identify available factors before triggering a challenge.
- **Account Administration** — Manage sub-accounts, monitor billing editions, and track telephony credits.
- **Connectivity Testing** — Verify API integration keys and perform liveness checks on the Auth API.

### How it works

1. Subscribe to this server
2. Provide your Duo API Hostname, Integration Key, and Secret Key
3. Start managing security and identity tasks from Claude, Cursor, or any MCP client

### Who is this for?

- **IT Administrators** — quickly audit user lists or update user statuses without navigating the Duo Admin Panel
- **Security Operations (SecOps)** — automate 2FA verification steps or check authentication transaction statuses during investigations
- **DevOps Engineers** — integrate identity checks and account provisioning into automated workflows


## Available Tools (18)
- **auth_status**: Poll for the status of an asynchronous authentication request
- **auth**: Perform second-factor authentication
- **bulk_create_users**: Create up to 100 users in one request
- **check_auth**: Verify integration keys and signature generation
- **create_account**: Create a child account
- **create_user**: Create a new user in Duo
- **delete_account**: Delete a child account
- **get_billing_edition**: Get the billing edition for an account
- **get_telephony_credits**: Get the telephony credits for an account
- **list_accounts**: Retrieve child accounts for Duo MSP partners
- **list_users**: Can filter by username, email, or user_id_list.

Retrieve a paged list of users
- **modify_user**: Change user details
- **ping_auth**: Liveness check for the Auth API
- **preauth**: Determine if a user is authorized to log in and return available factors
- **restore_users**: Restore users from trash
- **set_billing_edition**: Set the billing edition for an account
- **set_telephony_credits**: Set the telephony credits for an account
- **trash_users**: Send users to trash (pending deletion for 7 days)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Duo Security (Two-Factor Authentication API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the first 10 users from our Duo directory."

**🤖 AI Agent:**
> I've retrieved the user list. Found users: 'jdoe' (Active), 'asmith' (Bypass), and 8 others. Would you like to see details for a specific user?

---

**👤 You:**
> "Send a Duo Push authentication request to username 'mrossi'."

**🤖 AI Agent:**
> Authentication request sent to 'mrossi' via Push. Transaction ID: `TX123456`. I'll monitor the status for you.

---

**👤 You:**
> "Check if user 'lking' is authorized to log in and what factors they can use."

**🤖 AI Agent:**
> User 'lking' is authorized. Available factors: Duo Push, Phone Call, and SMS Passcode. Which one should we trigger?


## ❓ FAQ

**Q: Can I trigger a Duo Push notification for a specific user?**
Yes. Use the `auth` tool and set the `factor` to 'push'. You can provide either the `username` or `user_id` to target the correct person.

**Q: How do I check which authentication factors are available for a user?**
Run the `preauth` tool with the user's details. It will return whether the user is authorized and a list of supported factors like push, phone, or SMS.

**Q: Is it possible to change a user's status to 'bypass' or 'disabled'?**
Yes, the `modify_user` tool allows you to update the `status` field to 'active', 'bypass', or 'disabled' using the user's unique ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/duo-security-two-factor-authentication-api](https://vinkius.com/mcp/duo-security-two-factor-authentication-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Duo Security (Two-Factor Authentication API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `duo-security-two-factor-authentication-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Duo Security (Two-Factor Authentication API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "duo-security-two-factor-authentication-api": {
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
