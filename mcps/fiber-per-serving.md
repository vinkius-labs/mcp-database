# Fiber Per Serving MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/fiber-per-serving)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculates fiber distribution per serving for nutritional planning.

## Description
This MCP server provides tools to analyze dietary fiber distribution. Use `get_fiber_per_serving` to calculate fiber per portion, `get_serving_nutritional_classification` to determine fiber density, `validate_serving_integrity` to ensure nutritional data is physically possible, and `get_bulk_fiber_distribution` to analyze multiple food items at once.


## Available Tools (4)
- **get_serving_nutritional_classification**: Determines if a single serving provides a significant amount of fiber based on established dietary standards
- **get_bulk_fiber_distribution**: Provides a breakdown of fiber across multiple different food items to assist in meal planning
- **get_fiber_per_serving**: Calculates the exact amount of fiber contained in a single serving of a food item
- **validate_serving_integrity**: Ensures that the provided nutritional data represents a physically possible food item


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fiber Per Serving** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much fiber is in each serving if there are 20g of fiber in 4 servings?"

**🤖 AI Agent:**
> Each serving contains 5g of fiber.

---

**👤 You:**
> "Is a serving with 8g of fiber considered high fiber?"

**🤖 AI Agent:**
> Yes, 8g of fiber per serving is classified as High.

---

**👤 You:**
> "Can a 100g food item have 150g of fiber?"

**🤖 AI Agent:**
> No, that is not a physically possible food item as the fiber mass cannot exceed the total weight.


## ❓ FAQ

**Q: How do I calculate fiber per serving?**
You can use the `get_fiber_per_serving` tool by providing the total fiber grams and the number of servings.

**Q: Can I check if my food data is realistic?**
Yes, the `validate_serving_integrity` tool checks if the fiber mass is logically consistent with the total weight of the food.

**Q: How is nutritional density determined?**
The `get_serving_nutritional_classification` tool classifies fiber density as High, Moderate, or Low based on established dietary standards.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/fiber-per-serving](https://vinkius.com/en/ai-agent-connect/fiber-per-serving)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fiber Per Serving** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fiber-per-serving` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fiber Per Serving** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fiber-per-serving": {
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
