# Fermentation Salt Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/fermentation-salt-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [food-science](../categories/food-science.md)

Calculate precise salt quantities for dry-salt, brine, or mixed fermentation batches.

## Description
This MCP server provides precise salt calculations for various fermentation methods. Use `get_dry_salt_requirements` for direct vegetable salting, `get_brine_only_requirements` for liquid brine preparation, and `get_mixed_fermentation_requirements` for combined vegetable and brine batches. You can also use `scale_batch_to_vessel` to adjust your recipe to fit specific container sizes.

### Available Tools

`dry_salt_tool`, `brine_only_tool`, `mixed_fermentation_tool`, `scale_batch_tool`


## Available Tools (4)
- **brine_only_tool**: Calculates the salt needed to create a specific volume of liquid brine
- **dry_salt_tool**: Calculates the amount of salt needed for direct application to vegetables
- **mixed_fermentation_tool**: Calculates salt requirements for batches involving both solid vegetables and a liquid brine
- **scale_batch_tool**: Adjusts ingredient quantities to fit the physical limits of a container


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fermentation Salt Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much salt do I need for 500g of cabbage at 2% salinity using dry salt?"

**🤖 AI Agent:**
> You need 10 grams of salt for 500g of cabbage at 2% salinity.

---

**👤 You:**
> "I have 1000g of water. How much salt is needed for a 3% brine?"

**🤖 AI Agent:**
> You need 30.93 grams of salt to create a 3% brine with 1000g of water.

---

**👤 You:**
> "Scale my batch of 400g vegetables and 200g water to fit a 1000g vessel at 2.5% salinity."

**🤖 AI Agent:**
> To fit your 1000g vessel at 2.5% salinity, you should use 634.92g of vegetables and 315.08g of water.


## ❓ FAQ

**Q: How do I calculate salt for vegetables without adding water?**
You can use the `get_dry_salt_requirements` tool by providing the weight of your vegetables and your target salinity percentage. Tools available: `dry_salt_tool`, `brine_only_tool`, `mixed_fermentation_tool`.

**Q: Can I adjust my recipe to fit a specific jar?**
Yes, use the `scale_batch_to_vessel` tool. Input your current ingredient masses and the maximum capacity of your vessel to get the adjusted quantities.

**Q: What is the difference between brine and mixed fermentation?**
Brine-only fermentation uses a pre-made liquid solution, while mixed fermentation calculates salt for both the solid vegetables and the liquid brine combined.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/fermentation-salt-calculator](https://vinkius.com/en/ai-agent-connect/fermentation-salt-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fermentation Salt Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fermentation-salt-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fermentation Salt Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fermentation-salt-calculator": {
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
