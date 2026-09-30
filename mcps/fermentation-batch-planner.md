# Fermentation Batch Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/fermentation-batch-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Precision scaling and planning for fermentation batches.

## Description
A precision planning engine for fermentation producers. This MCP server provides tools to scale ingredient formulas to a specific target yield, calculate brine requirements (salt and water), verify if a batch fits within a specific vessel capacity using `validate_vessel_fit`, and aggregate total ingredient costs. It bridges the gap between small-scale recipes and large-scale production planning.


## Available Tools (4)
- **calculate_batch_cost**: Aggregates the total financial cost of the ingredients for the planned batch
- **calculate_batch_scaling**: Determines the exact weight of every ingredient required to reach the target yield
- **plan_brine_requirements**: Calculates the amount of salt and water needed to create the brine component
- **validate_vessel_fit**: Checks if the planned batch will fit into the intended fermentation vessel


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fermentation Batch Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to make a 10kg batch of sauerkraut. My formula is 100 parts cabbage and 2 parts salt. How much of each do I need?"

**🤖 AI Agent:**
> To reach a 10kg target yield, you will need 9.80kg of cabbage and 0.20kg of salt.

---

**👤 You:**
> "I have 5kg of cabbage and I need a 2% salt concentration. I want 1 liter of brine. How much salt and water do I need?"

**🤖 AI Agent:**
> You need 0.1kg of salt and 0.9 liters of water to create your brine.

---

**👤 You:**
> "Will 8kg of produce and 2 liters of brine fit in a 10 liter vessel if I want a 10% safety buffer?"

**🤖 AI Agent:**
> No, the batch will not fit. With a 10% safety buffer, your effective capacity is 9 liters, but your batch requires 10 liters.


## ❓ FAQ

**Q: How do I scale my recipe for a larger batch?**
Use the `calculate_batch_scaling` tool by providing your target yield and the ingredient formula as a JSON object.

**Q: Can I check if my fermentation crock is big enough?**
Yes, use the `validate_vessel_fit` tool to compare your total produce weight and brine volume against your vessel's capacity.

**Q: How is the brine calculated?**
The `plan_brine_requirements` tool calculates the exact salt weight based on your primary produce weight and the required salt percentage, then determines the necessary water volume.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/fermentation-batch-planner](https://vinkius.com/en/ai-agent-connect/fermentation-batch-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fermentation Batch Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fermentation-batch-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fermentation Batch Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fermentation-batch-planner": {
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
