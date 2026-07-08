# Smart Recipe Scaler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/smart-recipe-scaler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Scale ingredient quantities precisely using metric-based conversion and smart rounding.

## Description
The Smart Recipe Scaler is a precision utility designed for cooks and bakers who need to adjust recipe yields without losing accuracy. By converting all measurements--including fractions, decimals, and mixed units like '1 1/2 cups'--into a standardized metric base (ml or g), the server ensures mathematical exactness during scaling. After applying your scale factor, the `reformat_to_kitchen_standard` tool uses a smart rounding algorithm to convert the result back into practical, human-readable kitchen units like '2 tsp' or '1/4 cup', avoiding absurdly precise decimals. Use `parse_measurement` to standardize inputs and `execute_scaling` to apply your multiplier.


## Available Tools (3)
- **execute_scaling**: Returns scaled amount.

Performs the mathematical scaling of a normalized metric value
- **parse_measurement**: Returns amount, category (volume/mass), and unitName.

Parses a raw ingredient string into a standardized numerical value and identifies its unit category
- **reformat_to_kitchen_standard**: Returns formatted string.

Converts a scaled metric value back into the most human-readable, practical kitchen unit


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Smart Recipe Scaler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Scale '1 1/2 cups' of flour by 2.5x"

**🤖 AI Agent:**
> 3 3/4 cups

---

**👤 You:**
> "How much is 250g of sugar if I want to make 0.5x the recipe?"

**🤖 AI Agent:**
> 125g

---

**👤 You:**
> "Convert 60ml to a kitchen standard unit."

**🤖 AI Agent:**
> 4 tbsp


## ❓ FAQ

**Q: How does the scaling work?**
The process involves three steps: first, `parse_measurement` converts your input to a metric base; second, `execute_scaling` multiplies that amount by your factor; and finally, the result is reformatted into readable units.

**Q: Can I use fractions like '1 1/2'?**
Yes, the `parse_measurement` tool is specifically designed to handle whole numbers, decimals, and mixed fractions.

**Q: What kind of units are supported?**
The tool supports both volume (e.g., cups, tbsp, tsp, ml) and mass (e.g., g, kg, oz, lb) measurements.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/smart-recipe-scaler](https://vinkius.com/mcp/smart-recipe-scaler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Smart Recipe Scaler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `smart-recipe-scaler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Smart Recipe Scaler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "smart-recipe-scaler": {
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
