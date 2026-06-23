# US Filing Deadline Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-filing-deadline-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate US federal court filing deadlines with automatic weekend and holiday adjustments.

## Description
This MCP server provides specialized tools for legal professionals to determine US federal procedural filing deadlines. By using `calculate_deadline`, you can input an event date and a rule type (such as RULE_12 or NOTICE_OF_APPEAL) to find the final deadline, automatically adjusted for weekends and federal holidays. The server also includes `list_supported_rules` to browse available legal rules and `check_date_validity` to verify if a specific date is a valid business day for starting a legal clock.


## Available Tools (3)
- **calculate_deadline**: Determines the final filing deadline for a specific event and rule type
- **check_date_validity**: Validates whether a provided date is a viable starting point for a legal clock
- **list_supported_rules**: Provides a list of all legal rules currently supported by the calculator


## 💬 Prompt Examples

Here are some examples of how you can interact with the **US Filing Deadline Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the deadline for an event that occurred on 2024-01-01 using RULE_12."

**🤖 AI Agent:**
> The final filing deadline is 2024-01-23.

---

**👤 You:**
> "What are the supported rules?"

**🤖 AI Agent:**
> The available rules are: RULE_12, NOTICE_OF_APPEAL, and RULE_59.

---

**👤 You:**
> "Is 2024-07-04 a valid business day?"

**🤖 AI Agent:**
> No, 2024-07-04 is a holiday (Independence Day).


## ❓ FAQ

**Q: What rules are supported by the calculator?**
The calculator supports RULE_12 (21 days), NOTICE_OF_APPEAL (30 days), and RULE_59 (28 days). You can use the `list_supported_rules` tool to see the full list.

**Q: How are weekends and holidays handled?**
If the calculated deadline falls on a Saturday, Sunday, or a US federal holiday, the tool automatically extends the deadline to the next available business day.

**Q: Can I check if a specific date is a valid starting point?**
Yes, use the `check_date_validity` tool to determine if a provided date is a business day or falls on a weekend/holiday.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-filing-deadline-calculator](https://vinkius.com/mcp/us-filing-deadline-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **US Filing Deadline Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `us-filing-deadline-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **US Filing Deadline Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "us-filing-deadline-calculator": {
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
