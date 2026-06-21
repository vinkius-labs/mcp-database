# Thinkific MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/thinkific-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [learning-training](../categories/learning-training.md)

Manage Thinkific groups and webhooks — delete specific student groups and monitor site events directly from your AI agent.

## Description
Connect your **Thinkific** admin account to any AI agent to streamline your LMS management and event monitoring through natural conversation.

### What you can do

- **Group Administration** — Permanently delete specific student groups using their unique IDs to keep your dashboard organized.
- **Webhook Monitoring** — Retrieve a paginated list of all configured webhooks on your site to audit integrations and event triggers.
- **System Auditing** — Inspect webhook configurations including endpoints and limits to ensure your automated workflows are running correctly.

### How it works

1. Subscribe to this server
2. Enter your Thinkific API Key
3. Start managing your learning platform from Claude, Cursor, or any MCP-compatible client

No more digging through deep settings menus to find webhook URLs or clean up old groups. Your AI acts as a specialized LMS administrator.

### Who is this for?

- **Course Creators** — quickly clean up expired student groups without navigating the full admin UI.
- **LMS Developers** — audit and list active webhooks to debug integration flows directly from the terminal or code editor.
- **Operations Managers** — maintain site hygiene by managing organizational structures via simple commands.


## Available Tools (2)
- **delete_group**: Delete a group in Thinkific
- **list_webhooks**: List Thinkific webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Thinkific** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all webhooks configured on my Thinkific site."

**🤖 AI Agent:**
> I've retrieved your webhooks. You have 3 active webhooks, including 'Order Created' pointing to your Zapier endpoint and 'Enrollment Completed'.

---

**👤 You:**
> "Delete the Thinkific group with ID 987654."

**🤖 AI Agent:**
> The group with ID 987654 has been successfully deleted from your Thinkific site.

---

**👤 You:**
> "Show me the first 5 webhooks on page 2."

**🤖 AI Agent:**
> Fetching page 2 with a limit of 5... I found 5 webhooks on this page. Would you like to see the details for any specific one?


## ❓ FAQ

**Q: Can I delete a specific group if I have its ID?**
Yes. Use the `delete_group` tool by providing the Group ID. This will use the Thinkific Admin API to remove the group from your site.

**Q: How can I see which webhooks are currently active on my Thinkific site?**
You can use the `list_webhooks` tool. It allows you to retrieve a list of all configured webhooks, and you can even specify a `limit` or `page` number for better navigation.

**Q: Is there a limit to how many webhooks I can list at once?**
Yes, the `list_webhooks` tool accepts a `limit` parameter with a maximum of 25 items per page, as per Thinkific's API standards.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/thinkific-alternative](https://vinkius.com/mcp/thinkific-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Thinkific** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `thinkific-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Thinkific** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "thinkific-alternative": {
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
