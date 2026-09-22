# Jewelry Metal Weight Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/jewelry-metal-weight-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [calculation](../categories/calculation.md)

Calculate and validate precise metal weights for jewelry collections.

## Description
This MCP server provides specialized tools for managing precious metal mass in jewelry production and inventory. It allows AI agents to perform precise calculations using `sum_metal_weights` to aggregate specific metals, `get_weight_summary` to provide a full breakdown of all metals in a collection, and `check_weight_threshold` to monitor weight limits. Additionally, `validate_weight_entry` ensures all weight data meets strict domain standards for accuracy.


## Available Tools (4)
- **check_weight_threshold**: Does the total weight of a specific metal exceed a certain limit?
- **get_weight_summary**: Give me a breakdown of all metal totals from this list
- **sum_metal_weights**: What is the total weight of a specific metal across these provided items?
- **validate_weight_entry**: Is this specific weight entry valid and formatted correctly?


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Jewelry Metal Weight Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total weight of Gold in this list: [{'weight': 5, 'metalType': 'Gold'}, {'weight': 10, 'metalType': 'Gold'}, {'weight': 2, 'metalType': 'Silver'}]?"

**🤖 AI Agent:**
> The total weight of Gold is 15.

---

**👤 You:**
> "Give me a breakdown of all metal totals from this list: [{'weight': 10, 'metalType': 'Gold'}, {'weight': 5, 'metalType': 'Silver'}]"

**🤖 AI Agent:**
> Gold: 10, Silver: 5

---

**👤 You:**
> "Is the total weight of Silver over 20 in this list: [{'weight': 15, 'metalType': 'Silver'}, {'weight': 10, 'metalType': 'Silver'}]?"

**🤖 AI Agent:**
> Yes, the total weight of Silver is 25, which exceeds the limit of 20.


## ❓ FAQ

**Q: How can I find the total weight of gold in my list?**
You can use the `sum_metal_weights` tool by providing the metal type 'Gold' and the list of items.

**Q: Can I check if a metal weight exceeds a specific limit?**
Yes, the `check_weight_threshold` tool is designed to verify if the total weight of a specific metal is strictly greater than your defined limit.

**Q: How do I get a full report of all metals in a collection?**
Use the `get_weight_summary` tool to receive a complete breakdown of all aggregated metal totals found in your list.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/jewelry-metal-weight-calculator](https://vinkius.com/en/ai-agent-connect/jewelry-metal-weight-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Jewelry Metal Weight Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `jewelry-metal-weight-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Jewelry Metal Weight Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jewelry-metal-weight-calculator": {
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
