# Cabin Bag Weight Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/cabin-bag-weight-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate total weight and check airline compliance for cabin luggage.

## Description
This MCP server provides tools to manage cabin luggage weight. You can use `calculate_total_weight` to sum up individual item masses, `check_weight_compliance` to verify if the total stays within airline limits, `validate_item_list` to ensure all weights are valid, and `get_weight_category` to classify the bag's heaviness. It helps ensure your carry-on meets airline requirements before you head to the airport.


## Available Tools (4)
- **check_weight_compliance**: Determines if the total weight of the cabin bag stays within a specific limit
- **calculate_total_weight**: Calculates the total weight of all items provided
- **get_weight_category**: Categorizes the total weight into descriptive tiers
- **validate_item_list**: Verifies that a list of items contains only valid weight measurements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cabin Bag Weight Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total weight of my items: 2.5kg, 1.2kg, and 0.8kg?"

**🤖 AI Agent:**
> The total weight of your items is 4.5kg.

---

**👤 You:**
> "Is a 12kg bag compliant with a 10kg limit?"

**🤖 AI Agent:**
> No, the bag is not compliant. It exceeds the limit by 2kg.

---

**👤 You:**
> "What category does a 5kg bag fall into?"

**🤖 AI Agent:**
> A 5kg bag is categorized as Light.


## ❓ FAQ

**Q: How do I calculate the total weight of my bag?**
You can use the `calculate_total_weight` tool by providing an array of the weights for each item in your bag.

**Q: Can I check if my bag exceeds airline limits?**
Yes, the `check_weight_compliance` tool compares your total weight against a specific limit and tells you if you are compliant.

**Q: What happens if I provide invalid weight data?**
The `validate_item_list` tool can be used to verify that all provided weights are positive numbers before you perform calculations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/cabin-bag-weight-calculator](https://vinkius.com/en/ai-agent-connect/cabin-bag-weight-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cabin Bag Weight Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cabin-bag-weight-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cabin Bag Weight Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cabin-bag-weight-calculator": {
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
