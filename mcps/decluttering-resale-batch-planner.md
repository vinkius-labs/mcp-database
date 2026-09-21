# Decluttering & Resale Batch Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/decluttering-resale-batch-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Categorize household items into keep, resale, donate, recycle, or discard batches with logistical insights.

## Description
This MCP server acts as a logistical decision engine to help you manage household decluttering. By evaluating utility, sentimental value, condition, and space impact, it organizes items into actionable batches. Use `plan_decluttering_batches` to generate a full plan including recovered value and volume released, or `analyze_item_feasibility` to check a specific item. It also provides tools like `calculate_logistics_impact` to estimate disposal costs and `get_processing_sequence` to determine the most efficient order to clear physical space.


## Available Tools (4)
- **analyze_item_feasibility**: Evaluates a single item to determine its most likely category
- **calculate_logistics_impact**: Calculates the physical and financial consequences of a proposed batch of removals
- **get_processing_sequence**: Determines the most efficient order to process items to clear physical space quickly
- **plan_decluttering_batches**: Generates the complete decluttering plan for a collection of items


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Decluttering & Resale Batch Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan a decluttering session for these items: [{ "name": "Old Sofa", "utility": 2, "sentimental": 1, "condition": 3, "space_impact": 10, "market_value": 50 }, { "name": "Vintage Lamp", "utility": 5, "sentimental": 8, "condition": 5, "space_impact": 2, "market_value": 120 }]. Set a minimum resale price of 40."

**🤖 AI Agent:**
> Your decluttering plan is ready. The Old Sofa will be placed in the discard batch, releasing 10 units of volume. The Vintage Lamp will be placed in the resale batch, contributing $120 to your recovered value.

---

**👤 You:**
> "Is this item worth reselling: { "name": "Toaster", "utility": 4, "sentimental": 1, "condition": 4, "space_impact": 1, "market_value": 15 }? My minimum price is 20."

**🤖 AI Agent:**
> No, the Toaster is not suitable for resale because its market value of $15 is below your minimum price of $20. It will likely be categorized for donation.

---

**👤 You:**
> "What is the most efficient order to clear my room starting with these items: [{ "name": "Box of Books", "space_impact": 5, "condition": 4 }, { "name": "Large Desk", "space_impact": 15, "condition": 3 }]?"

**🤖 AI Agent:**
> To maximize space release quickly, you should process the Large Desk first, followed by the Box of Books.


## ❓ FAQ

**Q: How does the tool decide what to resell?**
An item is moved to the resale batch only if its condition is high and its estimated market value meets or exceeds your specified `minResalePrice`.

**Q: Can I prioritize clearing space over making money?**
Yes, you can use `plan_decluttering_batches` with user preferences to prioritize space release, which focuses on items with high space impact.

**Q: What information do I need to provide for an item?**
To get accurate results, provide the item's utility, sentimental value, condition, space impact, and estimated market value.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/decluttering-resale-batch-planner](https://vinkius.com/en/ai-agent-connect/decluttering-resale-batch-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Decluttering & Resale Batch Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `decluttering-resale-batch-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Decluttering & Resale Batch Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "decluttering-resale-batch-planner": {
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
