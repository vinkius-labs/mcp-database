# Burnout Risk Assessment MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/burnout-risk-assessment)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Assess burnout risk for Singapore professionals using work, commute, sleep, and vacation data.

## Description
This MCP server provides deterministic tools to evaluate burnout risk for young professionals in Singapore. By analyzing work hours, commute times, sleep patterns, and vacation usage, it calculates a comprehensive burnout profile. Use `get_burnout_profile` for a full diagnostic report, `get_commitment_metrics` to isolate workload components, or `get_recovery_deficit` to identify physiological and statutory recovery gaps.


## Available Tools (3)
- **get_burnout_profile**: Provides a full diagnostic profile of a professional's burnout risk based on their current work and lifestyle habits
- **get_commitment_metrics**: Isolates the professional workload components to understand the pure time commitment without health recovery factors
- **get_recovery_deficit**: Calculates the biological and statutory recovery gaps (sleep and vacation) to identify physiological strain


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Burnout Risk Assessment** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my burnout risk. I work 9 hours a day, commute 45 minutes each way, work 5 hours of overtime per week, have taken 4 vacation days this year, and sleep 7 hours a night."

**🤖 AI Agent:**
> Your weekly work hours are 50, and your total commitment is 65 hours. Your burnout index is Critical, your vacation deficit is 10 days, and your recovery score is 48.

---

**👤 You:**
> "What are my commitment metrics? I work 8 hours a day, commute 30 minutes each way, and do 2 hours of overtime weekly."

**🤖 AI Agent:**
> Your weekly work hours are 42, your weekly commute hours are 5, and your total commitment is 47 hours.

---

**👤 You:**
> "Check my recovery deficit. I've taken 10 vacation days this year and sleep 7 hours per night."

**🤖 AI Agent:**
> Your vacation deficit is 4 days and your weekly sleep debt is 7 hours.


## ❓ FAQ

**Q: What is included in the burnout profile?**
The `get_burnout_profile` tool provides weekly work hours, total commitment hours, a qualitative burnout index (Low to Critical), vacation deficit, and a holistic recovery score.

**Q: How is the vacation deficit calculated?**
It is calculated by subtracting the number of vacation days taken from the Singapore standard of 14 days.

**Q: Can I see just my workload without health factors?**
Yes, you can use the `get_commitment_metrics` tool to isolate work and commute hours from recovery data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/burnout-risk-assessment](https://vinkius.com/ai-agent-connect/burnout-risk-assessment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Burnout Risk Assessment** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `burnout-risk-assessment` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Burnout Risk Assessment** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "burnout-risk-assessment": {
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
