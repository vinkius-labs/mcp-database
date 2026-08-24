# Pool Chemistry Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/pool-chemistry-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Deterministic tool for precise swimming pool water chemistry adjustments and LSI analysis.

## Description
This MCP server provides precise chemical adjustment calculations and water balance diagnostics for swimming pools. Use `get_water_balance_analysis` to determine if your water is corrosive or scale-forming based on the Langelier Saturation Index (LSI). Use `calculate_chemical_adjustments` to find the exact amount of acid, alkalinity buffers, calcium, or chlorine needed to reach your target parameters. Additionally, `validate_water_safety` can be used to check if current pH and chlorine levels are safe for swimmers.


## Available Tools (3)
- **calculate_chemical_adjustments**: Calculates the exact mass or volume of specific chemicals needed to reach target parameters
- **get_water_balance_analysis**: Provides a comprehensive diagnostic of the current water state, including the LSI
- **validate_water_safety**: Checks if the water is safe for swimmers based on chlorine and pH levels


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pool Chemistry Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "My pool has a pH of 7.2 and total alkalinity of 80 ppm. What is the water balance?"

**🤖 AI Agent:**
> The water is currently in a corrosive state with an LSI of -0.4.

---

**👤 You:**
> "I need to raise my calcium hardness from 200 ppm to 300 ppm in a 20,000 gallon pool. How much calcium chloride do I need?"

**🤖 AI Agent:**
> You need to add 1,542 grams of calcium chloride.

---

**👤 You:**
> "Is it safe to swim if my pH is 8.0 and free chlorine is 2.0 ppm?"

**🤖 AI Agent:**
> No, the water is unsafe because the pH is outside the recommended range of 7.2-7.8.


## ❓ FAQ

**Q: How do I know if my pool water is balanced?**
You can use the `get_water_balance_analysis` tool to calculate the Langelier Saturation Index (LSI). A balanced state is between -0.3 and +0.3.

**Q: Can this tool tell me how much acid to add?**
Yes, the `calculate_chemical_adjustments` tool provides the exact volume of muriatic acid or sodium bisulfate required to reach your target pH.

**Q: Is my pool safe for swimming right now?**
You can verify this by using the `validate_water_safety` tool, which checks your current pH and chlorine levels against safety standards.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/pool-chemistry-calculator](https://vinkius.com/ai-agent-connect/pool-chemistry-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pool Chemistry Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pool-chemistry-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pool Chemistry Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pool-chemistry-calculator": {
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
