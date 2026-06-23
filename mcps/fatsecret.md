# FatSecret MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fatsecret)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Access millions of food items with calorie tracking, macro data, and serving sizes from the FatSecret platform used by 30M+ users worldwide.

## Description
The **FatSecret MCP Server** connects your AI agent to one of the world's most popular food tracking platforms — trusted by 30 million+ users for diet management and calorie counting.

### Core Capabilities

- **Food Search** — Find any food by name across a massive database of generic and branded products.
- **Detailed Nutrition** — Full macro breakdown per serving: calories, protein, fat, and carbohydrates.
- **Multiple Serving Sizes** — Every food includes multiple serving size options (per cup, per 100g, per piece, etc.).
- **Brand Coverage** — Extensive branded product database including restaurant chains and packaged goods.

Free developer plan available. OAuth 2.0 client credentials authentication.


## Available Tools (2)
- **get_fatsecret_food_details**: g. 1 cup, 100g, 1 oz).

Get detailed nutritional information for a specific food item with all serving sizes
- **search_fatsecret_foods**: Returns calorie, protein, fat, and carb data per serving. Popular with fitness and diet tracking apps worldwide.

Search the FatSecret food database for foods with calorie and macro data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FatSecret** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many calories in a Big Mac?"

**🤖 AI Agent:**
> According to FatSecret data, a McDonald's Big Mac contains 563 calories per serving (215g). Breakdown: 33g fat, 44g carbs, and 26g protein.

---

**👤 You:**
> "Search for the nutrition data of a medium apple."

**🤖 AI Agent:**
> A medium apple (182g) has approximately 95 calories, 0.3g of fat, 25g of carbohydrates (including 4.4g of fiber), and 0.5g of protein.

---

**👤 You:**
> "What are the macros for a serving of whey protein powder?"

**🤖 AI Agent:**
> A typical 30g scoop of whey protein powder contains roughly 110-120 calories, with 24g of protein, 2g of carbohydrates, and 1.5g of fat.


## ❓ FAQ

**Q: How do I get FatSecret API access?**
Register at platform.fatsecret.com for a free developer account. You'll receive a Client ID and Client Secret for OAuth 2.0 authentication.

**Q: Does FatSecret include data on restaurant chains and packaged foods?**
Yes, the database includes a vast array of branded products, restaurant chains, and generic foods from around the world.

**Q: Are multiple serving sizes supported for foods?**
Yes, most foods in the platform have multiple serving size options available, such as per 100g, per piece, or per cup, giving you highly accurate portion logging.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fatsecret](https://vinkius.com/mcp/fatsecret)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FatSecret** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fatsecret` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FatSecret** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fatsecret": {
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
