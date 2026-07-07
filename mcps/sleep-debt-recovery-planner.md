# Sleep Debt Recovery Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sleep-debt-recovery-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Incrementally resolve sleep deficits without disrupting your circadian rhythm.

## Description
The Sleep Debt Recovery Planner helps you manage accumulated sleep loss through small, safe adjustments to your sleep window. By using tools like `generate_recovery_schedule`, you can create a night-by-night itinerary that gradually increases your sleep duration without causing 'social jetlag'. You can also use `estimate_days_until_debt_free` to see how long your recovery will take, or `validate_recovery_parameters` to ensure your proposed recovery rate is within safe physiological limits for circadian stability.


## Available Tools (3)
- **estimate_days_until_debt_free**: Estimate the number of nights needed to clear sleep debt
- **generate_recovery_schedule**: Generate a night-by-night sleep recovery schedule
- **validate_recovery_parameters**: Validate if a recovery rate is safe


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sleep Debt Recovery Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 5 hours of sleep debt. I want to recover at 0.5 hours per night. My current bedtime is 23:00 and waketime is 07:00. Create a schedule for me."

**🤖 AI Agent:**
> Your recovery plan will take 10 nights. Night 1: Bedtime 22:30, Waketime 07:30, Remaining Debt: 4.5 hours. Night 2: Bedtime 22:00, Waketime 08:00, Remaining Debt: 4.0 hours...

---

**👤 You:**
> "How many nights will it take to clear 12 hours of sleep debt if I add 1 hour per night?"

**🤖 AI Agent:**
> It will take approximately 12 nights to fully recover from your 12-hour sleep debt.

---

**👤 You:**
> "Is it safe to increase my sleep by 2 hours per night?"

**🤖 AI Agent:**
> No, a 2-hour increase is considered aggressive and may disrupt your circadian rhythm. A smaller increment is recommended.


## ❓ FAQ

**Q: How does the recovery schedule work?**
The `generate_recovery_schedule` tool calculates a plan where each night your sleep duration increases by your chosen recovery cap, gradually reducing your debt.

**Q: Can I use any recovery rate?**
It is best to use small increments. You can check if your proposed rate is safe using the `validate_recovery_parameters` tool.

**Q: How do I know when my debt is gone?**
The `estimate_days_until_debt_free` tool provides a quick estimate of the total nights required to reach zero debt.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sleep-debt-recovery-planner](https://vinkius.com/mcp/sleep-debt-recovery-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sleep Debt Recovery Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sleep-debt-recovery-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sleep Debt Recovery Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sleep-debt-recovery-planner": {
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
