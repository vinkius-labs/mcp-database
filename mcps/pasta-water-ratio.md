# Pasta Water Ratio MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pasta-water-ratio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [culinary](../categories/culinary.md)

Calculate the perfect water volume, salt concentration, and cooking time for any pasta shape.

## Description
Achieve professional results every time with precise cooking parameters. This MCP server provides tools like `get_ideal_ratios` to determine the exact water, salt, and duration needed for specific pasta shapes and thicknesses. You can also use `verify_salinity` to check if your seasoning is correct or `assess_texture_risk` to prevent overcooking.


## Available Tools (3)
- **verify_salinity**: Verify if the salt concentration in pasta water is optimal
- **assess_texture_risk**: Assess the risk of pasta being overcooked or undercooked
- **get_ideal_ratios**: Calculate ideal cooking parameters for a specific pasta shape and thickness


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pasta Water Ratio** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the ideal cooking settings for medium thickness penne?"

**🤖 AI Agent:**
> You should use `get_ideal_rasios` with pastaShape='penne' and thicknessCategory='medium'. This will provide the exact water volume, salt grams per liter, and cooking duration.

---

**👤 You:**
> "I added 20g of salt to 2 liters of water. Is this correct?"

**🤖 AI Agent:**
> You can check this using `verify_salinity` with totalWaterLiters=2 and saltGrams=20 to see if the salinity is optimal.

---

**👤 You:**
> "My spaghetti has been cooking for 12 minutes. Am I overcooking it?"

**🤖 AI Agent:**
> Use the `assess_texture_risk` tool with pastaShape='spaghetti', thicknessCategory='medium', and minutesCooked=12 to check your current texture state.


## ❓ FAQ

**Q: How do I know if my pasta water is properly salted?**
Use the `verify_salinity` tool by providing the total liters of water and grams of salt added. It will tell you if your salinity is optimal.

**Q: Can I use this for different pasta thicknesses?**
Yes. The `get_ideal_ratios` tool allows you to specify thickness categories like thin, medium, or thick to get accurate results.

**Q: How can I prevent my pasta from becoming overcooked?**
You can use the `assess_texture_risk` tool. By inputting your pasta shape, thickness, and minutes cooked, you can see if you are approaching the overcooked state.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pasta-water-ratio](https://vinkius.com/mcp/pasta-water-ratio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pasta Water Ratio** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pasta-water-ratio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pasta Water Ratio** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pasta-water-ratio": {
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
