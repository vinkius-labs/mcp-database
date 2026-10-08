# Recovery Day Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/recovery-day-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automated scheduling for optimal athletic recovery.

## Description
This MCP server connects AI agents to your training calendar to optimize athletic performance. It automatically inserts mandatory rest and low-intensity recovery periods between training sessions based on your specific recovery requirements and availability. Use `schedule_recovery_plan` to generate a full schedule, `validate_recovery_gap` to check if you have enough downtime between sessions, or `calculate_recovery_efficiency` to evaluate your current plan.


## Available Tools (4)
- **calculate_recovery_efficiency**: Evaluates how well a proposed schedule meets the recovery needs relative to the training load
- **find_available_slots**: Identifies continuous blocks of time within the user's availability that are long enough to accommodate specific recovery needs
- **schedule_recovery_plan**: Generates a complete recovery schedule by inserting rest or low-intensity days between existing training sessions
- **validate_recovery_gap**: Checks if a specific interval between two activities meets the biological recovery requirements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Recovery Day Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a recovery plan for my training sessions: Monday 8am-10am (4h recovery), Wednesday 9am-11am (4h recovery). I am available all day Tuesday and Thursday."

**🤖 AI Agent:**
> Your recovery plan is ready: Monday training, Tuesday rest, Wednesday training, Thursday low-intensity.

---

**👤 You:**
> "Is a 3-hour gap enough if I need 4 hours of recovery?"

**🤖 AI Agent:**
> No, a 3-hour gap is insufficient as it does not meet the required 4 hours of recovery.

---

**👤 You:**
> "Find me a 5-hour slot in my availability: Monday 1pm-6pm and Tuesday 9am-12pm."

**🤖 AI Agent:**
> The available slot is Monday from 1:00 PM to 6:00 PM.


## ❓ FAQ

**Q: How do I generate a full recovery schedule?**
You can use the `schedule_recovery_plan` tool by providing your training sessions and available time blocks.

**Q: Can I check if my current gap between workouts is sufficient?**
Yes, use the `validate_recovery_gap` tool to verify if the time between your last session end and next session start meets your required recovery hours.

**Q: How is the recovery efficiency calculated?**
The `calculate_recovery_efficiency` tool evaluates how well your schedule meets recovery needs by comparing provided recovery hours against the total required hours.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/recovery-day-planner](https://vinkius.com/en/ai-agent-connect/recovery-day-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Recovery Day Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `recovery-day-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Recovery Day Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "recovery-day-planner": {
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
