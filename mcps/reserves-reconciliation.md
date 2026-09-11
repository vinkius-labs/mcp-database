# Reserves Reconciliation MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/reserves-reconciliation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [accounting](../categories/accounting.md)

Reconcile oil and gas reserve changes between reporting periods.

## Description
This MCP server provides specialized engineering and accounting tools to bridge the gap between opening and closing reserve volumes. It allows AI agents to calculate the reserve bridge using `calculate_reserve_bridge`, analyze the impact of technical versus commercial revisions with `analyze_revision_impact`, determine depletion efficiency via `calculate_production_efficiency`, and verify mathematical accuracy using `validate_reconciliation_integrity`.


## Available Tools (4)
- **analyze_revision_impact**: Analyze the impact of technical vs commercial revisions
- **calculate_production_efficiency**: Calculate production efficiency relative to total depletion
- **calculate_reserve_bridge**: Calculate the reserve bridge between opening and closing volumes
- **validate_reconciliation_integrity**: Validate the mathematical integrity of a reconciliation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reserves Reconciliation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the reserve bridge for an opening volume of 1000, production of 200, discoveries of 50, and technical revisions of -10."

**🤖 AI Agent:**
> The closing reserves are 840, with a total change of -160.

---

**👤 You:**
> "Analyze the impact of a 50 unit technical revision and a 20 unit commercial revision."

**🤖 AI Agent:**
> The primary driver is Technical, with a total impact of 70.

---

**👤 You:**
> "What is the production efficiency if production is 150, opening reserves were 1000, and other depletions are 50?"

**🤖 AI Agent:**
> The production percentage is 75%.


## ❓ FAQ

**Q: What is a reserve bridge?**
A reserve bridge is a reconciliation that explains the movement from opening reserves to closing reserves by accounting for production, discoveries, revisions, and other factors.

**Q: How can I check if my reconciliation is mathematically correct?**
You can use the `validate_reconciliation_integrity` tool to verify that the sum of all movements correctly bridges the opening and closing volumes.

**Q: Does this tool handle commercial revisions?**
Yes, the `calculate_reserve_bridge` tool specifically includes a parameter for commercial revisions to account for economic changes in reserve viability.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/reserves-reconciliation](https://vinkius.com/en/ai-agent-connect/reserves-reconciliation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Reserves Reconciliation** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `reserves-reconciliation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Reserves Reconciliation** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "reserves-reconciliation": {
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
