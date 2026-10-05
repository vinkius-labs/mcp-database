# Skincare Routine Budget Manager MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/skincare-routine-budget-manager)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track product longevity, replenishment dates, and monthly skincare spending limits.

## Description
This MCP server connects your AI assistant to your skincare inventory and budget. It provides tools to calculate exactly how long a product will last using `get_product_longevity`, predict when you need to buy more with `calculate_replenishment_schedule`, and monitor your monthly spending via `get_monthly_budget_status`. You can also organize your routine using `list_products_by_category`.


## Available Tools (4)
- **calculate_replenishment_schedule**: Determines the date when a product will need to be repurchased
- **get_monthly_budget_status**: Checks if the current skincare routine fits within the user's defined monthly spending limit
- **get_product_longevity**: Calculates how many days a specific product will last
- **list_products_by_category**: Filters products based on their type


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Skincare Routine Budget Manager** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many days will my 50ml cleanser last if I use 2ml twice a day?"

**🤖 AI Agent:**
> Your 50ml cleanser will last for 12.5 days.

---

**👤 You:**
> "When will I need to repurchase my moisturizer?"

**🤖 AI Agent:**
> You are expected to repurchase your moisturizer on October 15th, 2024.

---

**👤 You:**
> "Am I going to go over my $50 monthly skincare budget?"

**🤖 AI Agent:**
> No, your projected spend for this month is $35, leaving you with a $15 buffer.


## ❓ FAQ

**Q: How does the tool calculate product longevity?**
It uses the `get_product_longevity` tool to divide the total package size by the amount used per application, adjusted for how many times you use it daily.

**Q: Can I set a monthly spending limit?**
Yes, you can use `get_monthly_budget_status` to check if your scheduled product replacements stay within your defined monthly cap.

**Q: How do I know when to buy a new cleanser?**
The `calculate_replenishment_schedule` tool provides the specific date you should expect to run out of a product.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/skincare-routine-budget-manager](https://vinkius.com/en/ai-agent-connect/skincare-routine-budget-manager)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Skincare Routine Budget Manager** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `skincare-routine-budget-manager` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Skincare Routine Budget Manager** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "skincare-routine-budget-manager": {
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
