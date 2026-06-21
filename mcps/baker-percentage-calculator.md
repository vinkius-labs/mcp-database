# Baker Percentage Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/baker-percentage-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [baking](../categories/baking.md)

Convert baking recipes between absolute weights (grams) and professional Baker's percentages instantly, making scaling and comparison straightforward.

## Description
# Professional Recipe Standardization Tool

**Hook:** Have you ever struggled to compare a recipe from a European source (which uses Baker's percentages) with one from an American source (which uses absolute weights)? Or perhaps you need to scale a batch up or down while maintaining perfect proportions?

**Problem:** Baking recipes are highly specialized. Standard units of measure and percentage calculations make cross-regional comparison and professional scaling difficult. Simply measuring ingredients isn't enough; you need to understand the proportional relationship between components.

**Mechanism:** This tool provides three dedicated functions to manage this complexity:
1. **`recipe_to_baker_percentage`**: Takes your raw ingredient weights (e.g., 50g salt, 300g water) and calculates what their professional percentage is relative to the flour base.
2. **`scale_baker_percentage_to_weights`**: If you know a recipe's percentages but need to double or halve the batch size, this function accurately converts those ratios back into precise gram weights based on your scaling factor.
3. **`check_flour_base`**: This is an inverse solver. If you only measure one ingredient (like yeast) and know its percentage (e.g., 1%), this tool calculates the necessary total flour weight to make that measurement accurate.

The system uses these tools to maintain rigorous adherence to established baking standards, ensuring proportional accuracy every time.

**Advantage:** Stop guessing with recipes. Use this connector to transform any set of ingredient weights into standardized professional proportions or scale them precisely for commercial use.


## Available Tools
- **check_flour_base**: Calculate the flour base weight from a known ingredient weight and its Baker's percentage
- **recipe_to_baker_percentage**: Convert ingredient weights to Baker's percentages relative to flour weight
- **scale_baker_percentage_to_weights**: Scale Baker's percentages to absolute weights using a scaling factor


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Baker Percentage Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a batch with 400g of flour, 350g of water, and 12g of salt. Calculate the Baker's percentages for this recipe."

**🤖 AI Agent:**
> The scoring process is complete. The final calculated proportions are: Flour Base (100%), Water (87.50%), Salt (3.00%). This indicates a standard hydration level suitable for artisan loaves.

---

**👤 You:**
> "We need to double this recipe, which has 12g of salt (3% B%), and scale it up. What are the new weights?"

**🤖 AI Agent:**
> Scaling by a factor of 2.0 results in the following required weights: Salt: [NEW_SALT_WEIGHT] grams, Water: [NEW_WATER_WEIGHT] grams. The proportions are maintained.

---

**👤 You:**
> "I used 5g of yeast and know its professional percentage is 1.2%. What was the approximate total flour weight?"

**🤖 AI Agent:**
> Based on your input, the calculated necessary flour base weight is [CALCULATED_FLOUR_WEIGHT] grams. Please note that this batch size is small (< 5g warning).


## ❓ FAQ

**Q: How does the tool handle scaling a recipe?**
You use the `scale_baker_percentage_to_weights` function. You provide the desired batch size multiplier and an array of ingredients with their known percentages. The tool calculates the new absolute weights for every ingredient, ensuring perfect proportionality.

**Q: What is the primary input required for calculating Baker's Percentages?**
The `recipe_to_baker_percentage` tool requires two main inputs: the absolute weight of the flour base (in grams) and a list of all other ingredient weights. The flour weight always serves as the 100% reference point.

**Q: If I only know one ingredient's weight, how can I find the required flour base?**
Use the `check_flour_base` tool. You must provide the name of your known ingredient, its measured weight in grams, and its established professional percentage relative to flour. The function then calculates the necessary flour base weight.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/baker-percentage-calculator](https://vinkius.com/mcp/baker-percentage-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Baker Percentage Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `baker-percentage-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Baker Percentage Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "baker-percentage-calculator": {
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
