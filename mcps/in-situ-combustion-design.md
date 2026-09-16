# In-Situ Combustion Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/in-situ-combustion-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Simulate and optimize fire flood processes by scaling combustion tube data to field-scale operations.

## Description
This MCP server provides engineering tools to design and optimize in-situ combustion (ISC) processes. It allows users to scale laboratory combustion tube results to full-scale reservoir operations by calculating critical parameters like air injection rates, fuel consumption, and burn front velocity. Use `calculate_air_injection_rate` to stabilize the combustion front, `predict_fuel_consumption` to estimate oil loss, `estimate_burn_front_velocity` to predict front migration, and `evaluate_recovery_efficiency` to assess total oil recovery and breakthrough risks.


## Available Tools (4)
- **calculate_air_injection_rate**: Determines the required rate of air injection to maintain a stable combustion front
- **estimate_burn_front_velocity**: Predicts how fast the combustion front will migrate through the reservoir
- **evaluate_recovery_efficiency**: Calculates the expected oil recovery based on combustion parameters and breakthrough risks
- **predict_fuel_consumption**: Estimates how much oil will be consumed to sustain the combustion process


## 💬 Prompt Examples

Here are some examples of how you can interact with the **In-Situ Combustion Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What air injection rate do I need for a reservoir of 500,000 m3 with a target velocity of 0.05 m/day, 0.21 oxygen, and 0.15 permeability?"

**🤖 AI Agent:**
> The required air injection rate is 1250.5 m3/day with an expected pressure drop of 15.2 bar.

---

**👤 You:**
> "How much oil will be consumed if the initial saturation is 0.7, efficiency is 0.4, and the burn front volume is 50,000 m3?"

**🤖 AI Agent:**
> The total fuel consumed will be 14,000 m3, leaving 21,000 m3 of residual oil.

---

**👤 You:**
> "Predict the front velocity for an injection rate of 1000 m3/day, reactivity of 0.8, porosity of 0.25, and oxygen utilization of 0.7."

**🤖 AI Agent:**
> The predicted burn front velocity is 0.12 m/day, with an estimated time until breakthrough of 450 days.


## ❓ FAQ

**Q: How can I determine the required air supply?**
You can use the `calculate_air_injection_rate` tool to determine the necessary air volume per unit of time based on your reservoir volume and target front velocity.

**Q: Can I predict when air might reach the production well?**
Yes, the `estimate_burn_front_velocity` tool provides an estimated time until breakthrough, helping you manage oxygen utilization and prevent premature air arrival.

**Q: How is the total oil recovery calculated?**
The `evaluate_recovery_efficiency` tool calculates the expected recovery factor and volume by weighing the oil in place against front velocity and breakthrough risks.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/in-situ-combustion-design](https://vinkius.com/en/ai-agent-connect/in-situ-combustion-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **In-Situ Combustion Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `in-situ-combustion-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **In-Situ Combustion Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "in-situ-combustion-design": {
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
