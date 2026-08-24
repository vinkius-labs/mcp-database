# Fabric Dye Mixing Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/fabric-dye-mixing-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [chemistry](../categories/chemistry.md)

Deterministic textile dye formulation and bath parameter calculator.

## Description
This MCP server provides precise tools for textile dye formulation. It calculates the exact mass of dye powders needed based on fabric weight and target color ratios, determines required water volumes using liquor ratios, and computes necessary chemical modifiers like salt and soda ash. Use `calculate_dye_formulation` to determine dye weights, `calculate_bath_parameters` for water and modifiers, and `validate_recipe_consistency` to ensure industrial safety standards.


## Available Tools (3)
- **calculate_bath_parameters**: Calculate total water volume and required chemical modifiers
- **calculate_dye_formulation**: Determine the exact mass of each individual dye powder required
- **validate_recipe_consistency**: Verify if a completed recipe adheres to safe industrial manufacturing standards


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fabric Dye Mixing Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the dye weights for 500g of fabric with a 2% concentration and a color ratio of 70% Red and 30% Blue."

**🤖 AI Agent:**
> For 500g of fabric at 2% concentration, you need 10g of total dye. This consists of 7g of Red dye and 3g of Blue dye.

---

**👤 You:**
> "What are the bath parameters for 1000g of fabric with a 20:1 liquor ratio and 5% salt concentration?"

**🤖 AI Agent:**
> For 1000g of fabric with a 20:1 liquor ratio, you need 20000ml of water and 50g of salt.

---

**👤 You:**
> "Is a recipe with 10g dye, 100g fabric, and 500ml water safe?"

**🤖 AI Agent:**
> The recipe is valid and meets the required safety standards for even dye distribution.


## ❓ FAQ

**Q: How do I calculate the amount of dye needed?**
You can use the `calculate_dye_formulation` tool. Provide the dry fabric weight, the target color ratios (as a JSON array of dye names and percentages), and the total concentration percentage.

**Q: What is a liquor ratio?**
A liquor ratio is the relationship between the weight of the fabric and the volume of water in the dye bath. For example, a 20:1 ratio means 20ml of water for every 1g of fabric.

**Q: Can I verify if my recipe is safe for production?**
Yes, the `validate_recipe_consistency` tool checks if your dye weight, fabric weight, and water volume meet safe industrial manufacturing standards.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/fabric-dye-mixing-calculator](https://vinkius.com/ai-agent-connect/fabric-dye-mixing-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fabric Dye Mixing Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fabric-dye-mixing-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fabric Dye Mixing Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fabric-dye-mixing-calculator": {
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
