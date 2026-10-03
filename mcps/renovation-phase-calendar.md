# Renovation Phase Calendar MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/renovation-phase-calendar)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Schedules renovation phases by synchronizing tasks, dependencies, and resource availability.

## Description
This MCP server provides a specialized scheduling engine for renovation projects. It calculates precise timelines by synchronizing task durations, logical dependencies, contractor availability, inspection gates, and material lead times against a fixed target completion date. Use `get_project_timeline` to generate full schedules, `identify_critical_dependencies` to find bottlenecks, `check_resource_conflicts` to detect contractor overbooking, and `simulate_scenario` to evaluate how changes impact the final deadline.


## Available Tools (4)
- **check_resource_conflicts**: Detects overlapping task assignments where a contractor is scheduled for multiple tasks simultaneously
- **get_project_timeline**: Generates the full schedule of all renovation phases including start and end dates
- **identify_critical_dependencies**: Pinpoints specific constraints that are causing delays or driving the project end date
- **simulate_scenario**: Evaluates how changing a single variable affects the final deadline


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Renovation Phase Calendar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a full renovation schedule for my project."

**🤖 AI Agent:**
> The renovation schedule is ready. The foundation starts on May 1st and ends on May 10th, followed by framing from May 11th to May 20th.

---

**👤 You:**
> "What is causing the delay in my renovation timeline?"

**🤖 AI Agent:**
> The primary bottleneck is the 14-day lead time for custom windows, which is pushing the final completion date back.

---

**👤 You:**
> "What happens if I add an extra electrician to the team?"

**🤖 AI Agent:**
> Adding an extra electrician will reduce the electrical phase duration by 3 days, allowing the project to finish earlier.


## ❓ FAQ

**Q: How can I see my full renovation schedule?**
You can use the `get_project_timeline` tool to generate a complete list of all renovation phases, including their specific start and end dates.

**Q: How do I find out what is delaying my project?**
Use the `identify_critical_dependencies` tool to pinpoint specific tasks, material lead times, or inspection gates that are driving the project end date.

**Q: Can I check if my contractors are overbooked?**
Yes, the `check_resource_conflicts` tool detects overlapping task assignments and ensures contractors are working within their authorized availability windows.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/renovation-phase-calendar](https://vinkius.com/en/ai-agent-connect/renovation-phase-calendar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Renovation Phase Calendar** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `renovation-phase-calendar` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Renovation Phase Calendar** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "renovation-phase-calendar": {
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
