# Emergency Document Grab-Folder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/emergency-document-grab-folder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Organize and secure critical documents with prioritized folder structures and access controls.

## Description
This MCP server provides a specialized planning framework for organizing critical documentation. It helps users manage emergency files by applying criticality tiering and strict access control rules. Use `get_folder_structure` to create a prioritized hierarchy, `generate_checklist` to prepare physical and digital copies, `get_access_instructions` to manage privacy-based access for authorized people, and `generate_review_calendar` to maintain an annual audit schedule.


## Available Tools (4)
- **generate_checklist**: Produces a step-by-step operational list to prepare, copy, and update the emergency files
- **generate_review_calendar**: Creates a recurring schedule for annual document audits and contact updates
- **get_access_instructions**: Provides specific guidance on how authorized individuals can access the documents while respecting privacy constraints
- **get_folder_structure**: Generates a logical, prioritized hierarchy of folders and sub-folders based on the urgency of the documents


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Emergency Document Grab-Folder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a folder structure for my medical records, bank access, and utility info, prioritizing medical records first."

**🤖 AI Agent:**
> I have organized your folders. Tier 1: Medical Records is your top-level folder, followed by Tier 2: Financial & Legal (Bank Access), and Tier 3: Operational & Utility (Utility Info).

---

**👤 You:**
> "I need a checklist to prepare 2 copies of my medical records and 1 copy of my property deed."

**🤖 AI Agent:**
> Here is your checklist: 1. Verify the location of medical records. 2. Duplicate medical records (2 copies). 3. Verify the location of property deed. 4. Duplicate property deed (1 copy). 5. Update the central registry.

---

**👤 You:**
> "Who can access my medical records if I set them to Private?"

**🤖 AI Agent:**
> If medical records are set to Private, only the primary account holder or designated emergency contact can access them.


## ❓ FAQ

**Q: How does the folder structure work?**
The `get_folder_structure` tool organizes your documents into a hierarchy based on the criticality levels you provide, ensuring the most urgent items are easiest to find.

**Q: Can I control who sees my private documents?**
Yes. By using `get_access_instructions`, you can define privacy levels (Private, Shared, or Public) to ensure only authorized individuals can access specific files.

**Q: How do I ensure my documents stay up to date?**
You can use `generate_review_calendar` to create a recurring schedule for annual audits, ensuring your contact information and document locations remain accurate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/emergency-document-grab-folder](https://vinkius.com/en/ai-agent-connect/emergency-document-grab-folder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Emergency Document Grab-Folder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `emergency-document-grab-folder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Emergency Document Grab-Folder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "emergency-document-grab-folder": {
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
