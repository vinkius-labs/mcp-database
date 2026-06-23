# Ingredient Substitution Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ingredient-substitution-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [nutrition](../categories/nutrition.md)

Find dietary-friendly ingredient alternatives with usage ratios and sensory impact analysis.

## Description
The Ingredient Substitution Engine is a specialized culinary intelligence tool designed to help cooks and food scientists navigate dietary restrictions. By using tools like `search_substitutes`, you can find compatible ingredients for constraints such as Vegan, GlutenFree, or LactoseFree. The engine also provides deep insights through `analyze_substitution_impact`, detailing how a replacement affects the texture and flavor of your dish. Additionally, use `verify_restriction_compatibility` to ensure that any chosen substitute does not introduce new allergens or dietary violations into your recipe.


## Available Tools (3)
- **analyze_substitution_impact**: Analyze the sensory impact of a substitution
- **search_substitutes**: Find compatible ingredients for a dietary constraint
- **verify_restriction_compatibility**: Verify if a substitute meets all dietary requirements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ingredient Substitution Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I need a vegan substitute for milk. What are my options?"

**🤖 AI Agent:**
> You can use soy milk, almond milk, or oat milk as substitutes for dairy milk in a vegan recipe.

---

**👤 You:**
> "If I replace wheat flour with almond flour, how will it affect the texture?"

**🤖 AI Agent:**
> Replacing wheat flour with almond flour will change the texture from elastic and chewy to more gritty and crumbly.

---

**👤 You:**
> "Is cashew butter safe for a recipe that must be both GlutenFree and LactoseFree?"

**🤖 AI Agent:**
> Yes, cashew butter is safe as it does not contain gluten or lactose.


## ❓ FAQ

**Q: How do I find alternatives for an ingredient?**
Use the `search_substitutes` tool by providing the name of the ingredient and your specific dietary restriction, such as 'Vegan'.

**Q: Can I see how a substitution will change my recipe's texture?**
Yes, the `analyze_substitution_impact` tool provides detailed information on changes to mouthfeel and flavor profiles.

**Q: How do I ensure a substitute is safe for all my dietary needs?**
You can use the `verify_restriction_compatibility` tool to check if an ingredient adheres to a list of multiple constraints simultaneously.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ingredient-substitution-engine](https://vinkius.com/mcp/ingredient-substitution-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ingredient Substitution Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ingredient-substitution-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ingredient Substitution Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ingredient-substitution-engine": {
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
