# Cake Serving Sizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cake-serving-sizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utility](../categories/utility.md)

Calculate exact cake tier combinations and serving yields using Wilton standards.

## Description
The Cake Serving Sizer is a precision planning tool for bakers and event planners. Using industry-standard Wilton catering charts, it helps you determine the exact dimensions needed for your celebration. Use `calculate_required_tiers` to generate a multi-tier plan based on your guest count and preferred serving style (wedding or party). If you already have tiers, use `calculate_tier_yield` to find out how many people a single tier can feed, or `calculate_stack_yield` to calculate the total capacity of an entire cake stack. The tool supports round, square, and hexagonal geometries.


## Available Tools (3)
- **calculate_required_tiers**: Suggests a combination of tiers to meet a target guest count
- **calculate_stack_yield**: Calculates total servings for an existing multi-tier cake
- **calculate_tier_yield**: Calculates how many people a single tier can feed


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cake Serving Sizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many people can a 10-inch round cake feed using wedding servings?"

**🤖 AI Agent:**
> A 10-inch round cake provides approximately 39 wedding servings.

---

**👤 You:**
> "I need to feed 50 guests with square cakes. What tiers do I need for party servings?"

**🤖 AI Agent:**
> You need a 2-tier cake: 10" and 6" square tiers.

---

**👤 You:**
> "Calculate the yield of an 8-inch square tier for party style."

**🤖 AI Agent:**
> An 8-inch square tier yields 16 party servings.


## ❓ FAQ

**Q: What is the difference between wedding and party servings?**
Wedding servings are 1x2 inch slices, while party servings are larger 2x2 inch slices.

**Q: Does the tool support hexagonal cakes?**
Yes, you can calculate yields for round, square, and hexagonal tiers using `calculate_tier_yield`.

**Q: How do I plan a multi-tier cake for 100 guests?**
Use the `calculate_required_tiers` tool by providing a target guest count of 100 and your preferred serving type.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cake-serving-sizer](https://vinkius.com/mcp/cake-serving-sizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cake Serving Sizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cake-serving-sizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cake Serving Sizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cake-serving-sizer": {
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
