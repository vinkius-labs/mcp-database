# Menstrual Cycle Insulin Resistance Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/menstrual-cycle-insulin-resistance-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Adjust insulin parameters based on menstrual cycle phases.

## Description
This MCP server provides deterministic insulin resistance adjustments based on the physiological shifts of the menstrual cycle. It allows AI agents to calculate precise insulin-to-carbohydrate ratios (ICR) and insulin sensitivity factors (ISF) for the Follicular, Ovulation, and Luteal phases. By using `get_cycle_adjustments`, agents can determine the exact resistance multiplier and expected blood glucose trends to assist in glucose management.


## Available Tools (3)
- **get_cycle_adjustments**: Calculates insulin parameter adjustments based on the current cycle day
- **get_phase_summary**: Provides a summary of the current menstrual cycle phase and its insulin resistance impact
- **get_resistance_thresholds**: Retrieves the standard resistance multipliers used for calculations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Menstrual Cycle Insulin Resistance Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am on day 20 of my cycle. My baseline ICR is 1:10 and my baseline ISF is 1:50. What are my adjusted values?"

**🤖 AI Agent:**
> On day 20 (Luteal phase), your resistance multiplier is 1.2. Your adjusted ICR is 1:8.33 and your adjusted ISF is 1:41.67. You should expect a rising blood glucose trend.

---

**👤 You:**
> "What is the insulin resistance impact for day 5?"

**🤖 AI Agent:**
> On day 5, you are in the Follicular phase with Low resistance.

---

**👤 You:**
> "What are the standard resistance multipliers used?"

**🤖 AI Agent:**
> The standard multipliers are 1.0 for Follicular, 1.1 for Ovulation, and a range of 1.2 to 1.3 for the Luteal phase.


## ❓ FAQ

**Q: How does this tool help with insulin management?**
It uses `get_cycle_adjustments` to calculate how much insulin resistance increases during different phases, providing adjusted ICR and ISF values.

**Q: What phases are covered?**
The tool covers the Follicular, Ovulation, and Luteal phases of the menstrual cycle.

**Q: Can I see the resistance levels for each phase?**
Yes, you can use `get_phase_summary` to see the qualitative resistance level (Low, Moderate, or High) for the current cycle day.


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
