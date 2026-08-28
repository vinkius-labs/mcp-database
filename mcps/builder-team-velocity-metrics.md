# Builder Team Velocity Metrics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/builder-team-velocity-metrics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Analyzes software team productivity using velocity, quality, and delivery speed metrics.

## Description
This MCP server provides a specialized analytics engine to evaluate software builder team productivity. It synthesizes sprint velocity, team capacity, cycle time, and defect rates into actionable insights. Use `get_velocity_per_member` to determine individual throughput, `calculate_efficiency_score` to balance output against quality, `evaluate_delivery_speed` to analyze pipeline flow, and `identify_improvement_areas` to pinpoint specific bottlenecks like Quality, Flow, or Capacity Utilization.


## Available Tools (4)
- **calculate_efficiency_score**: Provides a single holistic metric of team performance by balancing output and quality
- **evaluate_delivery_speed**: Analyzes how quickly the team moves work through the pipeline
- **get_velocity_per_member**: Determines the individual throughput capacity of a team
- **identify_improvement_areas**: Pinpoints specific bottlenecks within the team's workflow


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Builder Team Velocity Metrics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the individual throughput for a team of 5 members that completed 40 story points?"

**🤖 AI Agent:**
> The velocity per member is 8 story points.

---

**👤 You:**
> "Our team has a 15% defect rate, 50 velocity, 1.2 maturity, and 1.0 complexity. What is our efficiency?"

**🤖 AI Agent:**
> Your efficiency score is 0.85, which is rated as Optimal.

---

**👤 You:**
> "The team has a cycle time of 10 days and a complexity factor of 1.5. How is our delivery speed?"

**🤖 AI Agent:**
> The delivery rhythm is currently Fluid.


## ❓ FAQ

**Q: How does this tool calculate team efficiency?**
The `calculate_efficiency_score` tool calculates a normalized value by balancing sprint velocity against the defect rate, while adjusting for team maturity and task complexity.

**Q: Can I identify specific workflow bottlenecks?**
Yes, by using `identify_improvement_areas`, the system can detect if the primary bottleneck is Quality, Flow, or Capacity Utilization.

**Q: What metrics are required for velocity analysis?**
To calculate individual throughput, you need to provide the total sprint velocity and the total number of active team members to the `get_velocity_per_member` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/builder-team-velocity-metrics](https://vinkius.com/ai-agent-connect/builder-team-velocity-metrics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Builder Team Velocity Metrics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `builder-team-velocity-metrics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Builder Team Velocity Metrics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "builder-team-velocity-metrics": {
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
