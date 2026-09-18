# WHOOP Recovery Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/whoop-recovery-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Optimize training and lifestyle based on WHOOP physiological metrics.

## Description
This MCP server connects AI agents to WHOOP physiological data to optimize daily training and recovery. By analyzing metrics like recovery score, HRV, and resting heart rate, the server provides specific training paths and lifestyle interventions. Use `analyze_daily_readiness` to determine your training type, `get_training_prescription` for detailed workout suggestions, `evaluate_rest_necessity` to check if a rest day is mandatory, and `suggest_recovery_interventions` for actionable advice to improve your recovery score.


## Available Tools (4)
- **suggest_recovery_interventions**: Provides actionable lifestyle advice to improve the recovery score
- **analyze_daily_readiness**: Determines the specific training path and physiological state for the current day
- **evaluate_rest_necessity**: Validates if the user's current physiological state requires a complete cessation of training
- **get_training_prescription**: Provides a detailed workout suggestion based on the user's ability to handle strain


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WHOOP Recovery Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Based on my recovery score of 85, HRV of 60, RHR of 52, and sleep performance of 90, what should my training look like today?"

**🤖 AI Agent:**
> Your recovery is optimal. You should aim for High Intensity training with a target strain of 14. A strength session for 45 minutes is recommended.

---

**👤 You:**
> "My recovery score is 30 and my HRV has dropped significantly. Do I need to rest?"

**🤖 AI Agent:**
> Yes, a rest day is mandatory due to your critically low recovery score and significant HRV deviation.

---

**👤 You:**
> "I have a recovery score of 55 and sleep performance of 40. How can I improve my recovery?"

**🤖 AI Agent:**
> To improve your recovery, focus on sleep hygiene: try an earlier bedtime and ensure a dark, cool environment to boost your sleep performance.


## ❓ FAQ

**Q: How does this tool help my training?**
It uses your WHOOP metrics to suggest whether you should perform high-intensity training, moderate exercise, or take a rest day using `analyze_daily_readiness`.

**Q: Can I get specific workout details?**
Yes, by using `get_training_prescription`, you can receive a detailed activity category, intensity level, and duration tailored to your current recovery capacity.

**Q: What if my recovery score is very low?**
If your recovery is low, you can use `evaluate_rest_necessity` to see if a rest day is mandatory and `suggest_recovery_interventions` to get tips on improving your score.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/whoop-recovery-optimizer](https://vinkius.com/en/ai-agent-connect/whoop-recovery-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **WHOOP Recovery Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `whoop-recovery-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **WHOOP Recovery Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "whoop-recovery-optimizer": {
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
