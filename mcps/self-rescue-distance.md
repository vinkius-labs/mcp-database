# Self-Rescue Distance MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/self-rescue-distance)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [maritime](../categories/maritime.md)

Assess kiteboarding self-rescue capability and drift risk.

## Description
This MCP server provides critical safety assessments for kiteboarders facing equipment failure. It calculates the feasibility of reaching shore by analyzing wind speed, current speed, and distance to land. Using `calculate_rescue_feasibility`, riders can determine if they can safely paddle to safety. The tool also includes `analyze_drift_risk` to predict movement if stationary, `evaluate_fitness_impact` to scale energy needs, and `get_safety_protocol` to provide immediate emergency instructions.


## Available Tools (4)
- **get_safety_protocol**: Provides standardized emergency procedures based on the calculated rescue outcome
- **analyze_drift_risk**: Predicts how much a rider will be pushed away from their target if they remain stationary
- **calculate_rescue_feasibility**: Determines if a rider can safely reach the shore based on current environmental conditions and personal capability
- **evaluate_fitness_impact**: Adjusts the estimated effort required based on the rider's specific fitness level


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Self-Rescue Distance** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am 500 meters from shore, wind is 10 m/s, and current is 0.5 m/s. My fitness is medium and my kite is functional. Can I make it?"

**🤖 AI Agent:**
> Yes, you can safely reach the shore. Estimated time is approximately 12 minutes.

---

**👤 You:**
> "How much will I drift if I stay still with a 15 m/s wind and 1 m/s current and a functional kite?"

**🤖 AI Agent:**
> You are estimated to drift 150 meters offshore.

---

**👤 You:**
> "I'm 800 meters out, wind is 12 m/s, current is 1.5 m/s, fitness is low, and my kite is damaged. What should I do?"

**🤖 AI Agent:**
> It is not safe to attempt paddling. Deploy flotation and wait for rescue.


## ❓ FAQ

**Q: How accurate is the rescue feasibility calculation?**
The calculation uses a physics-based model factoring in wind, current, and rider fitness to estimate if you can reach shore using `calculate_rescue_feasibility`.

**Q: Can I use this to predict where I will drift?**
Yes, you can use `analyze_drift_risk` to estimate the distance and direction you might be pushed by wind and current.

**Q: What happens if my kite is damaged?**
The tools account for `kiteCondition`. A damaged kite affects both buoyancy and how much the wind pulls you, which is reflected in the safety protocols.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/self-rescue-distance](https://vinkius.com/ai-agent-connect/self-rescue-distance)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Self-Rescue Distance** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `self-rescue-distance` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Self-Rescue Distance** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "self-rescue-distance": {
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
