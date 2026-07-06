# Memberstack MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/memberstack)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Member authentication and user management via Memberstack — manage members, plans, and custom fields.

## Description
Connect your **Memberstack** account to any AI agent and take full control of your member management and authentication workflows through natural conversation.

### What you can do

- **Member Administration** — List all members, search by email, and fetch detailed metadata including plan connections
- **Plan Management** — Enumerate membership plans and retrieve detailed configurations for free and paid offerings
- **Custom Data Handling** — List and manage custom fields defined for your members
- **Promotion & Offers** — Access and monitor active coupons and marketing promotions
- **App Visibility** — Retrieve high-level information about your current Memberstack application configuration

### How it works

1. Subscribe to this server
2. Enter your Memberstack Secret Key
3. Start managing your members from Claude, Cursor, or any MCP-compatible client


## Available Tools (10)
- **search_members**: Search members by email
- **get_member_plans**: Get plans for a specific member
- **get_plan**: Get details for a specific plan
- **list_coupons**: List all discount coupons
- **list_custom_fields**: List member custom fields
- **list_members**: List all members
- **list_plans**: List all membership plans
- **list_promotions**: List active promotions
- **get_application_info**: Get application details
- **get_member**: Get details for a specific member


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Memberstack** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 members who joined."

**🤖 AI Agent:**
> Retrieving members... I found your most recent users, including 'john.doe@example.com' and 'jane.smith@domain.com'.

---

**👤 You:**
> "Show details for member ID 'mem_12345'."

**🤖 AI Agent:**
> Inspecting member... Member 'mem_12345' is currently on the 'Pro Plan' and has been active since last month.

---

**👤 You:**
> "What are my available membership plans?"

**🤖 AI Agent:**
> Querying plans... You have 3 plans configured: 'Free Tier', 'Monthly Pro', and 'Annual Enterprise'.


## ❓ FAQ

**Q: How do I find my Memberstack Secret Key?**
Log in to Memberstack, go to Settings > API Keys, and you can generate or copy your Secret Key from there.

**Q: Can I search for members by email?**
Yes! Use the `search_members` tool and provide the email address to find a specific member record.

**Q: Is my member data secure?**
Absolutely. Your token is encrypted at rest and injected securely at runtime.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/memberstack](https://vinkius.com/mcp/memberstack)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Memberstack** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `memberstack` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Memberstack** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "memberstack": {
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
