# Sourdough Starter Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/sourdough-starter-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Deterministic feeding plans and microbial activity predictions for sourdough starters.

## Description
Manage your sourdough culture with precision. This MCP server provides tools to calculate exact feeding weights, determine discard amounts, and predict microbial activity based on ambient temperature. Use `calculate_feeding_plan` to get precise flour and water weights, `predict_starter_activity` to estimate peak rise times and pH trajectories, and `get_hydration_classification` to identify if your starter is stiff or liquid.


## Available Tools (3)
- **calculate_feeding_plan**: 
- **get_hydration_classification**: 
- **predict_starter_activity**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sourdough Starter Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 50g of starter at 100% hydration. I want to feed it at a 1:2:2 ratio. How much flour and water do I need?"

**🤖 AI Agent:**
> To maintain a 1:2:2 ratio with 50g of starter, you need 100g of flour and 100g of water. You should discard 0g if you want to keep the total mass at 250g, or adjust based on your target weight.

---

**👤 You:**
> "My kitchen is 28°C and my starter is 5 days old. When will it peak?"

**🤖 AI Agent:**
> At 28°C, you can expect the starter to reach its peak rise in approximately 4 to 6 hours.

---

**👤 You:**
> "Is my starter considered liquid or stiff if the hydration is 55%?"

**🤖 AI Agent:**
> A hydration of 55% is classified as a stiff starter.


## ❓ FAQ

**Q: How do I know if my starter is mature?**
You can use `predict_starter_activity` to estimate the maturity day. Typically, a starter reaches stability between day 7 and day 14.

**Q: What is an underfeeding risk?**
An underfeeding risk occurs when the feeding ratio is too low for the ambient temperature (e.g., ratio < 1:2:2 in warm conditions), which can lead to acid buildup.

**Q: Can I use this for stiff starters?**
Yes. Use `get_hydration_classification` to confirm if your starter is classified as stiff (50-65% hydration) or liquid (100-125%).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/sourdough-starter-tracker](https://vinkius.com/ai-agent-connect/sourdough-starter-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sourdough Starter Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sourdough-starter-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sourdough Starter Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sourdough-starter-tracker": {
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
