# Shared Folder Access Audit MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/shared-folder-access-audit)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Audits folder permissions to identify unauthorized access, expired permissions, and external sharing risks.

## Description
This MCP server provides a suite of security auditing tools to reconcile real-time folder access against authorized permission lists. Use `audit_access_integrity` to find discrepancies between current access and the approved list, `audit_access_expiry` to identify permissions that have passed their expiration date, and `audit_external_risk` to monitor exposure to users outside your organization. You can also generate a complete cleanup strategy using `audit_remediation_plan` to address unauthorized, expired, or unapproved external access.


## Available Tools (4)
- **audit_access_expiry**: Identifies all active access permissions that have passed their expiration threshold
- **audit_access_integrity**: Identifies discrepancies between current folder access and the approved access list
- **audit_external_risk**: Isolates access granted to users outside the organization to monitor external exposure
- **audit_remediation_plan**: Generates a list of specific cleanup actions based on all identified security risks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shared Folder Access Audit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check for any unauthorized access in folder 'folder_123'."

**🤖 AI Agent:**
> Unauthorized access detected in folder 'folder_123': User 'user_99' has 'Editor' access but is not in the approved access list.

---

**👤 You:**
> "Are there any expired permissions for folder 'folder_456' as of 2024-01-01T00:00:00Z?"

**🤖 AI Agent:**
> Yes, user 'user_42' has expired access to folder 'folder_456' (expired on 2023-12-15).

---

**👤 You:**
> "Identify external sharing risks for folder 'folder_789'."

**🤖 AI Agent:**
> External sharing risk found: User 'ext_user_01' (external) has 'Viewer' access to folder 'folder_789'.


## ❓ FAQ

**Q: How do I identify users who should no longer have access?**
You can use `audit_access_expiry` to find users whose access has expired, or `audit_access_integrity` to find users who are not on the approved access list.

**Q: Can I detect external users sharing my folders?**
Yes, the `audit_external_risk` tool specifically isolates access granted to users outside your organization.

**Q: How do I get a list of recommended cleanup actions?**
Run the `audit_remediation_plan` tool to receive a list of recommended removals based on identified security risks.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/shared-folder-access-audit](https://vinkius.com/en/ai-agent-connect/shared-folder-access-audit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Shared Folder Access Audit** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `shared-folder-access-audit` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Shared Folder Access Audit** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shared-folder-access-audit": {
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
