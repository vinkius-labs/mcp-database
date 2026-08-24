# IBU & SRM Brewing Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/ibu-srm-brewing-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Calculate beer bitterness (IBU) and color (SRM) using deterministic brewing formulas.

## Description
This MCP server provides precise brewing calculations for beer production. Use `calculate_bitterness` to determine the total International Bitterness Units (IBU) and the specific contribution of each hop addition based on the Tinseth formula. Use `calculate_color` to predict the final SRM color and its descriptive classification (pale, gold, amber, copper, or dark) using the Morey equation. Additionally, `simulate_boil_process` allows you to predict volume loss due to evaporation during the boil.


## Available Tools (3)
- **calculate_bitterness**: Calculate total bitterness (IBU) and contribution per hop addition
- **calculate_color**: Calculate final SRM color and its description
- **simulate_boil_process**: Predict final volume and volume lost during boil


## 💬 Prompt Examples

Here are some examples of how you can interact with the **IBU & SRM Brewing Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the bitterness for a batch of 5 gallons with 10g of hops at 10% alpha acid boiled for 60 minutes and an OG of 1.050."

**🤖 AI Agent:**
> The total bitterness for this batch is 32.5 IBU.

---

**👤 You:**
> "What will be the color of a beer made with 5kg of malt at 10 Lovibond in a 20 liter batch?"

**🤖 AI Agent:**
> The estimated color is 12.4 SRM, which is classified as amber.

---

**👤 You:**
> "If I start with 30 liters and boil for 60 minutes with a 10% boil-off rate, what is my final volume?"

**🤖 AI Agent:**
> Your final volume will be 27 liters, with a total volume lost of 3 liters.


## ❓ FAQ

**Q: How is the bitterness calculated?**
Bitterness is calculated using the Tinseth formula, which accounts for hop weight, alpha acid percentage, boil time, and the original gravity of the wort.

**Q: What determines the color of the beer?**
The color is determined by the Malting Color Units (MCU) of the grain bill, which is then converted to SRM using the Morey equation.

**Q: Can I predict evaporation loss?**
Yes, you can use the `simulate_boil_process` tool to predict the final volume and total volume lost based on your boil-off rate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/ibu-srm-brewing-calculator](https://vinkius.com/ai-agent-connect/ibu-srm-brewing-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **IBU & SRM Brewing Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ibu-srm-brewing-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **IBU & SRM Brewing Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ibu-srm-brewing-calculator": {
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
