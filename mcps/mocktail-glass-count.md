# Mocktail Glass Count MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/mocktail-glass-count)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [hospitality](../categories/hospitality.md)

Calculate exact serving yields and batch requirements for event planning.

## Description
This MCP server provides precision tools for event planners and bartenders to manage liquid inventory. Use `calculate_serving_yield` to determine how many full glasses can be poured from a batch, or `compare_glass_options` to find the most efficient glass size for your volume. It also includes `batch_scaling_requirement` to calculate necessary volumes for guest counts and `validate_recipe_capacity` to ensure your current batch covers your expected guests.


## Available Tools (4)
- **compare_glass_options**: Compare different glass sizes to maximize servings
- **batch_scaling_requirement**: Calculate required batch volume for a target number of servings
- **calculate_serving_yield**: Calculate the number of full servings available from a batch
- **validate_recipe_capacity**: Check if a batch is sufficient for the expected number of guests


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mocktail Glass Count** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many full glasses can I serve from a 5 liter batch using 200ml glasses with 5% waste?"

**🤖 AI Agent:**
> You can serve 23 full glasses from this batch.

---

**👤 You:**
> "I need to serve 50 guests with 150ml glasses. How much liquid do I need to prepare if I account for 10% waste?"

**🤖 AI Agent:**
> You need to prepare 8333.33 milliliters of liquid to meet your target.

---

**👤 You:**
> "Is my 2 liter batch enough for 15 guests using 125ml glasses and 5% waste?"

**🤖 AI Agent:**
> Yes, your batch is sufficient. You will have a surplus of 125 milliliters.


## ❓ FAQ

**Q: How does the tool handle liquid waste?**
You can specify a `wastagePercentage` to account for liquid lost during pouring or residue left in vessels. The tool subtracts this volume before calculating the final serving count.

**Q: Can I compare different glass sizes?**
Yes, use the `compare_glass_options` tool to evaluate multiple glass capacities and identify which one maximizes your total servings.

**Q: Is the serving count rounded?**
Yes, serving counts are always rounded down to the nearest whole number to ensure every guest receives a complete serving.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/mocktail-glass-count](https://vinkius.com/en/ai-agent-connect/mocktail-glass-count)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mocktail Glass Count** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mocktail-glass-count` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mocktail Glass Count** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mocktail-glass-count": {
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
