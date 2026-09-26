# Household Key Custody Log MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/household-key-custody-log)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track the lifecycle and accountability of physical keys within a household.

## Description
This MCP server provides tools to manage the custody of physical keys. It allows for recording when keys are issued to individuals, when they are returned, and identifying who currently holds specific keys. Use `log_key_issuance` to start a custody event, `log_key_return` to close it, `query_active_custody` to see current holders, and `generate_signoff_report` to produce audit summaries.


## Available Tools (4)
- **generate_signoff_report**: Only includes completed cycles.

Produce a final, high-level summary table for auditing completed key transactions
- **log_key_issuance**: Ensure the key is not already issued.

Record when a key is handed over to a specific individual
- **log_key_return**: The key must currently be in an issued state.

Record when a key is returned to the primary custodian
- **query_active_custody**: You can filter by holder name.

Identify all individuals currently in possession of keys


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Household Key Custody Log** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Record that the Front Door key was given to John Doe on 2023-10-01 for maintenance."

**🤖 AI Agent:**
> The issuance for the Front Door key to John Doe has been recorded for 2023-10-01.

---

**👤 You:**
> "Who is currently holding any keys?"

**🤖 AI Agent:**
> John Doe is currently holding the Front Door key issued on 2023-10-01.

---

**👤 You:**
> "John Doe returned the Front Door key today."

**🤖 AI Agent:**
> The return of the Front Door key from John Doe has been successfully logged.


## ❓ FAQ

**Q: How do I record a new key assignment?**
Use the `log_key_issuance` tool with the key label, holder name, and date.

**Q: Can I see who currently has a key?**
Yes, use the `query_active_custody` tool to list all current key holders.

**Q: How do I generate an audit report?**
Use the `generate_signoff_report` tool by providing a start and end date.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/household-key-custody-log](https://vinkius.com/en/ai-agent-connect/household-key-custody-log)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Household Key Custody Log** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `household-key-custody-log` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Household Key Custody Log** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "household-key-custody-log": {
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
