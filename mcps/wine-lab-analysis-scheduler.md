# Wine Lab Analysis Scheduler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-lab-analysis-scheduler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Optimize laboratory workflows by scheduling critical wine analyses and identifying instrument bottlenecks.

## Description
This MCP server connects AI agents to wine laboratory management systems to optimize the scheduling of chemical and biological analyses. It manages the sample queue by prioritizing time-critical tests like `get_priority_schedule` for YAN (Yeast Assimilable Nitrogen) and VA (Volatile Acidity) to prevent spoilage. The server allows agents to `get_daily_load` to monitor workload, `identify_bottlenecks` to find instrument limitations, and `validate_capacity_feasibility` to ensure laboratory equipment can handle requested analysis volumes.


## Available Tools (4)
- **get_daily_load**: Determine the total workload planned for a specific day
- **get_priority_schedule**: You can optionally filter by a specific sampleId.

Retrieve a ranked list of analyses to be performed based on urgency and queue position
- **identify_bottlenecks**: Locate the specific laboratory instrument limiting the processing speed
- **validate_capacity_feasibility**: Check if the current analysis requests can be physically completed with existing equipment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Lab Analysis Scheduler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total workload planned for tomorrow?"

**🤖 AI Agent:**
> The total workload planned for tomorrow is 480 minutes, consisting of 12 scheduled analyses.

---

**👤 You:**
> "Show me the prioritized list of analyses for sample ID 9876."

**🤖 AI Agent:**
> The prioritized schedule for sample 9876 includes a YAN analysis with a priority score of 95, estimated to start at 08:00 AM.

---

**👤 You:**
> "Is it feasible to run these 5 pH tests and 2 VA tests today?"

**🤖 AI Agent:**
> Yes, the requested analyses are feasible with the current instrument capacity.


## ❓ FAQ

**Q: How does the tool handle urgent wine spoilage tests?**
The system uses `get_priority_schedule` to ensure that high-priority tests like Volatile Acidity (VA) are moved to the front of the queue to prevent spoilage.

**Q: Can I check if the lab has enough equipment for a batch of samples?**
Yes, you can use `validate_capacity_feasibility` to check if the current instrument capacity can accommodate your specific analysis requests.

**Q: How do I find out which instrument is slowing down the lab?**
You can use the `identify_bottlenecks` tool to find the specific instrument with the highest utilization rate during a given period.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-lab-analysis-scheduler](https://vinkius.com/en/ai-agent-connect/wine-lab-analysis-scheduler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Lab Analysis Scheduler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-lab-analysis-scheduler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Lab Analysis Scheduler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-lab-analysis-scheduler": {
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
