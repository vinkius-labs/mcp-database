# Hops Bitterness Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/hops-bitterness-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Calculate precise IBU and BU:GU ratios for beer recipes.

## Description
This MCP server provides professional brewing tools to calculate International Bitterness Units (IBU) and the Bitterness-to-Gravity (BU:GU) ratio. It supports multiple utilization models including Tinseth, Rager, and Daniels. Use `calculate_single_addition_ibu` to find the bitterness contribution of specific hop additions, or `calculate_total_recipe_bitterness` to evaluate the balance of an entire recipe based on hop weight, alpha acid percentage, and wort gravity.


## Available Tools (3)
- **calculate_total_recipe_bitterness**: Aggregates multiple hop additions to find the total IBU and the BU:GU ratio
- **get_utilization_factors**: Retrieves the theoretical utilization multiplier constants
- **calculate_single_addition_ibu**: Calculates the specific IBU contribution of a single hop addition


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hops Bitterness Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the IBU for 50g of 12% alpha acid pellets boiled for 60 minutes in 20L of wort with 1.050 gravity."

**🤖 AI Agent:**
> The bitterness contribution for this addition is 42.5 IBU.

---

**👤 You:**
> "What is the BU:GU ratio for a recipe with 45 total IBU and a final gravity of 1.060?"

**🤖 AI Agent:**
> The BU:GU ratio is 0.75.

---

**👤 You:**
> "Calculate the IBU for 30g of 5% alpha acid whole leaf hops added during whirlpool in 25L of wort at 1.040 gravity."

**🤖 AI Agent:**
> The bitterness contribution for this whirlpool addition is 4.2 IBU.


## ❓ FAQ

**Q: How do I calculate the total bitterness of my recipe?**
You can use the `calculate_total_recipe_bitterness` tool. Provide an array of your hop additions and the final wort gravity to get the total IBU and the BU:GU ratio.

**Q: Does dry hopping contribute to IBU?**
No, dry hopping additions contribute zero IBU as they are added after fermentation and do not undergo the isomerization process.

**Q: Which utilization models are supported?**
The server supports the Tinseth, Rager, and Daniels utilization models to accommodate different brewing styles and wort gravities.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/hops-bitterness-calculator](https://vinkius.com/ai-agent-connect/hops-bitterness-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hops Bitterness Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hops-bitterness-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hops Bitterness Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hops-bitterness-calculator": {
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
