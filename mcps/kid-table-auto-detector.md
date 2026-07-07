# Kid Table Auto-Detector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kid-table-auto-detector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [automation](../categories/automation.md)

Automatically isolates children and links their parents to adjacent tables for supervision.

## Description
The `kid-table-auto-detector` MCP server automates the complex logic of event seating. It uses `identifyChildSeats` to find children and assign them to Kid Zone tables, then employs `linkParentSeating` to place parents at nearby tables for visibility. Finally, `auditSeatingSafety` ensures no child is left unsupervised.

### Available Tools

`identify_child_seats`, `link_parent_seating`, `audit_seating_safety`


## Available Tools (3)
- **audit_seating_safety**: Returns safety status and violations.

Validate the integrity of the final seating plan
- **identify_child_seats**: Returns child assignments and unassigned children.

Filter the guest list for children and assign them to available kid-specific tables
- **link_parent_seating**: Returns parent assignments and broken links.

Assign parents to tables near their children


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kid Table Auto-Detector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Assign children to kid tables for this guest list: [name: 'Timmy', is_child: true, parent_of: ['Alice']], [name: 'Alice', is_child: false]. Tables: [id: 1, zone: 'Kid'], [id: 2, zone: 'Standard']."

**🤖 AI Agent:**
> Timmy has been assigned to Table 1.

---

**👤 You:**
> "Link parents for the following assignments: Timmy is at Table 1."

**🤖 AI Agent:**
> Alice has been assigned to Table 2, which is adjacent to Table 1.

---

**👤 You:**
> "Check if the seating plan for Timmy at Table 1 and Alice at Table 2 is safe."

**🤖 AI Agent:**
> The seating plan is safe; all safety rules are met.


## ❓ FAQ

**Q: How does the tool identify children?**
It scans the `guestsArray` for any guest where the `is_child` property is set to true. Tools available: `identify_child_seats`, `link_parent_seating`, `audit_seating_safety`.

**Q: What defines a 'Kid Zone'?**
The `tablesArray` contains specific table IDs designated as part of the Kid Zone.

**Q: Can it handle large guest lists?**
Yes, the algorithm efficiently loops through guests and tables to assign seats based on proximity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kid-table-auto-detector](https://vinkius.com/mcp/kid-table-auto-detector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kid Table Auto-Detector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kid-table-auto-detector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kid Table Auto-Detector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kid-table-auto-detector": {
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
