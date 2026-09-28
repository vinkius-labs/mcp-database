# School Morning Readiness Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/school-morning-readiness-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Synchronize family routines using backward scheduling and task dependency logic.

## Description
Transform school start times into a precise morning execution plan. This MCP uses backward scheduling to work back from your departure time, ensuring all tasks like dressing and eating are completed on time. It manages task dependencies, assigns responsibilities to adults and children, and provides contingency steps if you fall behind schedule. Use `get_morning_sequence` to build your timeline and `get_responsibility_chart` to coordinate family members.


## Available Tools (4)
- **get_morning_sequence**: Generates the chronological timeline of activities for the morning
- **get_responsibility_chart**: Assigns specific tasks to adults or children to prevent scheduling conflicts
- **get_contingency_plan**: Provides specific actions to take if the morning falls behind schedule
- **get_evening_prep_list**: Identifies what must be prepared the night before to ensure a smooth morning


## 💬 Prompt Examples

Here are some examples of how you can interact with the **School Morning Readiness Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a morning schedule for a school start time of 08:30 with a 20 minute travel time. The routine should include waking up, dressing, and breakfast."

**🤖 AI Agent:**
> Your departure time is 08:10. The sequence is: 07:10 - 07:30 Waking up, 07:30 - 07:50 Dressing, 07:50 - 08:10 Breakfast.

---

**👤 You:**
> "What should I prepare the night before if I need to pack lunchboxes and set out uniforms?"

**🤖 AI Agent:**
> You should pack the lunchboxes and lay out the school uniforms.

---

**👤 You:**
> "We are 10 minutes behind schedule. What should we do?"

**🤖 AI Agent:**
> To catch up, you should shorten breakfast time or skip optional tasks like packing extra snacks.


## ❓ FAQ

**Q: How does the scheduling logic work?**
The engine uses backward scheduling, starting from the school start time and subtracting travel duration to find the required departure time, then building the routine backwards from there.

**Q: Can I assign tasks to specific family members?**
Yes, by using the `get_responsibility_chart` tool, you can map tasks to adults and children based on their availability.

**Q: What happens if we are running late?**
You can use `get_contingency_plan` to receive actionable steps, such as skipping flexible tasks, to get back on track.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/school-morning-readiness-plan](https://vinkius.com/en/ai-agent-connect/school-morning-readiness-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **School Morning Readiness Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `school-morning-readiness-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **School Morning Readiness Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "school-morning-readiness-plan": {
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
