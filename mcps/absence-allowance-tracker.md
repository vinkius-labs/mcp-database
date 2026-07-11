# Absence Allowance Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/absence-allowance-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Monitor student attendance against school policies and identify unexcused absence thresholds.

## Description
The Absence Allowance Tracker is a specialized tool for educational administrators and students to monitor attendance metrics. Using `get_attendance_summary`, you can calculate the proportion of days attended versus total scheduled days. The `get_policy_status` tool evaluates how close a student is to violating unexcused absence limits, providing 'Safe', 'Warning', or 'Critical' statuses. For schools using alternating schedules, `calculate_block_schedule_impact` provides independent metrics for both A and B day cycles, ensuring accurate tracking of attendance patterns in block schedule environments.


## Available Tools (3)
- **get_attendance_summary**: Get a high-level overview of current attendance standing
- **calculate_block_schedule_impact**: Calculate metrics for A/B alternating schedules
- **get_policy_status**: Evaluate how close a student is to violating attendance policy


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Absence Allowance Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my current attendance percentage if I have 180 total school days, 5 excused absences, and 2 unexcused absences?"

**🤖 AI Agent:**
> You have attended 173 days out of 180, which is an attendance percentage of approximately 96.11%.

---

**👤 You:**
> "Check my policy status. I have 8 unexcused absences and the limit is 10."

**🤖 AI Agent:**
> Your current status is 'Warning' because you only have 2 unexcused absences remaining before hitting the limit.

---

**👤 You:**
> "Calculate impact for a block schedule: A days total is 90 with 2 absences, B days total is 90 with 0 absences."

**🤖 AI Agent:**
> For the A day cycle, your status is safe. For the B day cycle, your status is also safe. Both cycles are currently within safe limits.


## ❓ FAQ

**Q: How does the tool calculate attendance percentage?**
The tool subtracts both excused and unexcused absences from the total scheduled school days to determine the number of days attended, then calculates the ratio.

**Q: Can I track A/B block schedules?**
Yes, by using the `calculate_block_schedule_impact` tool, you can evaluate attendance for A and B cycles as independent datasets.

**Q: What does a 'Warning' status mean?**
A 'Warning' status is triggered when the remaining unexcused absence allowance reaches a low critical margin, alerting you that a policy violation is imminent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/absence-allowance-tracker](https://vinkius.com/mcp/absence-allowance-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Absence Allowance Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `absence-allowance-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Absence Allowance Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "absence-allowance-tracker": {
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
