# PRMS Reserves Categorization MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/prms-reserves-categorization)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [energy](../categories/energy.md)

Classify petroleum volumes into PRMS categories like 1P, 2P, and 3P.

## Description
This MCP server provides tools to classify petroleum volumes according to the Petroleum Resources Management System (PRMS) framework. It uses geological certainty, development status, and commercial viability to categorize volumes into Proved (1P), Probable (2P), Possible (3P), Contingent Resources, or Prospective Resources. Use `categorize_volumes` to perform individual classifications, `get_reserve_totals` to aggregate cumulative totals, and `validate_prms_compliance` to ensure hierarchical data integrity.


## Available Tools (4)
- **evaluate_commercial_risk**: Analyzes whether a volume should be moved from "Resources" to "Reserves" based on commercial thresholds
- **get_reserve_totals**: Aggregates multiple classified volumes to calculate cumulative 1P, 2P, and 3P totals
- **validate_prms_compliance**: Checks if a set of categorized volumes follows the hierarchical rules of the PRMS
- **categorize_volumes**: Performs the primary classification of petroleum volumes into PRMS categories


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PRMS Reserves Categorization** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Classify a volume of 500 units with high geological certainty, currently in production, and commercially viable."

**🤖 AI Agent:**
> The volume is classified as Proved (1P).

---

**👤 You:**
> "What is the total 2P reserve if I have a Proved volume of 100 and a Probable volume of 50?"

**🤖 AI Agent:**
> The cumulative 2P total is 150.

---

**👤 You:**
> "Analyze the commercial risk for a Contingent Resource with an economic indicator of 0.8."

**🤖 AI Agent:**
> The volume is commercially viable, and the recommended action is to re-classify as Reserves.


## ❓ FAQ

**Q: How do I classify a new volume?**
You can use the `categorize_volumes` tool by providing the geological confidence, development status, and commercial viability of the volume.

**Q: Can I calculate cumulative 1P, 2P, and 3P totals?**
Yes, the `get_reserve_totals` tool aggregates multiple classified volumes to provide cumulative 1P, 2P, and 3P totals.

**Q: How does the tool ensure PRMS compliance?**
The `validate_prms_compliance` tool checks your volume sets against hierarchical rules, such as ensuring a 'Possible' volume has corresponding 'Probable' or 'Proved' data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/prms-reserves-categorization](https://vinkius.com/en/ai-agent-connect/prms-reserves-categorization)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PRMS Reserves Categorization** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `prms-reserves-categorization` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PRMS Reserves Categorization** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "prms-reserves-categorization": {
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
