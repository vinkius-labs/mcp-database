# Pan Size Converter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pan-size-converter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate baking pan volumes and find perfect shape or size substitutions.

## Description
The Pan Size Converter MCP server provides AI agents with precise tools to manage baking consistency. By using `calculate_volume`, agents can determine the exact capacity of any pan shape. The `find_equivalent_pan` tool allows for intelligent substitutions, suggesting alternative pans that maintain the same volume within a specified tolerance. Additionally, `validate_dimensions` ensures all input measurements are physically plausible and compatible with the chosen geometry.


## Available Tools (3)
- **calculate_volume**: Calculates the total volumetric capacity of a specific pan
- **find_equivalent_pan**: Identifies alternative pan shapes and sizes with near-identical volume
- **validate_dimensions**: Verifies that a set of pan dimensions is physically plausible


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pan Size Converter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the volume of a 22cm round pan with 5cm depth?"

**🤖 AI Agent:**
> The calculated volume for a round pan with a 22cm diameter and 5cm depth is approximately 1900.66 cm³.

---

**👤 You:**
> "Find an alternative for a square pan that is 20cm by 5cm."

**🤖 AI Agent:**
> A suitable alternative found via `find_equivalent_pan` is a round pan with a diameter of approximately 17.8cm and 5cm depth.

---

**👤 You:**
> "Check if these dimensions are valid for a rectangular pan: [20, 10, 5]."

**🤖 AI Agent:**
> The `validate_dimensions` tool confirms that the dimensions [20, 10, 5] are valid for a rectangular pan.


## ❓ FAQ

**Q: How can I find a different pan for my recipe?**
Use the `find_equivalent_pan` tool. Provide your current pan's shape and dimensions, and the tool will suggest alternatives with similar volumes.

**Q: Does this tool support rectangular pans?**
Yes. By using `calculate_volume`, you can input three dimensions (length, width, and depth) for rectangular pans to find their capacity.

**Q: How accurate are the substitutions?**
You can control accuracy using the `tolerancePercentage` parameter in `find_equivalent_pan`. A lower percentage ensures a tighter volume match.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pan-size-converter](https://vinkius.com/mcp/pan-size-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pan Size Converter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pan-size-converter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pan Size Converter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pan-size-converter": {
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
