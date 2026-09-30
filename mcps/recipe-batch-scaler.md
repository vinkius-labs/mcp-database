# Recipe Batch Scaler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/recipe-batch-scaler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Scales ingredient quantities for target servings, waste allowance, and container size.

## Description
This MCP server provides precise tools for culinary scaling and batch management. Use `get_scaled_ingredients` to calculate exact ingredient amounts for any number of servings while accounting for preparation waste. You can use `validate_batch_capacity` to ensure your scaled batch fits in your equipment, `calculate_portion_yield` to determine total portions and leftovers, and `get_scaling_efficiency` to analyze the impact of waste margins on your total ingredient requirements.


## Available Tools (4)
- **calculate_portion_yield**: Determines how many full portions can be extracted from a batch based on a specific portion size
- **get_scaled_ingredients**: Calculates the exact amount of each ingredient needed for a specific number of servings
- **get_scaling_efficiency**: Evaluates the impact of the waste allowance on the total ingredient requirement
- **validate_batch_capacity**: Checks if a scaled recipe batch will fit within the physical limits of a specific container


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Recipe Batch Scaler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a recipe for 4 servings that uses 200g of flour. How much flour do I need for 10 servings with a 5% waste allowance?"

**🤖 AI Agent:**
> You will need 525g of flour.

---

**👤 You:**
> "Will a 5000ml batch fit in a 4.5L container?"

**🤖 AI Agent:**
> No, the batch will not fit. It exceeds the container capacity by 500ml.

---

**👤 You:**
> "If I have 1200g of sauce and each portion is 150g, how many portions can I serve?"

**🤖 AI Agent:**
> You can serve 8 portions.


## ❓ FAQ

**Q: How does the waste allowance work?**
The waste allowance adds a percentage to the scaled ingredients to compensate for loss during preparation, such as peeling or residue left in bowls.

**Q: Can I check if my batch will fit in my pot?**
Yes, you can use the `validate_batch_capacity` tool to compare the total volume of your scaled recipe against the volume of your container.

**Q: How many servings will I get from a batch?**
You can use `calculate_portion_yield` to find out exactly how many full portions can be extracted from your total batch quantity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/recipe-batch-scaler](https://vinkius.com/en/ai-agent-connect/recipe-batch-scaler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Recipe Batch Scaler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `recipe-batch-scaler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Recipe Batch Scaler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "recipe-batch-scaler": {
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
