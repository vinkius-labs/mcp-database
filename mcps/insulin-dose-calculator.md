# Insulin Dose Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/insulin-dose-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

A deterministic tool for calculating mealtime insulin doses and estimating insulin on board.

## Description
This MCP server provides precise tools for diabetes management. Use `calculate_insulin_dose` to determine the total insulin required by combining carbohydrate needs and glucose correction. Use `estimate_iob_decay` to track remaining active insulin, and `validate_glucose_safety` to ensure blood glucose levels are within safe limits before bolusing.


## Available Tools (3)
- **calculate_insulin_dose**: Calculates the specific insulin dose required for a meal and blood glucose correction
- **estimate_iob_decay**: Estimates the remaining active insulin based on time elapsed since the last dose
- **validate_glucose_safety**: Checks if the current glucose level is within safe limits for bolusing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Insulin Dose Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my insulin dose. My glucose is 150 mg/dL, target is 100 mg/dL, I'm eating 60g of carbs, my ICR is 10, my ISF is 50, and I have 2 units of active insulin."

**🤖 AI Agent:**
> Your meal bolus is 6.0 units, your correction bolus is 1.0 unit, and after subtracting your 2 units of active insulin, your total recommended dose is 5.0 units.

---

**👤 You:**
> "Is it safe to bolus? My current glucose is 65 mg/dL."

**🤖 AI Agent:**
> No, it is not safe to bolus. Your blood glucose is below the safety threshold of 70 mg/dL.

---

**👤 You:**
> "I took 5 units of insulin 2 hours ago. How much is left?"

**🤖 AI Agent:**
> Approximately 2.5 units of insulin are still active in your body.


## ❓ FAQ

**Q: How does the tool calculate the total dose?**
The tool calculates the meal bolus based on carbohydrates and the correction bolus based on the difference between current and target glucose, then subtracts the active insulin (IOB) to prevent stacking.

**Q: What happens if my blood glucose is too low?**
If the current blood glucose is below 70 mg/dL, the tool will trigger a hypoglycemia warning and recommend a dose of 0 to ensure safety.

**Q: Can I use this to track my insulin on board?**
Yes, you can use `estimate_iob_decay` to estimate how much insulin remains active in your body based on the time elapsed since your last dose.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/insulin-dose-calculator](https://vinkius.com/ai-agent-connect/insulin-dose-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Insulin Dose Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `insulin-dose-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Insulin Dose Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "insulin-dose-calculator": {
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
