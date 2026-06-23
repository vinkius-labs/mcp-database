# Apgar Score Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/apgar-score-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Calculate and compare newborn Apgar scores to assess vitality at 1 and 5 minutes.

## Description
The Apgar Score Calculator is a clinical assessment tool designed to evaluate the health of a newborn immediately after birth. By analyzing five physiological parameters--heart rate, respiratory effort, muscle tone, reflex irritability, and skin color--the tool provides a standardized score at 1-minute and 5-minute intervals. Use `compute_apgar_at_interval` to calculate total scores and clinical recommendations, `compare_apgar_intervals` to track health trends (improving, stable, or declining), and `get_parameter_reference` to understand the specific clinical observations for each score value.


## Available Tools (3)
- **compare_apgar_intervals**: Compare Apgar scores between two different time intervals
- **get_parameter_reference**: Get clinical descriptions for Apgar parameter scores
- **compute_apgar_at_interval**: Calculate the Apgar score for a newborn at a specific interval


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Apgar Score Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the Apgar score for a baby with: heart rate 8, breathing 1, muscle tone 2, reflex 1, and skin color 1."

**🤖 AI Agent:**
> The total Apgar score is 13. Wait, the input values must be scores (0-2). Let me re-calculate based on valid inputs: If heart rate is 2, respiratory effort is 1, muscle tone is 2, reflex irritability is 1, and skin color is 1, the total score is 7. This falls into the Stable category with routine newborn care recommended.

---

**👤 You:**
> "The baby had a score of 4 at 1 minute and 7 at 5 minutes. What is the trend?"

**🤖 AI Agent:**
> The infant's condition is Improving.

---

**👤 You:**
> "What does a score of 0 for heart rate mean?"

**🤖 AI Agent:**
> A score of 0 for heart rate indicates that no pulse was detected.


## ❓ FAQ

**Q: What is the purpose of the Apgar score?**
The Apgar score is a rapid assessment used to evaluate a newborn's physical condition and determine if immediate medical intervention is required.

**Q: How do I use the `compute_apgar_at_interval` tool?**
Provide the scores (0, 1, or 2) for heart rate, respiratory effort, muscle tone, reflex irritability, and skin color. The tool will return the total score, clinical classification, and recommended action.

**Q: Can I compare scores from different time intervals?**
Yes, use the `compare_apgar_intervals` tool by providing the 1-minute and 5-minute total scores to see if the infant's condition is improving, stable, or declining.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/apgar-score-calculator](https://vinkius.com/mcp/apgar-score-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Apgar Score Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `apgar-score-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Apgar Score Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "apgar-score-calculator": {
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
