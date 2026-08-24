# Gemstone Weight Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/gemstone-weight-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Estimate gemstone carat weight and market value using physical dimensions.

## Description
This MCP server provides precise tools for gemstone professionals and enthusiasts to calculate mass and value. By using the `estimate_carat_weight` tool, you can determine the carat weight of a stone by providing its shape, length, width, depth, and material type. The server also includes `calculate_gemstone_value` to estimate market price and `get_gemstone_specifications` to retrieve specific gravity and shape correction factors.


## Available Tools (3)
- **calculate_gemstone_value**: Determines the estimated market price range for a gemstone
- **estimate_carat_weight**: Calculates the estimated carat weight of a gemstone based on its physical dimensions and material type
- **get_gemstone_specifications**: Retrieves the physical constants (specific gravity) and correction factors for a given gemstone and shape combination


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gemstone Weight Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the estimated weight of a round diamond that is 6mm long, 6mm wide, and 3.5mm deep?"

**🤖 AI Agent:**
> The estimated weight for a round diamond with those dimensions is 0.68 carats.

---

**👤 You:**
> "Calculate the value of a 2.5 carat sapphire if the price per carat is $500."

**🤖 AI Agent:**
> The estimated market value for the sapphire is $1,250.00.

---

**👤 You:**
> "What is the specific gravity for an emerald?"

**🤖 AI Agent:**
> The specific gravity for an emerald is 2.72.


## ❓ FAQ

**Q: How accurate are these weight estimates?**
Estimates are calculated using deterministic formulas based on specific gravity and shape-specific correction factors provided by the `get_gemstone_specifications` tool.

**Q: Which gemstone types are supported?**
The tool supports diamond, ruby, sapphire, emerald, amethyst, topaz, garnet, opal, and pearl.

**Q: Can I calculate the price of a stone?**
Yes, you can use the `calculate_gemstone_value` tool by providing the estimated carat weight and the current market rate per carat.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/gemstone-weight-calculator](https://vinkius.com/ai-agent-connect/gemstone-weight-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gemstone Weight Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gemstone-weight-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gemstone Weight Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gemstone-weight-calculator": {
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
