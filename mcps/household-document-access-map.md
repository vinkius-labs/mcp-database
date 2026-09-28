# Household Document Access Map MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/household-document-access-map)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage and visualize document permissions within a household using role-based access.

## Description
This MCP server provides a structured way to manage document permissions for all household members. It applies role-based access control (RBAC) and manages emergency-only exceptions to ensure sensitive documents are only accessible to authorized individuals. Use `get_permission_matrix` to see a full overview of access, `get_access_instructions` for personalized guides, `get_emergency_access_protocol` for crisis management, and `generate_revocation_and_review_plan` to maintain security through audits and revocation tasks.


## Available Tools (4)
- **get_access_instructions**: Provides a personalized guide for a specific member explaining how and where they can access their permitted documents
- **get_emergency_access_protocol**: Identifies which documents are accessible under "Emergency Only" conditions and which members are authorized for such access
- **get_permission_matrix**: Generates a complete overview of who can access which documents
- **generate_revocation_and_review_plan**: Produces a checklist of actions for maintaining security, including removing access for departed members and scheduled audits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Household Document Access Map** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me a matrix of all document permissions in my house."

**🤖 AI Agent:**
> Here is the permission matrix showing the access levels for all household members across all documents.

---

**👤 You:**
> "What documents can John access?"

**🤖 AI Agent:**
> John is authorized to access the following documents: Passport (View), Utility Bill (Edit), and Medical Record (View).

---

**👤 You:**
> "What is the emergency protocol for critical documents?"

**🤖 AI Agent:**
> In an emergency, the following documents are accessible: Birth Certificate (for Head of Household) and Legal Will (for designated Emergency Contact).


## ❓ FAQ

**Q: How can I see who has access to specific documents?**
You can use the `get_permission_matrix` tool to generate a complete overview of all household members and their permitted access levels for every document.

**Q: What happens during an emergency?**
The `get_emergency_access_protocol` tool identifies which documents and members are authorized for access under predefined emergency conditions, bypassing standard restrictions.

**Q: How do I manage access when someone leaves the household?**
Use the `generate_revocation_and_review_plan` tool to create a checklist of revocation tasks to remove access for departed members and schedule necessary security audits.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/household-document-access-map](https://vinkius.com/en/ai-agent-connect/household-document-access-map)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Household Document Access Map** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `household-document-access-map` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Household Document Access Map** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "household-document-access-map": {
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
