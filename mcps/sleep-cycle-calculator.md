# Sleep Cycle Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/sleep-cycle-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [wellness](../categories/wellness.md)

Calculate optimal bedtimes and sleep stage distributions using 90-minute circadian cycles.

## Description
Optimize your rest by aligning your sleep with natural 90-minute circadian cycles. This tool uses `calculate_bedtimes` to provide specific bedtime options based on your desired wake time and sleep latency. It also includes `evaluate_sleep_adequacy` to ensure your sleep duration meets the biological needs of your age group, and `calculate_jet_lag_adjustment` to help you plan for time zone shifts during travel.


## Available Tools (3)
- **calculate_bedtimes**: Determines the best times to go to bed to wake up at a specific time while completing full 90-minute sleep cycles
- **calculate_jet_lag_adjustment**: Determines the necessary circadian adjustment period for travel
- **evaluate_sleep_adequacy**: Checks if the proposed sleep duration meets the biological needs of the user based on their age


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sleep Cycle Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to wake up at 07:00 and it usually takes me 15 minutes to fall asleep. What are my best bedtime options?"

**🤖 AI Agent:**
> To wake up at 07:00, your optimal bedtimes are 21:45 (6 cycles), 23:15 (5 cycles), or 00:45 (4 cycles).

---

**👤 You:**
> "I am an adult and I slept for 6 hours. Is that enough?"

**🤖 AI Agent:**
> No, that is insufficient. As an adult, you require a minimum of 7 hours of sleep, leaving a shortfall of 60 minutes.

---

**👤 You:**
> "I am traveling across 3 time zones. How long will it take to adjust?"

**🤖 AI Agent:**
> You will need 3 days to adjust to the new time zone.


## ❓ FAQ

**Q: How do 90-minute sleep cycles work?**
The human sleep pattern is composed of repeating cycles that typically last approximately 90 minutes. Using `calculate_bedtimes` helps you wake up at the end of a cycle to minimize sleep inertia.

**Q: Can I check if I am getting enough sleep?**
Yes, you can use `evaluate_sleep_adequacy` to compare your total sleep duration against the minimum requirements for your age group.

**Q: How do I adjust for jet lag?**
You can use `calculate_jet_lag_adjustment` to determine how many days you need to adjust your internal clock based on the number of time zones you cross.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/sleep-cycle-calculator](https://vinkius.com/ai-agent-connect/sleep-cycle-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sleep Cycle Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sleep-cycle-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sleep Cycle Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sleep-cycle-calculator": {
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
