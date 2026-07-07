# Reverse Sleep Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/reverse-sleep-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate your ideal bedtime by counting backwards from your wake-up time.

## Description
Determine the optimal time to go to bed based on your target wake-up time, accounting for sleep latency and complete 90-minute sleep cycles. Using the `calculate_bed_time_schedule` tool, you can find both your primary ideal bedtime and a fallback window if you miss your first opportunity.


## Available Tools (3)
- **calculate_bed_time_schedule**: Calculates ideal bedtime and a fallback time
- **get_sleep_cycle_metrics**: Provides duration metrics for sleep cycles
- **validate_sleep_constraints**: Validates if sleep parameters are realistic


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reverse Sleep Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I need to wake up at 07:00. I usually take 20 minutes to fall asleep, and I want 5 cycles of sleep."

**🤖 AI Agent:**
> To wake up at 07:00 with 20 minutes of latency and 5 cycles, your ideal bedtime is 22:10. Your fallback bedtime is 23:40.

---

**👤 You:**
> "Check if my sleep plan for 6 cycles with 30 minutes of latency is realistic."

**🤖 AI Agent:**
> Yes, your parameters are within human-realistic bounds.

---

**👤 You:**
> "How many minutes are in a sleep cycle?"

**🤖 AI Agent:**
> The duration of a single cycle is 90 minutes.


## ❓ FAQ

**Q: How does the calculation work?**
The tool subtracts your estimated sleep latency from your target wake time, then subtracts the total duration of your desired 90-minute sleep cycles.

**Q: What is a sleep cycle?**
A single sleep cycle lasts approximately 90 minutes. You can use `get_sleep_cycle_metrics` to see the total time required for a specific number of cycles.

**Q: Does it account for how long it takes me to fall asleep?**
Yes, by providing your sleep latency in minutes, the `calculate_bed_time_schedule` tool ensures your schedule is accurate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/reverse-sleep-calculator](https://vinkius.com/mcp/reverse-sleep-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Reverse Sleep Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `reverse-sleep-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Reverse Sleep Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "reverse-sleep-calculator": {
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
