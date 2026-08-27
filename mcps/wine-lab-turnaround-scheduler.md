# Wine Lab Turnaround Scheduler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wine-lab-turnaround-scheduler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Optimize wine laboratory throughput and minimize turnaround time during harvest.

## Description
This MCP server provides high-precision scheduling for wine laboratory workflows. It connects AI agents to critical winery operations, allowing for real-time management of laboratory capacity and sample routing. Use `get_current_capacity` to monitor available resources, `calculate_daily_throughput` to predict processing limits, `schedule_sample_batch` to optimize sample grouping, and `identify_bottlenecks` to detect delays in analysis types like YAN or Brix. It is designed to handle the high-pressure demands of the harvest period by prioritizing time-critical nutrient and spoilage assessments.


## Available Tools (4)
- **calculate_daily_throughput**: Estimates how many samples of various types can be processed in a single day
- **get_current_capacity**: Checks the available laboratory resources and current workload
- **identify_bottlenecks**: Identifies which specific analysis type or equipment is causing delays
- **schedule_sample_batch**: Determines the optimal timing and grouping for a new set of samples


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Lab Turnaround Scheduler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current capacity of lab_001?"

**🤖 AI Agent:**
> The current capacity for lab_001 shows 75% utilization with 4 hours of available time remaining.

---

**👤 You:**
> "Schedule a batch for 50L of wine with Brix and YAN analysis, marking it as time-critical."

**🤖 AI Agent:**
> The batch has been scheduled (ID: B-992). It is set to start immediately due to the time-critical flag, with an estimated completion in 45 minutes.

---

**👤 You:**
> "Are there any bottlenecks expected in the next 12 hours?"

**🤖 AI Agent:**
> A primary bottleneck is identified in YAN analysis, with an estimated delay of 30 minutes due to high sample volume.


## ❓ FAQ

**Q: How does the scheduler handle urgent YAN testing?**
By using the `isTimeCritical` flag in `schedule_sample_batch`, the system prioritizes YAN samples to ensure immediate nutrient assessment and prevent fermentation issues.

**Q: Can I check if the lab is overloaded?**
Yes, you can use `identify_bottlenecks` to find specific analysis types causing delays or `get_current_capacity` to see the current utilization levels.

**Q: What analysis types are supported?**
The system supports standard wine analyses including Brix, pH, TA, YAN, and VA.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wine-lab-turnaround-scheduler](https://vinkius.com/ai-agent-connect/wine-lab-turnaround-scheduler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Lab Turnaround Scheduler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-lab-turnaround-scheduler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Lab Turnaround Scheduler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-lab-turnaround-scheduler": {
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
