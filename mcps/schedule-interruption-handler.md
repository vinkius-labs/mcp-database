# Schedule Interruption Handler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/schedule-interruption-handler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [automation](../categories/automation.md)

Adjust medical or procedural schedules based on missed doses and interruptions.

## Description
The Schedule Interruption Handler is a specialized tool for managing time-sensitive regimens. When an unplanned gap occurs in a schedule, this MCP server allows AI agents to recalculate the timeline without losing progress. Using `calculate_underrun`, you can determine how many weeks are added to your completion date. The `get_resumed_schedule` tool generates the new sequence of instructions from the point of resumption, ensuring that the dosage remains stable despite the advancement of the virtual clock. Additionally, `get_interruption_summary` provides a human-readable explanation of the disruption's impact.


## Available Tools (3)
- **calculate_underrun**: Calculate the impact of a schedule interruption on completion date
- **get_interruption_summary**: Get a summary of the schedule interruption
- **get_resumed_schedule**: Generate the adjusted schedule following an interruption


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Schedule Interruption Handler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I missed 3 weeks of my treatment starting from week 5. What is the new completion date?"

**🤖 AI Agent:**
> The schedule has been extended by 3 weeks. Your new target completion week is now week 15.

---

**👤 You:**
> "Generate a new schedule for me after a 2-week interruption at week 10, where my dose was 5mg."

**🤖 AI Agent:**
> The adjusted schedule starting from week 12 will continue with a dosage of 5mg for all subsequent weeks in the sequence.

---

**👤 You:**
> "Summarize the impact of missing 6 weeks starting at week 2."

**🤖 AI Agent:**
> A major interruption occurred. The schedule was paused for 6 weeks, and while the virtual clock advanced, your dosage level remained stable.


## ❓ FAQ

**Q: How does the tool handle missed weeks?**
The tool uses a 'virtual clock' approach. It advances the timeline by the number of missed weeks without changing the active dosage, ensuring the integrity of the regimen is maintained.

**Q: Does the dosage change during an interruption?**
No. The `get_resumed_schedule` tool ensures that every entry in the new sequence retains the exact same dosage value that was active at the time of the interruption.

**Q: Can I see the impact on my final completion date?**
Yes, by using the `calculate_underrun` tool, you can identify the new target completion week and the total extension duration caused by the gap.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/schedule-interruption-handler](https://vinkius.com/mcp/schedule-interruption-handler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Schedule Interruption Handler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `schedule-interruption-handler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Schedule Interruption Handler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "schedule-interruption-handler": {
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
