# Smart Well Control Optimization MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/smart-well-control-optimization)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [optimization](../categories/optimization.md)

Optimize ICV settings to maximize oil recovery and manage production constraints.

## Description
This MCP server provides advanced optimization capabilities for intelligent wells. It allows AI agents to analyze reservoir characteristics using `get_zonal_analysis`, determine optimal valve positions via `calculate_icv_optimization`, and verify operational safety with `validate_control_schedule`. Additionally, it can assess the impact of new telemetry through `simulate_realtime_impact` to ensure production plans remain reliable as reservoir conditions change.


## Available Tools (4)
- **validate_control_schedule**: Verifies if a proposed sequence of ICV adjustments is safe and feasible
- **calculate_icv_optimization**: Determines the best valve positions to meet a specific production goal
- **get_zonal_analysis**: Provides a summary of current reservoir characteristics for all zones in a specific well
- **simulate_realtime_impact**: Predicts how real-time sensor updates will affect the current optimization plan


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Smart Well Control Optimization** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the current reservoir characteristics for well-123?"

**🤖 AI Agent:**
> Well-123 has three zones: Zone A has 15% porosity and 200mD permeability, Zone B has 12% porosity and 150mD permeability, and Zone C has 18% porosity and 300mD permeability.

---

**👤 You:**
> "Find the optimal ICV settings for well-456 to maximize oil while keeping water cut below 10%."

**🤖 AI Agent:**
> The optimal settings for well-456 are: Zone 1 at 85% opening, Zone 2 at 40% opening, and Zone 3 at 75% opening. This is expected to increase recovery by 4.2%.

---

**👤 You:**
> "Is this schedule safe: [{ "zoneId": "Z1", "valvePosition": 90, "timestamp": "2024-05-01T10:00:00Z" }] for well-789?"

**🤖 AI Agent:**
> The proposed schedule for well-789 is valid and respects all current production constraints.


## ❓ FAQ

**Q: How can I find the best valve settings for my well?**
You can use the `calculate_icv_optimization` tool to determine the best valve positions based on your specific objectives, such as maximizing oil or minimizing water.

**Q: Can I check if a planned adjustment is safe?**
Yes, the `validate_control_schedule` tool verifies if a proposed sequence of ICV adjustments respects mechanical limits and production constraints.

**Q: How does the tool handle new sensor data?**
The `simulate_realtime_impact` tool predicts how new telemetry, like pressure or flow rate updates, will affect your current optimization plan.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/smart-well-control-optimization](https://vinkius.com/en/ai-agent-connect/smart-well-control-optimization)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Smart Well Control Optimization** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `smart-well-control-optimization` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Smart Well Control Optimization** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "smart-well-control-optimization": {
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
