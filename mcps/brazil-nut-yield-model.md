# Brazil Nut Yield Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/brazil-nut-yield-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [environmental-science](../categories/environmental-science.md)

Estimates Brazil nut yield per hectare using allometric equations and environmental data.

## Description
This MCP server provides specialized tools for modeling Brazil nut production in natural forest systems. It uses allometric scaling to calculate how tree size (DBH) and environmental factors like rainfall and pollinator abundance affect fruit set and kernel yield. Use `calculate_tree_productivity` to find individual tree output, `estimate_hectare_yield` for area-wide production, and `analyze_pollination_impact` to assess how bee populations influence yield.


## Available Tools (3)
- **analyze_pollination_impact**: Analyzes how sensitive the yield is to changes in pollinator populations
- **calculate_tree_productivity**: Calculates expected fruit production for a single tree based on DBH, exposure, and environmental factors
- **estimate_hectare_yield**: Estimates the total expected kernel yield per hectare


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Brazil Nut Yield Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the expected kernel yield for a tree with a DBH of 50cm, high crown exposure, flowering intensity of 0.8, pollinator abundance of 0.5, and 1500mm rainfall?"

**🤖 AI Agent:**
> The expected kernel weight for this tree is 12.4 kg.

---

**👤 You:**
> "Calculate the total yield per hectare if there are 40 trees per hectare and each tree produces 15kg of kernels."

**🤖 AI Agent:**
> The total expected yield is 600 kg per hectare.

---

**👤 You:**
> "How much will a decrease in bees affect my yield if flowering intensity is 0.9 and current pollinator abundance is 0.4?"

**🤖 AI Agent:**
> The sensitivity index is 0.75, indicating that a small decrease in bee populations will significantly reduce the fruit set rate.


## ❓ FAQ

**Q: How does pollinator abundance affect the results?**
The `analyze_pollination_impact` tool calculates how sensitive the yield is to bee populations. Low pollinator abundance can significantly reduce the fruit set efficiency regardless of flowering intensity.

**Q: What inputs are needed for tree productivity?**
To use `calculate_tree_productivity`, you need the DBH distribution, crown exposure class, flowering intensity, pollinator abundance, and rainfall amount.

**Q: Can I estimate total yield for a large area?**
Yes, by using `estimate_hectare_yield` with the tree density and the productivity data obtained from `calculate_tree_productivity`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/brazil-nut-yield-model](https://vinkius.com/ai-agent-connect/brazil-nut-yield-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Brazil Nut Yield Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `brazil-nut-yield-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Brazil Nut Yield Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "brazil-nut-yield-model": {
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
