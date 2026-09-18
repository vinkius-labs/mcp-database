# Sarcopenia Risk Assessment MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/sarcopenia-risk-assessment)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Estimates muscle loss risk and provides functional health insights.

## Description
This MCP server provides physiological assessment tools to monitor muscle health. Use `get_sarcopenia_risk` to determine vulnerability to muscle loss, `estimate_muscle_health` to evaluate functional capacity, `predict_decline_trajectory` to forecast mobility changes, and `get_training_recommendations` for personalized resistance training guidance.


## Available Tools (4)
- **estimate_muscle_health**: Provides an estimation of current muscle mass status and functional capacity
- **get_sarcopenia_risk**: Determines the current risk level of muscle loss based on primary physiological indicators
- **get_training_recommendations**: Generates personalized resistance training guidance based on risk and current status
- **predict_decline_trajectory**: Forecasts the likely direction of physical mobility and strength over time


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sarcopenia Risk Assessment** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my sarcopenia risk if I am 70 years old, have 25kg grip strength, walk at 1.1 m/s, and am sedentary?"

**🤖 AI Agent:**
> Your sarcopenia risk category is high.

---

**👤 You:**
> "Estimate my muscle health with 30kg grip strength and 1.3 m/s walking speed."

**🤖 AI Agent:**
> Your muscle health proxy is 0.85 and your functional capacity is optimal.

---

**👤 You:**
> "What training should I do if I have a moderate risk and am currently active?"

**🤖 AI Agent:**
> We recommend maintaining your current routine with added progressive resistance training twice a week.


## ❓ FAQ

**Q: What is sarcopenia?**
Sarcopenia is the progressive loss of skeletal muscle mass and strength, often associated with aging.

**Q: How accurate are the risk scores?**
The scores are estimates based on physiological markers like grip strength and walking speed to assist in screening.

**Q: Can I get training advice?**
Yes, you can use `get_training_recommendations` to receive personalized resistance training guidance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/sarcopenia-risk-assessment](https://vinkius.com/en/ai-agent-connect/sarcopenia-risk-assessment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sarcopenia Risk Assessment** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sarcopenia-risk-assessment` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sarcopenia Risk Assessment** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sarcopenia-risk-assessment": {
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
