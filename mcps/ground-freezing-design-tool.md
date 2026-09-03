# Ground Freezing Design Tool MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/ground-freezing-design-tool)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculates thermal and hydraulic parameters for artificial ground freezing.

## Description
This MCP server provides engineering calculations for Artificial Ground Freezing (AGF) used in excavation stabilization. It allows AI agents to determine the necessary freeze pipe layout using `calculate_pipe_layout`, predict the time required to form an ice wall with `estimate_freezing_duration`, determine coolant requirements via `calculate_brine_properties`, and estimate electrical needs with `estimate_power_requirement`.


## Available Tools (4)
- **calculate_brine_properties**: Determines the required temperature of the coolant to achieve the target ground temperature
- **calculate_pipe_layout**: Determines the number and arrangement of freeze pipes needed to surround the excavation
- **estimate_freezing_duration**: Predicts how many days it will take to establish a continuous ice wall
- **estimate_power_requirement**: Calculates the electrical power needed to drive the freezing process


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ground Freezing Design Tool** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many freeze pipes do I need for a 20m by 10m excavation with 2m spacing?"

**🤖 AI Agent:**
> For a 20m x 10m excavation with 2m spacing, you will need 30 freeze pipes to form a continuous perimeter.

---

**👤 You:**
> "How long will it take to freeze a sand excavation if the target temperature is -10°C?"

**🤖 AI Agent:**
> Based on the sand soil type and a target temperature of -10°C, the estimated freezing duration is 25 days.

---

**👤 You:**
> "What is the required brine temperature for a target ground temperature of -5°C in clay?"

**🤖 AI Agent:**
> To achieve a target ground temperature of -5°C in clay, the required brine temperature is -15°C.


## ❓ FAQ

**Q: What can I calculate with this tool?**
You can calculate the number of freeze pipes, the duration of the freezing process, the required brine temperature, and the total power requirement for an excavation.

**Q: Which soil types are supported?**
The tool supports calculations for Silt, Clay, Sand, and Gravel.

**Q: How do I connect this to my AI client?**
Connect using your personal Connection Token via Vinkius Edge. This works with Cursor, VS Code, Claude Desktop, Windsurf, and any MCP-compatible client.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/ground-freezing-design-tool](https://vinkius.com/ai-agent-connect/ground-freezing-design-tool)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ground Freezing Design Tool** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ground-freezing-design-tool` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ground Freezing Design Tool** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ground-freezing-design-tool": {
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
