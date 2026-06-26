# Values Alignment Score MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/values-alignment-score)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [psychology](../categories/psychology.md)

Measure the gap between your core values and your current life reality.

## Description
The Values Alignment Score MCP server provides diagnostic tools to identify discrepancies between your personal values and how you are currently living them. Using `calculate_alignment_gaps`, you can quantify the distance between importance and realization for each value. The `generate_dissatisfaction_ranking` tool helps you see which areas of life cause the most friction, while `identify_priority_area` pinpoints exactly where to focus your energy for maximum impact on well-being.


## Available Tools (3)
- **calculate_alignment_gaps**: Calculates the numerical discrepancy for every declared value
- **identify_priority_area**: Pinpoints the specific category or value that requires immediate focus
- **generate_dissatisfaction_ranking**: Identifies which values are causing the most significant life friction


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Values Alignment Score** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the alignment gaps for these values: Honesty (Importance 9, Realization 7), Career (Importance 8, Realization 4), and Health (Importance 10, Realization 9)."

**🤖 AI Agent:**
> [{"name": "Honesty", "gap": 2}, {"name": "Career", "gap": 4}, {"name": "Health", "gap": 1}]

---

**👤 You:**
> "Based on these gaps: Honesty (2), Career (4), Health (1), which value is causing the most dissatisfaction?"

**🤖 AI Agent:**
> ["Career", "Honesty", "Health"]

---

**👤 You:**
> "Identify the priority area using these gaps: Honesty (2), Career (4) and metadata: Honesty is Personal, Career is Professional."

**🤖 AI Agent:**
> Career


## ❓ FAQ

**Q: How do I use the alignment gap tool?**
Provide a JSON array of assessments to `calculate_alignment_gaps`, where each object includes the value name, its importance (0-10), and its realization (0-10).

**Q: What does the dissatisfaction ranking show?**
The `generate_dissatisfaction_ranking` tool returns a list of values sorted by the magnitude of their alignment gap, highlighting which areas are causing the most tension.

**Q: How can I identify my priority area?**
Use `identify_priority_area` by providing the gap results and a metadata mapping that links each value to its category (e.g., Personal, Professional).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/values-alignment-score](https://vinkius.com/mcp/values-alignment-score)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Values Alignment Score** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `values-alignment-score` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Values Alignment Score** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "values-alignment-score": {
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
