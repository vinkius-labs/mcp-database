# Wine Chaptalization Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-chaptalization-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate precise sugar additions for increasing alcohol potential in grape must.

## Description
This MCP server provides winemakers with precise tools for chaptalization. It calculates the exact mass of sugar needed to reach a target Brix level while accounting for volume displacement caused by sugar dissolution. Users can verify if planned additions meet regional legal standards using `check_legal_compliance`, estimate the resulting alcohol impact with `get_alcohol_potential_summary`, and manage inventory via `validate_sugar_inventory`. It is designed to ensure accuracy and regulatory compliance during the winemaking process.


## Available Tools (4)
- **check_legal_compliance**: Verifies if the planned chaptalization adheres to the legal limits of specific regions
- **get_alcohol_potential_summary**: Provides a high-level overview of the alcohol impact of a planned addition
- **get_sugar_addition_requirements**: Calculates the exact mass of sugar needed to reach a target Brix level
- **validate_sugar_inventory**: Checks if the winemaker has enough physical sugar on hand


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Chaptalization Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much sucrose do I need to add to 500 liters of must at 18 Brix to reach 22 Brix?"

**🤖 AI Agent:**
> To reach 22 Brix in 500 liters of must, you need to add 10,452.6 grams of sucrose. This will result in a total volume of approximately 510.2 liters.

---

**👤 You:**
> "Is it legal in the EU to increase Brix from 15 to 20?"

**🤖 AI Agent:**
> No, an increase from 15 to 20 Brix exceeds the maximum allowable Brix increase for the EU region.

---

**👤 You:**
> "What will be the alcohol increase if I add 5000 grams of sugar to 1000 liters of must?"

**🤖 AI Agent:**
> Adding 5000 grams of sugar to 1000 liters of must will result in an alcohol increase of approximately 0.29% v/v.


## ❓ FAQ

**Q: How does the tool account for volume changes?**
The `get_sugar_addition_requirements` tool calculates the volume displacement caused by the added sugar mass to ensure the final Brix and alcohol calculations are accurate.

**Q: Can I check if my sugar addition is legal?**
Yes, you can use the `check_legal_compliance` tool to verify if your planned Brix increase adheres to the specific regulations of the USA or EU.

**Q: What sugar types are supported?**
The calculator supports both sucrose (granulated sugar) and liquid concentrates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-chaptalization-calculator](https://vinkius.com/en/ai-agent-connect/wine-chaptalization-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Chaptalization Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-chaptalization-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Chaptalization Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-chaptalization-calculator": {
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
