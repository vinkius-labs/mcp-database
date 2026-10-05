# Unit Price Shopping Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/unit-price-shopping-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Optimize purchasing decisions by analyzing usable quantity, true cost, and storage efficiency.

## Description
This MCP server provides a decision-support engine to help users look beyond sticker prices. By analyzing the 'true cost' of products, it helps identify the best value through several specialized tools. Use `compare_packages` to find the best value among multiple options, `calculate_lifecycle_cost` to project long-term spending, `evaluate_storage_utility` to assess if bulk items fit your space, and `optimize_purchase_frequency` to balance budget and consumption needs.


## Available Tools (4)
- **calculate_lifecycle_cost**: Calculate the total cost of a product over a specific period
- **compare_packages**: Compare packages by usable quantity, price, discounts, waste, storage, and purchase frequency
- **evaluate_storage_utility**: Evaluate if a bulk purchase is worth the storage space
- **optimize_purchase_frequency**: Optimize the balance between bulk buying and frequent purchases


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Unit Price Shopping Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which of these three milk packages is the best deal: 1L for $2.00, 2L for $3.50, or 4L for $6.00? Use 1000ml as the target unit."

**🤖 AI Agent:**
> The 2L package is the best deal with a unit price of $1.75 per liter.

---

**👤 You:**
> "How much will I spend on coffee over 6 months if I use 500g per month and the package is 1kg for $15?"

**🤖 AI Agent:**
> You will spend $45.00 over 6 months, requiring 3 purchases of the 1kg package.

---

**👤 You:**
> "I have 10 liters of space. Is it better to buy a 5L detergent for $10 or a 12L detergent for $22?"

**🤖 AI Agent:**
> The 5L detergent is the only viable option as the 12L package exceeds your available storage volume.


## ❓ FAQ

**Q: How does this tool calculate value?**
It calculates value by comparing the usable weight against the price, while also accounting for waste and storage requirements using `compare_packages`.

**Q: Can I plan my monthly grocery budget?**
Yes, you can use `calculate_lifecycle_cost` to estimate your total spend over a specific period based on your consumption rate.

**Q: How do I know if a bulk package fits in my pantry?**
The `evaluate_storage_utility` tool analyzes the storage volume of different packages against your available space to recommend the most efficient option.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/unit-price-shopping-plan](https://vinkius.com/en/ai-agent-connect/unit-price-shopping-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Unit Price Shopping Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `unit-price-shopping-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Unit Price Shopping Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "unit-price-shopping-plan": {
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
