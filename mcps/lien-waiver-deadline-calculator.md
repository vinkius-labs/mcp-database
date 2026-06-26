# Lien Waiver Deadline Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lien-waiver-deadline-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate statutory Mechanics Lien deadlines for preliminary notice, filing, and enforcement.

## Description
This MCP server provides precise calculations for US Mechanics Lien deadlines. By using tools like `get_state_regulations`, `calculate_preliminary_notice_deadline`, `calculate_lien_filing_deadline`, and `calculate_enforcement_deadline`, subcontractors and suppliers can identify critical statutory windows to preserve their rights to payment based on specific state laws.


## Available Tools (4)
- **calculate_enforcement_deadline**: Calculate the deadline for filing an enforcement lawsuit
- **calculate_lien_filing_deadline**: Calculate the deadline for recording a lien
- **calculate_preliminary_notice_deadline**: Calculate the deadline for serving a preliminary notice
- **get_state_regulations**: Retrieve statutory period durations for a specific jurisdiction


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lien Waiver Deadline Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the lien rules for California?"

**🤖 AI Agent:**
> For California, the statutory periods are: Preliminary Notice (20 days), Lien Filing (20 days after completion), and Enforcement (90 days after filing).

---

**👤 You:**
> "When is my preliminary notice deadline for Texas if work started on 2024-01-01?"

**🤖 AI Agent:**
> The preliminary notice deadline for Texas, based on a start date of 2024-01-01, is 2024-01-31.

---

**👤 You:**
> "Calculate the filing deadline for California if the project was completed on 2024-06-01."

**🤖 AI Agent:**
> The lien filing deadline for California, based on a completion date of 2024-06-01, is 2024-06-21.


## ❓ FAQ

**Q: How do I find the notice period for a specific state?**
Use the `get_state_regulations` tool and provide the name of the state to retrieve the statutory days for notice, filing, and enforcement.

**Q: Can I calculate the filing deadline if I know when the project ended?**
Yes, use the `calculate_lien_filing_deadline` tool by providing the state name and the project completion date in ISO 8601 format.

**Q: What happens if I miss the enforcement deadline?**
Missing the deadline calculated by `calculate_enforcement_deadline` may result in the loss of your lien rights, making the lien void.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lien-waiver-deadline-calculator](https://vinkius.com/mcp/lien-waiver-deadline-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lien Waiver Deadline Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lien-waiver-deadline-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lien Waiver Deadline Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lien-waiver-deadline-calculator": {
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
