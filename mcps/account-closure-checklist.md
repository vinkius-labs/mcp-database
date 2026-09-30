# Account Closure Checklist MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/account-closure-checklist)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generates structured task checklists and dependency maps for closing digital accounts.

## Description
This MCP server provides a structured framework for managing the complex process of digital account decommissioning. It helps users mitigate financial, access, and security risks by generating precise task checklists and dependency maps. Using tools like `get_closure_prerequisites` and `map_closure_dependencies`, agents can identify necessary manual actions, such as clearing balances or unlinking services, and determine the correct order of operations. The server also includes `calculate_closure_timeline` to manage deadlines and `verify_account_readiness` to perform final audits before deactivation.


## Available Tools (4)
- **get_closure_prerequisites**: Identifies the immediate manual actions required to prepare an account for closure
- **map_closure_dependencies**: Determines the order of operations by identifying which tasks must be completed before others
- **verify_account_readiness**: Performs a final audit to see if the account meets all criteria for immediate closure
- **calculate_closure_timeline**: Determines the final target date for account deactivation based on service rules and pending tasks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Account Closure Checklist** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What do I need to do before I can close account ACC-123?"

**🤖 AI Agent:**
> To prepare account ACC-123 for closure, you must: 1. Clear the remaining credit balance of $15.00. 2. Cancel the active 'Premium Monthly' subscription. 3. Unlink the primary recovery email.

---

**👤 You:**
> "Is account ACC-456 ready to be closed right now?"

**🤖 AI Agent:**
> No, account ACC-456 is not ready. There is still an active subscription linked to the account and an outstanding balance of $5.00.

---

**👤 You:**
> "What is the timeline if I want to close account ACC-789 by December 31st?"

**🤖 AI Agent:**
> To meet the target closure date of December 31st, all prerequisite actions must be completed by December 15th to account for the service cooling-off period. The risk level is currently low.


## ❓ FAQ

**Q: How do I know if my account is ready to be closed?**
You can use the `verify_account_readiness` tool to perform a final audit. It checks if all financial balances are zero and all critical dependencies are resolved.

**Q: Can I determine the best date to close my account?**
Yes, the `calculate_closure_timeline` tool helps you determine the final target date and identifies the deadline for all prerequisite actions.

**Q: What kind of tasks will be included in the checklist?**
The `get_closure_prerequisites` tool identifies tasks across financial, service, and security categories, such as clearing balances or canceling subscriptions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/account-closure-checklist](https://vinkius.com/en/ai-agent-connect/account-closure-checklist)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Account Closure Checklist** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `account-closure-checklist` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Account Closure Checklist** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "account-closure-checklist": {
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
