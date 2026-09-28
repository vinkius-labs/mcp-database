# Personal Records Emergency Folder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/personal-records-emergency-folder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Securely organize and access life-critical documents and emergency contacts.

## Description
This MCP server provides a secure bridge for AI agents to help you organize and manage life-critical information. It allows for the creation of a structured emergency folder containing medical records, insurance details, and authorized contacts. Use `get_emergency_folder_outline` to view your organized sections, `generate_contents_checklist` to track missing documents, `get_access_instructions` to guide authorized personnel during a crisis, and `schedule_refresh_reminders` to ensure your records stay current through annual audits.


## Available Tools (4)
- **generate_contents_checklist**: Produces a task list of what documents or information are currently present versus what is missing
- **get_access_instructions**: Describes how authorized personnel can retrieve and view the documents in a crisis
- **get_emergency_folder_outline**: Provides a high-level structural view of the user's emergency organization
- **schedule_refresh_reminders**: Configures and retrieves the schedule for the annual audit of the emergency folder


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Personal Records Emergency Folder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me an outline of my critical emergency information."

**🤖 AI Agent:**
> Your critical sections include: Medical History (3 items), Emergency Contacts (2 items), and Allergies (1 item).

---

**👤 You:**
> "What documents am I missing from my emergency folder?"

**🤖 AI Agent:**
> You are currently missing: Life Insurance Policy and Last Will and Testament.

---

**👤 You:**
> "How can my spouse access my medical records in an emergency?"

**🤖 AI Agent:**
> Your spouse can follow the steps provided by the access instructions, which include verifying their identity and confirming the active emergency state.


## ❓ FAQ

**Q: How can I see what information is currently organized?**
You can use the `get_emergency_folder_outline` tool to see a high-level view of your organized sections based on importance levels.

**Q: How do I ensure my emergency contacts are up to date?**
Use the `schedule_refresh_reminders` tool to set a monthly reminder for your annual audit to keep all records valid.

**Q: Can my family access my records during an emergency?**
Yes, authorized personnel can use `get_access_instructions` to follow specific steps for retrieving documents during a crisis.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/personal-records-emergency-folder](https://vinkius.com/en/ai-agent-connect/personal-records-emergency-folder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Personal Records Emergency Folder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `personal-records-emergency-folder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Personal Records Emergency Folder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "personal-records-emergency-folder": {
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
