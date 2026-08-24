# Sushi Rice & Ingredient Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/sushi-rice-ingredient-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate exact quantities of uncooked rice, seasoning, nori, and protein for sushi production.

## Description
This MCP server provides deterministic calculations for sushi preparation. It determines the exact mass of uncooked rice and seasoned vinegar using specific hydration and seasoning ratios. It also calculates the necessary nori sheets and protein weights for various sushi styles including nigiri, maki, uramaki, and temaki. Use `rice_requirements` to get rice and seasoning totals, `nori_requirements` for seaweed counts, and `ingredient_weights` for protein mass.


## Available Tools (3)
- **ingredient_weights**: Calculate protein/filling weight requirements
- **nori_requirements**: Calculate nori sheet requirements
- **rice_requirements**: Calculate uncooked rice and seasoning requirements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sushi Rice & Ingredient Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much uncooked rice and seasoning do I need for 20 pieces of nigiri?"

**🤖 AI Agent:**
> For 20 pieces of nigiri, you will need 171.43g of uncooked rice and 30g of seasoning (consisting of 20g vinegar, 10g sugar, and 5g salt).

---

**👤 You:**
> "How many nori sheets are needed for 10 maki rolls?"

**🤖 AI Agent:**
> You will need 5 full nori sheets for 10 maki rolls.

---

**👤 You:**
> "How much fish do I need for 5 temaki cones?"

**🤖 AI Agent:**
> You will need the specific protein weight calculated for temaki to ensure a balanced cone.


## ❓ FAQ

**Q: How does the rice calculation work?**
The tool calculates uncooked rice weight by accounting for the water-to-rice ratio (1:1.1) and then determines the seasoning (su) based on 10% of the cooked rice weight.

**Q: What sushi types are supported?**
The calculator supports nigiri, maki, uramaki, and temaki.

**Q: Can I calculate protein requirements?**
Yes, use the `ingredient_weights` tool to find the required mass of protein or filling for your specific sushi type.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/sushi-rice-ingredient-calculator](https://vinkius.com/ai-agent-connect/sushi-rice-ingredient-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sushi Rice & Ingredient Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sushi-rice-ingredient-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sushi Rice & Ingredient Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sushi-rice-ingredient-calculator": {
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
