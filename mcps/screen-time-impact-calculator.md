# Screen Time Impact Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/screen-time-impact-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Assess the physiological and productivity costs of digital device usage.

## Description
The Screen Time Impact Calculator helps you understand how your digital habits affect your well-being. Use `calculate_exposure_risk` to determine eye strain levels from phone, computer, and TV use. Evaluate sleep disruption with `calculate_sleep_impact` based on pre-bedtime usage. Project potential efficiency gains using `project_productivity_gains` by comparing current hours to target goals. Finally, create a sustainable reduction strategy with `generate_detox_plan`, which provides a week-by-week schedule for gradual digital detox.


## Available Tools (4)
- **generate_detox_plan**: Generate a digital detox reduction schedule
- **calculate_exposure_risk**: Calculate eye strain risk and blue light exposure
- **project_productivity_gains**: Project productivity gains from reduced screen time
- **calculate_sleep_impact**: Calculate impact of screen time on sleep


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Screen Time Impact Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my eye strain risk if I spend 5 hours on my phone, 6 hours on my computer, and 2 hours watching TV?"

**🤖 AI Agent:**
> Your eye strain risk is High. Your blue light exposure score is 78/100 due to significant high-proximity device usage.

---

**👤 You:**
> "I currently use screens for 8 hours a day, but I want to drop to 4 hours. How much time can I reclaim and what is the productivity boost?"

**🤖 AI Agent:**
> By reaching your target, you will reclaim 4 hours per day. This is projected to provide a 15% boost in your task efficiency and focus.

---

**👤 You:**
> "Create a 4-week plan to reduce my daily screen time from 9 hours down to 5 hours."

**🤖 AI Agent:**
> Your detox plan is ready: Week 1: 8.0 hours, Week 2: 7.0 hours, Week 3: 6.0 hours, Week 4: 5.0 hours.


## ❓ FAQ

**Q: How does the eye strain calculation work?**
The `calculate_exposure_risk` tool weights usage based on device proximity. High-proximity devices like phones and computers contribute more to your risk score than TVs.

**Q: Can I plan a gradual reduction in my screen time?**
Yes, the `generate_detox_plan` tool creates a multi-week schedule that incrementally lowers your daily limit to prevent rebound usage.

**Q: Does this tool account for sleep disruption?**
Yes, using `calculate_sleep_impact`, you can see how screen use in the hours before bed increases sleep latency and affects your overall sleep quality.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/screen-time-impact-calculator](https://vinkius.com/mcp/screen-time-impact-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Screen Time Impact Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `screen-time-impact-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Screen Time Impact Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "screen-time-impact-calculator": {
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
