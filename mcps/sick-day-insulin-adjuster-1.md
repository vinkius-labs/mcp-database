# Sick Day Insulin Adjuster MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/sick-day-insulin-adjuster-1)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Deterministic insulin adjustment and care planning for illness.

## Description
This MCP server provides precise, deterministic calculations to manage insulin resistance and care requirements during illness. It helps users adjust insulin doses based on fever and physiological stress, determines necessary hydration levels, and assesses ketone-related risks to prevent Diabetic Ketoacidosis (DKA). Use `calculate_insulin_adjustments` to determine dose increases, `get_care_schedule` for monitoring and hydration targets, and `evaluate_ketone_risk` to assess immediate medical needs.


## Available Tools (3)
- **calculate_insulin_adjustments**: 
- **evaluate_ketone_risk**: 
- **get_care_schedule**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sick Day Insulin Adjuster** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a fever of 38.5°C and my baseline insulin is 40 units. How much should I adjust my insulin?"

**🤖 AI Agent:**
> With a temperature of 38.5°C, your fever-related insulin increase is 10%. Combined with the stress factor, your total adjusted insulin requirement will be calculated by the tool.

---

**👤 You:**
> "My baseline insulin is 30 units. What are my hydration and monitoring needs while sick?"

**🤖 AI Agent:**
> You should aim for 45ml of hydration (1.5x baseline) and monitor your glucose every 2-4 hours.

---

**👤 You:**
> "I detected moderate ketones. What is my risk level?"

**🤖 AI Agent:**
> Moderate ketones indicate a significant risk. You should increase your correction bolus by 10-20% and contact a healthcare professional immediately.


## ❓ FAQ

**Q: How does fever affect my insulin needs?**
Fever increases insulin resistance. The `calculate_insulin_adjustments` tool adds 10% to your baseline insulin for every degree Celsius your temperature is above 37.5°C.

**Q: What should I do if I have moderate or large ketones?**
If ketones are moderate or large, you should increase your correction bolus by 10-20% and seek medical advice immediately as indicated by `evaluate_ketone_risk`.

**Q: How often should I monitor my blood glucose during illness?**
During illness, you should monitor more frequently. The `get_care_schedule` tool recommends checking every 2 to 4 hours.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/sick-day-insulin-adjuster-1](https://vinkius.com/ai-agent-connect/sick-day-insulin-adjuster-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sick Day Insulin Adjuster** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sick-day-insulin-adjuster-1` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sick Day Insulin Adjuster** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sick-day-insulin-adjuster-1": {
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
