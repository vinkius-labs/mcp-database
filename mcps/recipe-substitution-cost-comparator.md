# Recipe Substitution Cost Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/recipe-substitution-cost-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [nutrition](../categories/nutrition.md)

Compare ingredient substitutions by cost, availability, allergens, and serving impact.

## Description
This MCP server provides tools to evaluate ingredient substitutions in recipes. It calculates the required quantity based on conversion ratios, determines total cost, checks ingredient availability, and verifies allergen safety. You can use `get_substitution_analysis` for single replacements, `compare_multiple_substitutions` to rank several options, `validate_allergen_profile` for dietary safety, and `calculate_yield_adjustment` to see how a change affects recipe servings.


## Available Tools (4)
- **calculate_yield_adjustment**: Determines how much the total volume/weight of a recipe changes due to a substitution
- **compare_multiple_substitutions**: Ranks a list of potential ingredient replacements to find the most cost-effective and safe option
- **validate_allergen_profile**: Checks if a specific ingredient contains any prohibited allergens based on a user's provided list
- **get_substitution_analysis**: Evaluates a single substitution against an original ingredient to determine cost, quantity, and dietary safety


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Recipe Substitution Cost Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to replace 200g of butter with margarine. Margarine costs 0.05 per gram and I have 500g in stock. The conversion ratio is 1.1. How much will it cost and is it available?"

**🤖 AI Agent:**
> You will need 220g of margarine, which will cost 11.00. The required quantity is available in your stock.

---

**👤 You:**
> "Compare replacing 100g of flour with almond flour (0.1/g, 50g stock, 1.2 ratio) vs cornstarch (0.02/g, 100g stock, 1.0 ratio)."

**🤖 AI Agent:**
> The best option is cornstarch. It is the cheapest option at 2.00 and is fully available.

---

**👤 You:**
> "If I replace 500ml of milk with 400ml of coconut milk for a recipe that serves 4, how many servings will I get?"

**🤖 AI Agent:**
> The adjusted serving count is 3.2 servings.


## ❓ FAQ

**Q: How does the tool handle different ingredient ratios?**
The `get_substitution_analysis` tool uses a conversion ratio to calculate the exact amount of the replacement ingredient needed to match the original recipe's requirements.

**Q: Can I compare multiple ingredients at once?**
Yes, use `compare_multiple_substitutions` to provide a list of options. The tool will rank them based on cost, safety, and availability.

**Q: How are allergens checked?**
The `validate_allergen_profile` tool checks ingredients against a provided list of prohibited allergens to ensure dietary safety.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/recipe-substitution-cost-comparator](https://vinkius.com/en/ai-agent-connect/recipe-substitution-cost-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Recipe Substitution Cost Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `recipe-substitution-cost-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Recipe Substitution Cost Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "recipe-substitution-cost-comparator": {
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
