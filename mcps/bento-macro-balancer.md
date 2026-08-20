# Bento Macro Balancer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/bento-macro-balancer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate precise nutritional profiles and traditional balance ratios for Japanese bento boxes.

## Description
This MCP server provides deterministic nutritional analysis for traditional Japanese bento boxes. Use `analyze_bento_nutrition` to calculate total calories, protein, carbs, and fat, while automatically flagging high-calorie meals or high-sodium content from pickled items. You can also use `check_bento_balance` to verify if your meal adheres to the traditional 4:3:2:1 weight ratio (Carbs:Protein:Veg:Pickles), or `list_available_items` to see the nutritional constants for allowed ingredients like white rice, salmon, and broccoli.


## Available Tools (3)
- **analyze_bento_nutrition**: Calculates the complete nutritional profile and health flags for a specific bento configuration
- **check_bento_balance**: Evaluates how closely the bento matches the traditional 4:3:2:1 weight ratio
- **list_available_items**: Provides the user with the valid list of items and their nutritional constants for reference


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bento Macro Balancer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the nutrition for a bento with 200g white rice, 100g salmon, 50g broccoli, and 10g pickled plum."

**🤖 AI Agent:**
> The total calories for your bento are 413 kcal, with 28.2g of protein, 58.3g of carbs, and 4.2g of fat.

---

**👤 You:**
> "Is a bento with 300g white rice, 150g salmon, 100g tamagoyaki, and 60g pickled plum balanced?"

**🤖 AI Agent:**
> The bento is not balanced according to the traditional 4:3:2:1 ratio, and it is flagged for high sodium because the pickled plum exceeds 50g.

---

**👤 You:**
> "What are the nutritional values for the available items?"

**🤖 AI Agent:**
> The available items are white rice (130kcal/100g), salmon (208kcal/100g), tamagoyaki (142kcal/100g), pickled plum (15kcal/100g), and broccoli (34kcal/100g).


## ❓ FAQ

**Q: How do I check if my bento is nutritionally balanced?**
You can use the `check_bento_balance` tool. It evaluates your components against the traditional Japanese 4:3:2:1 ratio to see how well they align.

**Q: What ingredients can I include in my calculation?**
The calculator supports a specific set of items: white rice, salmon, tamagoyaki, pickled plum, and broccoli. Use `list_available_items` to see the exact nutritional values for each.

**Q: Will the tool warn me about high calorie or high sodium meals?**
Yes. The `analyze_bento_nutrition` tool automatically flags meals exceeding 800 calories and alerts you if pickled items exceed 50g due to sodium concerns.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/bento-macro-balancer](https://vinkius.com/ai-agent-connect/bento-macro-balancer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bento Macro Balancer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bento-macro-balancer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bento Macro Balancer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bento-macro-balancer": {
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
