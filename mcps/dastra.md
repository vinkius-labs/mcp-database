# Dastra MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dastra)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Stay GDPR compliant with privacy management tools for data mapping, consent records, and breach notification workflows.

## Description
Connect your **Dastra** account to any AI agent and take full control of your data privacy and GDPR/LGPD compliance workflows through natural conversation.

### What you can do

- **DSR Orchestration** — Manage the full lifecycle of Data Subject Requests (DSR) programmatically, from creation and status tracking to high-fidelity resolution and archiving
- **Breach & Incident Tracking** — Programmatically document and track security incidents and data breaches to maintain a perfectly coordinated regulatory response
- **ROPA & Asset Intelligence** — Access your Record of Processing Activities (ROPA) and documented datasets to oversee data flow and classification across workspaces
- **Compliance Architecture** — Retrieve complete directories of actors (controllers, processors), tags, and processing activities to maintain a high-fidelity privacy registry
- **Workspace Visibility** — List and manage multiple workspaces programmatically to coordinate privacy operations across different business units directly through your agent

### How it works

1. Subscribe to this server
2. Retrieve your **API Access Token** from your Dastra user profile (API Access)
3. Start managing your compliance registry and privacy requests from Claude, Cursor, or any MCP client

No more manual record logging or digging through complex compliance tables in the portal. Your AI acts as your dedicated DPO and compliance coordinator.

### Who is this for?

- **Data Protection Officers (DPOs)** — instantly retrieve ROPA summaries and check DSR statuses using natural language commands
- **Compliance Teams** — automate the documentation of security incidents and monitor dataset classifications without leaving your workspace
- **Developers & Ops** — integrate automated privacy right handling and data mapping into custom internal tools through simple AI queries


## Available Tools
- **archive_dsr**: Archive a DSR
- **create_breach**: Create a new data breach record
- **create_dsr**: Create a new Data Subject Request
- **get_dsr**: Get details for a specific DSR
- **list_actors**: ).

List actors
- **list_breaches**: List data breaches
- **list_datasets**: List datasets
- **list_dsr**: List Data Subject Requests
- **list_processings**: List processing activities (ROPA)
- **list_tags**: List workspace tags
- **list_workspaces**: List all workspaces
- **update_dsr**: Update an existing DSR


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dastra** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active workspaces in my Dastra account."

**🤖 AI Agent:**
> I've retrieved your workspaces. You have 3 active environments: 'Core Operations' (ID: ws_123), 'Marketing', and 'HR Data'. Which one should we check for pending DSR requests?

---

**👤 You:**
> "Show pending DSR requests for workspace 'ws_123'."

**🤖 AI Agent:**
> Scanning workspace... I found 2 pending requests: 'Right of Access' from @user1 and 'Erasure Request' (ID: dsr_456). Would you like the full details for the access request?

---

**👤 You:**
> "Register a new data breach 'Server Unauthorized Access' in workspace 'ws_123'."

**🤖 AI Agent:**
> Breach documented! I've successfully registered the 'Server Unauthorized Access' incident in workspace ws_123. The incident ID is 'br_789'. I'll now help you monitor the investigation status.


## ❓ FAQ

**Q: How do I find my Dastra Access Token?**
Log in to Dastra, click your profile icon, navigate to **API Access**, and generate a new Access Token for your account.

**Q: What is a DSR request?**
Data Subject Requests are exercises of privacy rights (Access, Erasure, etc.) submitted by individuals under data protection laws.

**Q: Can I manage multiple workspaces?**
Yes! Use the `list_workspaces` tool to identify your workspace IDs, then use them as parameters in other tools like `list_dsr` or `list_breaches`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dastra](https://vinkius.com/mcp/dastra)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dastra** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `dastra` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dastra** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dastra": {
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
