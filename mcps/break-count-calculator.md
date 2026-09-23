# Break Count Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/break-count-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate mandatory break counts and schedules based on work duration.

## Description
This MCP server provides precision tools for managing work schedules and rest periods. It allows AI agents to determine the total number of breaks earned, generate chronological break schedules, validate work configurations against policy, and calculate work efficiency metrics. Use `get_break_count` to find total rest periods, `get_break_schedule` for timing, `validate_break_parameters` for policy compliance, and `get_work_efficiency_metrics` to analyze time lost to breaks.


## Available Tools (4)
- **get_break_count**: Determines how many breaks a worker is entitled to based on their shift
- **get_break_schedule**: Generates a chronological list of when each break should occur
- **get_work_efficiency_metrics**: Calculates the ratio of actual work time to total duration
- **validate_break_parameters**: Checks if a specific work and break configuration is logically sound


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Break Count Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many breaks will I get in an 8-hour shift if I take a break every 60 minutes?"

**🤖 AI Agent:**
> You are entitled to 7 breaks during an 8-hour shift with a 60-minute interval.

---

**👤 You:**
> "Give me a schedule for a 4-hour work session with breaks every 45 minutes."

**🤖 AI Agent:**
> Your breaks should occur at 45, 90, 135, and 180 minutes.

---

**👤 You:**
> "Is a 30-minute break interval valid for a 2-hour work session?"

**🤖 AI Agent:**
> Yes, the configuration is valid.


## ❓ FAQ

**Q: How do I calculate the total number of breaks?**
You can use the `get_break_count` tool by providing the total work duration and the desired break interval in minutes.

**Q: Can I check if my break schedule follows company policy?**
Yes, the `validate_break_parameters` tool checks if your work and break configuration is logically sound and compliant.

**Q: How is work efficiency calculated?**
The `get_work_efficiency_metrics` tool calculates the ratio of actual work time to total duration, accounting for time lost to breaks.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/break-count-calculator](https://vinkius.com/en/ai-agent-connect/break-count-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Break Count Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `break-count-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Break Count Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "break-count-calculator": {
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
