# Stockpile Management Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/stockpile-management-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [inventory-management](../categories/inventory-management.md)

Optimize stockpile inventory, blending ratios, and draw strategies with real-time grade and capacity tracking.

## Description
The Stockpile Management Model connects AI agents to critical inventory and blending operations. It provides tools to monitor stockpile health, calculate precise blending ratios to meet target grades, and optimize extraction strategies. By accounting for physical factors like oxidation and segregation, it ensures consistent feed quality. Use `get_stockpile_status` to check current levels and grades, `calculate_blending_ratios` to plan material mixes, `optimize_draw_strategy` for extraction instructions, and `check_capacity_constraints` to prevent storage overflows.


## Available Tools (4)
- **calculate_blending_ratios**: Determines how to mix different stockpiles to hit a specific target grade
- **check_capacity_constraints**: Validates if planned inventory additions or movements will exceed physical limits
- **get_stockpile_status**: Provides a real-time snapshot of current stockpile levels, grades, and physical health
- **optimize_draw_strategy**: Determines the best way to extract material from stockpiles to maintain grade consistency and manage inventory


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Stockpile Management Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current status of stockpile ID 'STK-001'?"

**🤖 AI Agent:**
> Stockpile STK-001 has a current volume of 500m³, a grade of 65%, and a low segregation risk.

---

**👤 You:**
> "How much of STK-001 and STK-002 do I need to get 100m³ at a grade of 70%?"

**🤖 AI Agent:**
> To achieve 100m³ at 70% grade, you need 40m³ from STK-001 and 60m³ from STK-002.

---

**👤 You:**
> "Give me a draw strategy for a target grade of 68% and 50m³ volume using STK-001 and STK-003."

**🤖 AI Agent:**
> The optimal draw strategy is to extract 30m³ from STK-001 and 20m³ from STK-003 to maintain feed stability.


## ❓ FAQ

**Q: How does the model handle material degradation?**
The model accounts for oxidation by adjusting the current grade of a stockpile based on its exposure level, ensuring blending calculations remain accurate.

**Q: Can I check if a stockpile is full before adding material?**
Yes, you can use the `check_capacity_constraints` tool to validate if proposed additions will exceed the physical limits of your stockpiles.

**Q: How are blending ratios calculated?**
The `calculate_blending_ratios` tool calculates the exact proportions of available stockpiles needed to reach a specific target grade and volume.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/stockpile-management-model](https://vinkius.com/en/ai-agent-connect/stockpile-management-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Stockpile Management Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `stockpile-management-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Stockpile Management Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "stockpile-management-model": {
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
