# Household Accounts Record Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/household-accounts-record-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Organize household account metadata, provider contacts, and access governance.

## Description
This MCP server provides a structured system for managing household account metadata and access governance. It allows users to maintain a registry of service providers, contact information, and renewal schedules without storing sensitive credentials. Use `register_account_metadata` to add new services, `generate_contact_map` to aggregate provider details, `list_pending_updates` to track upcoming renewals, and `create_sharing_protocol` to generate secure instructions for authorized users.


## Available Tools (4)
- **create_sharing_protocol**: Generate instructions for safely sharing account information with an authorized user
- **generate_contact_map**: Aggregate all provider contact information for a specific category
- **list_pending_updates**: Identify accounts that require attention due to upcoming renewals or lapsed review intervals
- **register_account_metadata**: Create a new entry in the household account registry


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Household Accounts Record Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Register a new internet service from ProviderX that renews on 2025-05-20."

**🤖 AI Agent:**
> The account for ProviderX has been registered with ID REG-123 and is set for renewal on May 20, 2025.

---

**👤 You:**
> "Show me all contact information for my Utility accounts."

**🤖 AI Agent:**
> I found the following contacts for Utility accounts: Water Corp (email: support@watercorp.com) and Power Grid (phone: 555-0199).

---

**👤 You:**
> "Which accounts need to be reviewed within the next 30 days?"

**🤖 AI Agent:**
> The following accounts require attention: Netflix (Renewal Task) and Home Insurance (Review Task).


## ❓ FAQ

**Q: Does this server store my passwords?**
No. This system follows minimum-necessary data principles and only stores metadata. You should use `register_account_metadata` to reference an external secure storage location where your actual credentials reside.

**Q: How can I see which accounts need renewal?**
You can use the `list_pending_updates` tool to identify accounts that require attention due to upcoming renewal dates or lapsed review intervals.

**Q: How do I share account details with a family member?**
Use the `create_sharing_protocol` tool. It will verify if the recipient is an authorized user and then generate a secure procedure for sharing the information.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/household-accounts-record-plan](https://vinkius.com/en/ai-agent-connect/household-accounts-record-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Household Accounts Record Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `household-accounts-record-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Household Accounts Record Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "household-accounts-record-plan": {
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
