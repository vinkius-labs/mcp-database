# Paddling Cadence Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/paddling-cadence-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [performance](../categories/performance.md)

Optimize your paddling efficiency with real-time cadence, power, and endurance analysis.

## Description
This MCP server connects AI agents to advanced paddling performance metrics. It provides precise guidance for paddlers by calculating the `get_optimal_cadence` based on fitness and water conditions, determining the `get_power_profile` for efficient force application, and generating a tailored `get_endurance_plan` for managing energy. Users can also use `analyze_cadence_efficiency` to compare their actual performance against theoretical targets, ensuring maximum efficiency in both sprint and distance paddling.


## Available Tools (4)
- **analyze_cadence_efficiency**: Evaluates how well a user is performing against their theoretical optimum
- **get_endurance_plan**: Generates a pacing strategy to manage energy depletion
- **get_optimal_cadence**: Determines the target strokes per minute based on user profile and environment
- **get_power_profile**: Provides instructions on how to apply force during the stroke


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Paddling Cadence Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am an intermediate paddler in calm water planning a distance session. What is my optimal cadence?"

**🤖 AI Agent:**
> For an intermediate paddler in calm water focusing on distance, your optimal stroke rate is 52 strokes per minute with a focus on maximizing glide.

---

**👤 You:**
> "I'm an advanced paddler in choppy water. How should I distribute my power for a sprint?"

**🤖 AI Agent:**
> In choppy water during a sprint, you should use a high-frequency, high-stability power distribution to maintain momentum through the waves.

---

**👤 You:**
> "My target cadence was 55 but I am currently at 50. I am an advanced paddler. How efficient am I?"

**🤖 AI Agent:**
> Your efficiency score is 91%, showing a slight deviation from the target rate due to the current environmental resistance.


## ❓ FAQ

**Q: How does the tool determine my optimal stroke rate?**
The `get_optimal_cadence` tool analyzes your fitness level, the current wave conditions, and your specific session goal to calculate the most efficient strokes per minute.

**Q: Can I use this for both sprint and distance paddling?**
Yes, the system provides different strategies for Sprint and Distance goals, adjusting power distribution and endurance plans accordingly.

**Q: How do wave conditions affect my results?**
Wave conditions change the required stability and cadence. The tool adjusts the `get_power_profile` to prioritize stability in rough water or glide in calm water.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/paddling-cadence-optimizer](https://vinkius.com/en/ai-agent-connect/paddling-cadence-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Paddling Cadence Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `paddling-cadence-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Paddling Cadence Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "paddling-cadence-optimizer": {
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
