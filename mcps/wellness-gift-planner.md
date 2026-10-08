# Wellness Gift Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wellness-gift-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [e-commerce](../categories/e-commerce.md)

Select perfect wellness gift combinations based on budget, preferences, and delivery dates.

## Description
This MCP server helps you curate thoughtful wellness gift packages. Use `get_available_gifts` to browse items, `calculate_best_combinations` to find sets that fit your budget and recipient preferences, and `get_shipping_estimates` to determine delivery costs. You can also use `validate_gift_selection` to ensure your chosen items meet all constraints before finalizing.


## Available Tools (4)
- **get_available_gifts**: Retrieves a list of all wellness gift items currently available for selection
- **get_shipping_estimates**: Provides shipping options or confirms the cost of delivery for the selected items
- **validate_gift_selection**: Verifies if a specific selection of gifts is feasible under current constraints
- **calculate_best_combinations**: Finds the most suitable sets of gift items based on budget, preferences, and time constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wellness Gift Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find me some relaxation gifts for under $50 that can arrive by next Friday."

**🤖 AI Agent:**
> I found a combination including a Lavender Essential Oil kit and a Weighted Eye Mask for a total of $42.00, which fits your $50 budget and will arrive by next Friday.

---

**👤 You:**
> "What are the available fitness gifts?"

**🤖 AI Agent:**
> The available fitness gifts are a Yoga Mat, Resistance Bands, and a Foam Roller.

---

**👤 You:**
> "Is a selection of a Zen Candle and a Mindfulness Journal valid for a $30 budget with $5 shipping?"

**🤖 AI Agent:**
> Yes, the total cost is $28.00, which is within your $30 budget.


## ❓ FAQ

**Q: How do I find gifts that fit my budget?**
You can use the `calculate_best_combinations` tool by providing your maximum budget and recipient preferences to see valid options.

**Q: Can I check if my gift selection will arrive on time?**
Yes, use `validate_gift_selection` with your target delivery date to verify if the items will arrive when needed.

**Q: How are shipping costs calculated?**
Shipping costs can be determined using the `get_shipping_estimates` tool for your specific list of gift IDs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wellness-gift-planner](https://vinkius.com/en/ai-agent-connect/wellness-gift-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wellness Gift Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wellness-gift-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wellness Gift Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wellness-gift-planner": {
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
