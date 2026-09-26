# Family Language Access Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-language-access-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication](../categories/communication.md)

Generate actionable communication guides by aggregating family language preferences and interpreter resources.

## Description
This MCP server provides a centralized system to manage language access for family units. It allows users to register language preferences, link professional or community interpreters, and catalog translated documents. The core capability is the `create_communication_guide` tool, which synthesizes these inputs into a contactable guide that maps every family member to their preferred language and necessary support resources.


## Available Tools (5)
- **create_communication_guide**: Generates the final, actionable contactable communication guide for a specific family unit
- **link_interpreter**: Connects a specific interpreter to a language pair or a specific family member
- **query_family_registry**: Retrieves the list of family members and their existing language/communication metadata
- **register_language_preference**: Records or updates the preferred language and communication needs for an individual
- **catalog_translated_document**: Adds a document to the available resources for a specific language


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Language Access Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a communication guide for the Smith family members: ID-123 and ID-456."

**🤖 AI Agent:**
> The communication guide for the Smith family has been generated. It includes profiles for ID-123 and ID-456, their preferred languages, and the contact details for the primary Spanish interpreter.

---

**👤 You:**
> "What is the current language profile for the Garcia family?"

**🤖 AI Agent:**
> The Garcia family registry contains three members: Maria (Spanish), Jose (Spanish), and Elena (English).

---

**👤 You:**
> "Register a new language preference for member ID-999."

**🤖 AI Agent:**
> The language preference for member ID-999 has been successfully updated to French with the requested communication settings.


## ❓ FAQ

**Q: How do I generate a guide for my family?**
Use the `create_communication_guide` tool by providing the unique identifiers for the family members you wish to include.

**Q: Can I add translated documents to the plan?**
Yes, you can use `catalog_translated_document` to register existing translated assets, which the guide will then suggest as alternatives to live interpretation.

**Q: How are interpreters assigned?**
You can use `link_interpreter` to connect an interpreter to a specific language pair and designate them as a primary contact.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-language-access-plan](https://vinkius.com/en/ai-agent-connect/family-language-access-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Language Access Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-language-access-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Language Access Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-language-access-plan": {
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
