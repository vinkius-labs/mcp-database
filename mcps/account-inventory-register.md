# Account Inventory Register MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/account-inventory-register)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Organize and audit your digital accounts by provider, purpose, and security status.

## Description
The Account Inventory Register provides a structured way to manage your digital credentials. Use `list_accounts` to view your full registry, `find_duplicate_purposes` to identify redundant accounts, and `identify_vulnerable_accounts` to find high-risk entries missing recovery methods. You can also use `get_review_priorities` to receive a prioritized list of accounts requiring immediate attention based on security gaps or inactivity.


## Available Tools (4)
- **identify_vulnerable_accounts**: Locates accounts that lack a recovery method
- **list_accounts**: Provides a full overview of all registered accounts
- **find_duplicate_purposes**: Identifies accounts that share the same provider and purpose
- **get_review_priorities**: Generates a prioritized list of accounts that need user intervention


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Account Inventory Register** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all my accounts."

**🤖 AI Agent:**
> Here is the list of your registered accounts: Google (personal, user@gmail.com), AWS (work, admin@company.com), and Netflix (entertainment, user@email.com).

---

**👤 You:**
> "Are there any duplicate accounts for Google?"

**🤖 AI Agent:**
> Yes, you have two Google accounts serving the same purpose: user@gmail.com and user_backup@gmail.com.

---

**👤 You:**
> "Which accounts need my immediate attention?"

**🤖 AI Agent:**
> Your highest priority review is user@gmail.com because it is missing a recovery method.


## ❓ FAQ

**Q: How can I see all my registered accounts?**
You can use the `list_accounts` tool to retrieve a complete overview of all your registered accounts.

**Q: How do I find accounts that are security risks?**
Use `identify_vulnerable_accounts` to find accounts missing recovery methods, or `get_review_priorities` to see a prioritized list of accounts needing attention.

**Q: Can I filter my account list by a specific service?**
Yes, most tools like `list_accounts` and `identify_vulnerable_accounts` allow you to filter results by a specific provider.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/account-inventory-register](https://vinkius.com/en/ai-agent-connect/account-inventory-register)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Account Inventory Register** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `account-inventory-register` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Account Inventory Register** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "account-inventory-register": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
