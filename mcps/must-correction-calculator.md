# Must Correction Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/must-correction-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate precise chemical and nutrient adjustments for grape must before fermentation.

## Description
This MCP server provides winemakers with the precise stoichiometric calculations needed to adjust grape must parameters. It handles chaptalization via `calculate_sugar_adjustment`, acidity adjustments through `calculate_acid_adjustment`, and nitrogen requirements using `calculate_nutrient_addition`. The server also generates a logical operational plan using `correction_schedule` to ensure all additions are sequenced correctly, accounting for volume changes and regional legal constraints.


## Available Tools (4)
- **acid_adjustment**: Calculates the amount of acid needed to reach target pH and TA levels
- **correction_schedule**: Provides a step-by-step operational plan for all necessary adjustments
- **nutrient_addition**: Determines the amount of nitrogen source required to reach target YAN
- **sugar_adjustment**: Calculates the amount of sugar needed to reach a target Brix level


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Must Correction Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 500L of must with 18 Brix. I need to reach 22 Brix in the USA. How much sugar do I need?"

**🤖 AI Agent:**
> You need to add 11.54 kg of sugar to reach 22 Brix, resulting in a final volume of 511.54 liters.

---

**👤 You:**
> "My must has a pH of 3.6 and TA of 6.0 g/L. I want to reach pH 3.4 and TA 7.5 g/L in 1000L using tartaric acid."

**🤖 AI Agent:**
> To reach your target, you need to add 1.45 kg of tartaric acid, resulting in a final volume of 1001.45 liters.

---

**👤 You:**
> "The YAN is 120 mg/L and I need it to be 200 mg/L for 250L of must using DAP."

**🤖 AI Agent:**
> You need to add 0.032 kg of DAP to reach the target YAN level.


## ❓ FAQ

**Q: How does the tool handle regional regulations?**
The `calculate_sugar_adjustment` tool checks the specified region (e.g., USA or Europe) to ensure that any requested sugar addition remains within legal limits for that jurisdiction.

**Q: Does the calculation account for volume changes?**
Yes, all tools use stoichiometric calculations that account for the increase in total volume when adding sugar, acid, or nutrients.

**Q: Can I use this with Claude Desktop?**
Yes, you can connect this server to Claude Desktop, Cursor, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/must-correction-calculator](https://vinkius.com/en/ai-agent-connect/must-correction-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Must Correction Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `must-correction-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Must Correction Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "must-correction-calculator": {
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
