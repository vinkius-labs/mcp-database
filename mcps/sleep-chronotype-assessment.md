# Sleep Chronotype Assessment MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/sleep-chronotype-assessment)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Determine your biological sleep timing and peak performance windows.

## Description
This MCP server provides a scientific approach to understanding your circadian rhythm. By using the `get_chronotype_from_meq` tool, you can determine your biological sleep category based on psychometric scores and age. Once your chronotype is identified, you can use `get_sleep_window` to find your ideal rest period, `get_performance_peaks` to locate your highest alertness times, and `get_schedule_recommendations` to receive actionable lifestyle advice to minimize circadian misalignment.


## Available Tools (4)
- **get_chronotype_from_meq**: Determines a user's chronotype category based on raw psychometric questionnaire scores
- **get_performance_peaks**: Maps the times of day when an individual will experience peak cognitive and physical alertness
- **get_schedule_recommendations**: Provides actionable lifestyle and scheduling advice to minimize circadian misalignment
- **get_sleep_window**: Identifies the optimal biological time range for sleep


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sleep Chronotype Assessment** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "My MEQ score is 55 and I am 30 years old. What is my chronotype?"

**🤖 AI Agent:**
> Your chronotype is Intermediate. This means you have a balanced circadian rhythm that allows for flexibility in both morning and evening activities.

---

**👤 You:**
> "I am an Evening Type. When is my best time to sleep?"

**🤖 AI Agent:**
> For an Evening Type, your ideal sleep window is typically between 00:00 and 08:00.

---

**👤 You:**
> "I am a Morning Type with early morning meetings. How can I manage this?"

**🤖 AI Agent:**
> To mitigate misalignment, seek bright light exposure immediately upon waking and maintain a consistent evening wind-down routine to support your natural rhythm.


## ❓ FAQ

**Q: What is a chronotype?**
A chronotype is your body's natural inclination regarding the timing of sleep and wakefulness, driven by your internal circadian rhythm.

**Q: How accurate is the assessment?**
The assessment uses the standardized Morningness-Eveningness Questionnaire (MEQ) and applies age-related phase shift logic to ensure accuracy across different life stages.

**Q: Can I use this to improve my work schedule?**
Yes. By using `get_performance_peaks`, you can identify when you are most alert to schedule deep work and high-priority tasks.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/sleep-chronotype-assessment](https://vinkius.com/en/ai-agent-connect/sleep-chronotype-assessment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sleep Chronotype Assessment** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sleep-chronotype-assessment` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sleep Chronotype Assessment** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sleep-chronotype-assessment": {
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
