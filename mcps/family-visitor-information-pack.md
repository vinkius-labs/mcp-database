# Family Visitor Information Pack MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-visitor-information-pack)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Synthesize household data into a cohesive, guest-ready visitor document.

## Description
This MCP server provides a suite of tools to transform fragmented household information into a professional, organized visitor guide. Use `assemble_visitor_pack` to aggregate contacts, access instructions, routines, safety notes, and essentials into a single Markdown document. You can also use `query_household_info` to find specific details or `format_emergency_brief` to generate a mobile-friendly safety summary for immediate needs.


## Available Tools (4)
- **format_emergency_brief**: Creates a high-priority, condensed summary of only safety and contact information
- **assemble_visitor_pack**: Generates the final, formatted guest document by aggregating all provided household data
- **query_household_info**: Retrieves a specific subset of information from the provided household dataset
- **validate_household_data**: ) meets the required schema.

Checks the integrity and completeness of the individual data modules before assembly


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Visitor Information Pack** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a complete visitor pack with these contacts: [{'name': 'Alice', 'relationship': 'Host', 'phone': '555-0101'}], access: 'Use the keypad code 1234', routines: [], safety: [], essentials: [], departure: []"

**🤖 AI Agent:**
> # Welcome & Access
Use the keypad code 1234.

# People & Contacts
- Alice (Host): 555-0101

---

**👤 You:**
> "I need a quick emergency summary for these safety notes: [{'hazard': 'Loose rug', 'location': 'Hallway', 'instruction': 'Watch your step'}] and contacts: [{'name': 'Bob', 'relationship': 'Emergency', 'phone': '555-0202', 'is_emergency': true}]"

**🤖 AI Agent:**
> ## Safety
- Loose rug (Hallway): Watch your step

## Emergency Contacts
- Bob (Emergency): 555-0202

---

**👤 You:**
> "Search for 'coffee' in the essentials category."

**🤖 AI Agent:**
> The coffee is located in the kitchen pantry on the second shelf.


## ❓ FAQ

**Q: How do I create the final document?**
Use the `assemble_visitor_pack` tool by providing the necessary data modules like contacts, routines, and safety notes.

**Q: Can I get a quick summary for emergencies?**
Yes, use the `format_emergency_brief` tool to generate a condensed, mobile-friendly summary of safety and contact information.

**Q: How can I verify my data is correct?**
You can use `validate_household_data` to check the integrity and completeness of individual data modules before assembly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-visitor-information-pack](https://vinkius.com/en/ai-agent-connect/family-visitor-information-pack)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Visitor Information Pack** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-visitor-information-pack` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Visitor Information Pack** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-visitor-information-pack": {
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
