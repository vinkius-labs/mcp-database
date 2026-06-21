# Applied Epic MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/applied-epic)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage insurance clients, policies, and activities with Applied Epic — track renewals and compliance via AI.

## Description
The **Applied Epic MCP Server** provides a powerful natural language interface to your Applied Systems insurance management platform. Connect your Applied Epic account to your AI agent to gain real-time visibility into your client relationships, policy lifecycles, and agency workflows.

### Key Capabilities

- **Client Management** — List and search for clients, and access full demographic and compliance data.
- **Policy Lifecycle** — Track active and historical policies, including effective and expiration dates and current statuses.
- **Workflow Automation** — Create and manage activities (tasks/logs) directly from your chat interface to ensure consistent follow-ups.
- **Lines of Business** — Drill down into specific lines of business for any policy, such as Workers Comp or General Liability.
- **Attachment Oversight** — Find and manage documents, photos, and proof of insurance linked to your clients and policies.
- **Secure Integration** — Uses industry-standard OAuth 2.0 authentication to safely access your agency's data.

### Who is this for?

- **Insurance Agents** — Quickly check client information and policy details without navigating complex menus.
- **Account Managers** — Monitor upcoming renewals and ensure all compliance tasks are completed on time.
- **Agency Operations** — Streamline workflow tracking and documentation management using AI-assisted automation.


## Available Tools
- **create_activity**: Create a new activity record
- **get_account_check**: Verify Applied Epic account connection
- **get_client**: Get details for a specific client
- **get_policy**: Get details for a specific policy
- **list_activities**: List all activities (tasks/logs)
- **list_attachments**: List all file attachments
- **list_clients**: List all insurance clients in Applied Epic
- **list_lines**: g., Workers Comp, GL) for a specific policyId.

List lines of business for a policy
- **list_policies**: List all insurance policies


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Applied Epic** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active insurance clients."

**🤖 AI Agent:**
> I've retrieved your active clients. You have 150 active clients, including 'Global Logistics Inc.' and 'Downtown Realty'.

---

**👤 You:**
> "Show me upcoming policy expirations for next month."

**🤖 AI Agent:**
> You have 12 policies expiring next month. The largest is 'Policy #ABC-123' for 'Global Logistics Inc.' expiring on the 15th.

---

**👤 You:**
> "Create an activity 'Renewal Follow-up' for client ID 'C998877'."

**🤖 AI Agent:**
> Activity 'Renewal Follow-up' has been successfully created and linked to client 'C998877'.


## ❓ FAQ

**Q: How do I get my Applied Epic API credentials?**
Register your application in the [Applied Dev Center](https://developer.myappliedproducts.com/) to receive a Client ID and Client Secret. You will also need your Enterprise ID and Epic Database Name.

**Q: What is the Database Name?**
The Database Name is the internal name of your Applied Epic database. You can find this information in your Epic platform settings or by contacting your agency's system administrator.

**Q: Can I see document attachments?**
Yes, the `list_attachments` tool allows you to find documents and files linked to clients and policies, though the content itself remains secured in your Epic platform.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/applied-epic](https://vinkius.com/mcp/applied-epic)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Applied Epic** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `applied-epic` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Applied Epic** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "applied-epic": {
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
