# Family Account Permission Matrix MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-account-permission-matrix)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage and audit family service access permissions through structured matrices and secure access references.

## Description
This MCP server provides a governance framework for managing family service access. It allows users to `generate_permission_matrix` to map family members to specific services, define permitted and prohibited actions, and generate secure `accessReference` identifiers. You can also use `get_access_verification` to validate permissions, `schedule_permission_review` to manage security audits, and `audit_approval_workflow` to identify authorized approvers for any service.


## Available Tools (4)
- **audit_approval_workflow**: Identifies which contact needs to be reached to change permissions for a specific service
- **generate_permission_matrix**: Produces the primary access document by mapping people to services and their allowed actions
- **get_access_verification**: Validates if a specific person has the right to perform an action on a specific service using the access reference
- **schedule_permission_review**: Records or retrieves the next scheduled audit date for a specific service's permissions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Account Permission Matrix** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a permission matrix for Alice and Bob for Netflix and Utilities, where Alice can do everything and Bob can only view."

**🤖 AI Agent:**
> The permission matrix has been generated. Alice has full access to Netflix and Utilities, while Bob is restricted to viewing only.

---

**👤 You:**
> "Can I verify if the access reference 'ref_123' is allowed to 'Pay Bill' on the 'Utilities' service?"

**🤖 AI Agent:**
> Yes, the access reference 'ref_123' is authorized to 'Pay Bill' for the Utilities service.

---

**👤 You:**
> "Who is the authorized contact to change permissions for the Banking service?"

**🤖 AI Agent:**
> The authorized approver for the Banking service is the Primary Account Holder.


## ❓ FAQ

**Q: How do I create a new permission grid?**
Use the `generate_permission_matrix` tool by providing the list of services, family members, and the specific actions allowed or forbidden.

**Q: What is an access reference?**
An access reference is a unique, non-sensitive identifier used to verify if a person has permission to perform an action without exposing passwords.

**Q: How can I schedule a security audit?**
You can use the `schedule_permission_review` tool to set a future date for auditing a specific service's permissions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-account-permission-matrix](https://vinkius.com/en/ai-agent-connect/family-account-permission-matrix)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Account Permission Matrix** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-account-permission-matrix` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Account Permission Matrix** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-account-permission-matrix": {
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
