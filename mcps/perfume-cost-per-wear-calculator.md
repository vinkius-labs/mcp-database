# Perfume Cost Per Wear Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/perfume-cost-per-wear-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate fragrance cost per spray, wear, month, and year.

## Description
This MCP server provides tools to analyze fragrance value and usage. Use `calculate_single_perfume_metrics` to find the cost per spray and wear based on bottle volume and price. Use `compare_perfume_value` to rank multiple fragrances by their cost efficiency. You can also `estimate_longevity` to predict how many months a bottle will last or `get_spray_efficiency_rating` to understand atomizer density.


## Available Tools (4)
- **calculate_single_perfume_metrics**: Calculates all cost and usage metrics for a single fragrance bottle
- **compare_perfume_value**: Compares two or more perfumes to determine which offers better value
- **estimate_longevity**: Predicts how many months or years a bottle will last based on usage habits
- **get_spray_efficiency_rating**: Categorizes how efficient a perfume's atomizer is in terms of liquid delivery


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Perfume Cost Per Wear Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much will a 100ml bottle of perfume costing $200 cost me per wear if I use 3 sprays per wear, 4 times a week, and each spray is 0.1ml?"

**🤖 AI Agent:**
> Based on your usage, the cost per spray is $0.50, making the cost per wear $1.50. You will use the bottle in approximately 167 weeks.

---

**👤 You:**
> "Which is a better value: a 50ml bottle for $100 with 2 sprays per wear, or a 100ml bottle for $180 with 4 sprays per wear? (Assume 0.1ml per spray)"

**🤖 AI Agent:**
> The 50ml bottle is the better value with a cost per wear of $1.00, compared to $1.80 for the 100ml bottle.

---

**👤 You:**
> "How long will my 50ml perfume last if I use 2 sprays every single day and each spray is 0.1ml?"

**🤖 AI Agent:**
> Your 50ml bottle will last approximately 250 days, which is about 8 months.


## ❓ FAQ

**Q: How is the cost per wear calculated?**
The tool calculates the total usable volume by subtracting waste, then divides the price by the total number of sprays to get the cost per spray. The cost per wear is then the cost per spray multiplied by your sprays per use.

**Q: Can I compare multiple perfumes at once?**
Yes, you can use the `compare_perfume_value` tool to provide a list of perfumes and receive a ranking based on the lowest cost per wear.

**Q: What is the waste percentage?**
The waste percentage accounts for liquid lost to evaporation or residue left in the bottle pump, ensuring your cost calculations reflect the actual usable liquid.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/perfume-cost-per-wear-calculator](https://vinkius.com/en/ai-agent-connect/perfume-cost-per-wear-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Perfume Cost Per Wear Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `perfume-cost-per-wear-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Perfume Cost Per Wear Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "perfume-cost-per-wear-calculator": {
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
