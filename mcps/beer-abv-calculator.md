# Beer ABV Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/beer-abv-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate ABV, attenuation, calories, and beer style from gravity readings.

## Description
This MCP server provides precise tools for homebrewers to analyze fermentation data. Use `calculate_abv_metrics` to determine alcohol content, apparent attenuation, real extract, and caloric density. You can also use `convert_gravity_units` to switch between Specific Gravity and Plato, or `validate_fermentation_sanity` to ensure your gravity readings are physically realistic.


## Available Tools (3)
- **validate_fermentation_sanity**: Checks if the provided gravity readings are physically possible in a brewing context
- **calculate_abv_metrics**: Calculates primary fermentation metrics including alcohol content, attenuation, and caloric density
- **convert_gravity_units**: Converts a gravity measurement between Specific Gravity and Plato


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Beer ABV Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the ABV and metrics for a beer with an OG of 1.060 and an FG of 1.012."

**🤖 AI Agent:**
> The beer has an ABV of 5.76%, an apparent attenuation of 80%, and contains approximately 165 calories per 12oz serving. It is classified as a Standard style beer.

---

**👤 You:**
> "Convert 12.5 Plato to Specific Gravity."

**🤖 AI Agent:**
> 12.5 Plato is approximately 1.051 Specific Gravity.

---

**👤 You:**
> "Is it possible to have an OG of 1.050 and an FG of 1.055?"

**🤖 AI Agent:**
> No, that fermentation is not physically possible as the final gravity cannot be higher than the original gravity.


## ❓ FAQ

**Q: What units can I use for gravity?**
You can use either Specific Gravity (e.g., 1.050) or Plato (e.g., 12.5). The `calculate_abv_metrics` tool handles both automatically.

**Q: How is the beer style determined?**
The style (Session, Standard, Strong, or Imperial) is automatically assigned based on the calculated ABV percentage.

**Q: Can I check if my gravity readings are valid?**
Yes, use the `validate_fermentation_sanity` tool to check if your original and final gravity readings are physically possible.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/beer-abv-calculator](https://vinkius.com/ai-agent-connect/beer-abv-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Beer ABV Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `beer-abv-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Beer ABV Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "beer-abv-calculator": {
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
