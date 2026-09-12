# Butadiene Extraction Plant Design Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/butadiene-extraction-plant-design-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

A specialized design engine for modeling extractive distillation units to recover high-purity butadiene.

## Description
This MCP server provides a complete suite of engineering tools for designing butadiene extraction plants. It allows users to evaluate C4 feedstock suitability using `analyze_feedstock_composition`, identify the most efficient extraction agents with `select_optimal_solvent`, calculate physical tower dimensions via `design_extraction_column`, and predict final product quality through `calculate_process_yield`. It is designed to handle complex extractive distillation modeling, including solvent selection (NMP, DMF, ACN) and critical impurity management.


## Available Tools (4)
- **analyze_feedstock_composition**: 
- **calculate_process_yield**: 
- **design_extraction_column**: 
- **select_optimal_solvent**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Butadiene Extraction Plant Design Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Evaluate a C4 cut with 0.4 butadiene, 0.3 butenes, and 0.3 butanes at a capacity of 500 units."

**🤖 AI Agent:**
> The feedstock suitability score is 0.75, with an estimated recovery potential of 92%.

---

**👤 You:**
> "What is the best solvent for a feedstock with 0.5 butadiene and a target purity of 0.995?"

**🤖 AI Agent:**
> NMP is the recommended solvent, offering a selectivity index of 0.88 and a boiling point suitable for this purity target.

---

**👤 You:**
> "Design a column using NMP with a feed flow of 100 and a solvent-to-feed ratio of 5 for 0.995 purity."

**🤖 AI Agent:**
> The designed column will have a diameter of 2.4 meters, 35 trays, and a total height of 18.5 meters.


## ❓ FAQ

**Q: How do I evaluate my feedstock?**
You can use the `analyze_feedstock_composition` tool by providing the molar fractions of your C4 cut and the required plant capacity.

**Q: Can I design the physical column dimensions?**
Yes, once you have selected a solvent, use `design_extraction_column` to calculate tower diameter, tray count, and total height.

**Q: How is the final product quality determined?**
The `calculate_process_yield` tool determines the final recovery efficiency and impurity levels based on your column design and feedstock.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/butadiene-extraction-plant-design-engine](https://vinkius.com/en/ai-agent-connect/butadiene-extraction-plant-design-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Butadiene Extraction Plant Design Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `butadiene-extraction-plant-design-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Butadiene Extraction Plant Design Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "butadiene-extraction-plant-design-engine": {
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
