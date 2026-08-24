# Menstrual Cycle Insulin Resistance Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/menstrual-cycle-insulin-resistance-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Adjust insulin parameters based on menstrual cycle phases.

## Description
This MCP server provides deterministic insulin resistance adjustments based on the physiological shifts in the menstrual cycle. It calculates adjusted Insulin-to-Carbohydrate Ratio (ICR) and Insulin Sensitivity Factor (ISF) for the Follicular, Ovulation, and Luteal phases. Use `calculate_insulin_adjustments` to get precise values for your current cycle day, or `get_cycle_phase_info` to understand your current resistance level.


## Available Tools (3)
- **calculate_insulin_adjustments**: 
- **get_cycle_phase_info**: 
- **validate_baseline_parameters**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Menstrual Cycle Insulin Resistance Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are my insulin adjustments for day 20 of my cycle with a baseline ICR of 10 and ISF of 50?"

**🤖 AI Agent:**
> For day 20 (Luteal phase), your resistance multiplier is 1.25. Your adjusted ICR is 8 and your adjusted ISF is 40.

---

**👤 You:**
> "What phase am I in on day 14?"

**🤖 AI Agent:**
> You are currently in the Ovulation phase, which typically involves a slight increase in insulin resistance.

---

**👤 You:**
> "Check if an ICR of 5 and ISF of 40 are valid."

**🤖 AI Agent:**
> Yes, those baseline parameters are valid.


## ❓ FAQ

**Q: How does this tool help with insulin management?**
The tool uses `calculate_insulin_adjustments` to provide updated ICR and ISF values that account for the increased insulin resistance often seen during the Luteal phase.

**Q: Can I check my current cycle phase?**
Yes, you can use the `get_cycle_phase_info` tool to identify if you are in the Follicular, Ovulation, or Luteal phase.

**Q: Is it safe to use these adjustments?**
You can use `validate_baseline_parameters` to ensure your input values are within safe, positive ranges before performing calculations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/menstrual-cycle-insulin-resistance-tracker](https://vinkius.com/ai-agent-connect/menstrual-cycle-insulin-resistance-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Menstrual Cycle Insulin Resistance Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `menstrual-cycle-insulin-resistance-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Menstrual Cycle Insulin Resistance Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "menstrual-cycle-insulin-resistance-tracker": {
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
