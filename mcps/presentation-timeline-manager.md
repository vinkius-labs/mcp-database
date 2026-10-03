# Presentation Timeline Manager MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/presentation-timeline-manager)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Schedules research, slides, rehearsal, and feedback around a presentation date.

## Description
This MCP server manages the end-to-end preparation lifecycle for presentations. It uses backward scheduling to ensure all critical phases--Research, Slide Creation, Feedback, and Rehearsal--are completed with a sufficient safety buffer before the final delivery. Use `get_timeline_milestones` to generate a full schedule, `validate_phase_sequence` to ensure logical flow, `calculate_buffer_margin` to check safety time, and `check_phase_readiness` to verify if a phase can begin.


## Available Tools (4)
- **calculate_buffer_margin**: Determines the amount of available safety time between the end of the rehearsal phase and the delivery date
- **check_phase_readiness**: Determines if a specific phase can begin based on the status of its predecessor
- **get_timeline_milestones**: Provides a full schedule of all necessary preparation milestones based on a target date
- **validate_phase_sequence**: Checks if a proposed sequence of tasks follows the logical flow of preparation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Presentation Timeline Manager** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a timeline for a presentation on December 15, 2024."

**🤖 AI Agent:**
> Here is your presentation schedule: Research must be completed by Nov 10, Slide Creation by Nov 25, Feedback by Dec 1, and Rehearsal by Dec 10.

---

**👤 You:**
> "Is it okay to start Slide Creation if I haven't finished Research yet?"

**🤖 AI Agent:**
> No, you cannot start Slide Creation until the Research phase is marked as completed.

---

**👤 You:**
> "Check if my sequence [Research, Slide Creation, Rehearsal] is valid."

**🤖 AI Agent:**
> The sequence is invalid because the Feedback phase is missing between Slide Creation and Rehearsal.


## ❓ FAQ

**Q: How do I generate a complete schedule?**
You can use the `get_timeline_milestones` tool by providing your target presentation date in ISO format.

**Q: Can I check if my preparation order is correct?**
Yes, the `validate_phase_sequence` tool checks if your planned phases follow the mandatory Research to Rehearsal sequence.

**Q: How do I know if I have enough time before my presentation?**
Use the `calculate_buffer_margin` tool to determine the number of safety days between your final rehearsal and the presentation date.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/presentation-timeline-manager](https://vinkius.com/en/ai-agent-connect/presentation-timeline-manager)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Presentation Timeline Manager** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `presentation-timeline-manager` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Presentation Timeline Manager** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "presentation-timeline-manager": {
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
