# Personalized Sleep Report Generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/personalized-sleep-report-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Transform raw sleep data and health profiles into actionable sleep optimization reports.

## Description
This MCP server acts as a specialized engine that synthesizes physiological sleep metrics, subjective wellbeing data, and health history. By using tools like `get_sleep_metrics` and `analyze_subjective_wellbeing`, AI agents can identify why sleep quality fluctuates and generate tailored advice. The engine correlates sleep architecture with user habits to provide deep insights via `generate_insights` and creates prioritized, goal-oriented recovery paths through `provide_action_plan`.


## Available Tools (4)
- **generate_insights**: Generate insights by correlating metrics, health history, and habits
- **analyze_subjective_wellbeing**: Analyze user perceived energy and sleepiness alignment with physiological data
- **get_sleep_metrics**: Calculate physiological sleep statistics for a user over a period
- **provide_action_plan**: Provide specific actionable steps to reach sleep goals


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Personalized Sleep Report Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How did I sleep last night?"

**🤖 AI Agent:**
> Last night you achieved 7 hours of sleep with a sleep efficiency of 88%. Your deep sleep was slightly lower than your average, but your REM cycles were optimal.

---

**👤 You:**
> "Why was my sleep quality low yesterday?"

**🤖 AI Agent:**
> Your sleep quality was impacted by high sleep latency. This correlates with your reported caffeine intake late in the evening.

---

**👤 You:**
> "Give me a plan to reduce my sleep latency."

**🤖 AI Agent:**
> To reduce latency, you should establish a consistent wind-down routine, avoid blue light 60 minutes before bed, and maintain a cool bedroom temperature.


## ❓ FAQ

**Q: How does the engine calculate sleep quality?**
The quality score is a normalized value derived from a combination of sleep efficiency, latency, and the specific distribution of sleep stages like REM and Deep sleep.

**Q: Can I use this to improve my deep sleep?**
Yes, you can use `provide_action_plan` with the goal type 'increase_deep_sleep' to receive specific, prioritized steps to improve your recovery.

**Q: Does it consider my health history?**
Yes, when using `generate_insights`, you can enable health context to factor in medication schedules or specific health constraints.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/personalized-sleep-report-generator](https://vinkius.com/en/ai-agent-connect/personalized-sleep-report-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Personalized Sleep Report Generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `personalized-sleep-report-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Personalized Sleep Report Generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "personalized-sleep-report-generator": {
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
