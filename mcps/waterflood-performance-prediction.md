# Waterflood Performance Prediction MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/waterflood-performance-prediction)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [energy](../categories/energy.md)

Forecast oil recovery, water cut, and sweep efficiency for waterflood operations.

## Description
This MCP server provides specialized simulation tools for forecasting secondary recovery performance in oil reservoirs. It allows AI agents to calculate cumulative oil recovery and water cut evolution using `predict_recovery_evolution`. Users can evaluate reservoir coverage with `analyze_sweep_efficiency`, determine necessary water volumes via `calculate_injection_requirements`, and monitor fluid distribution using `get_saturation_profile`. It is designed to assist in pattern design and injection strategy optimization.


## Available Tools (4)
- **analyze_sweep_efficiency**: Evaluates how well the injected water covers the reservoir area and vertical thickness
- **calculate_injection_requirements**: Determines the amount of water needed to maintain reservoir pressure or meet specific production targets
- **get_saturation_profile**: Provides the distribution of oil and water saturation at a specific point in the flood cycle
- **predict_recovery_evolution**: Forecasts the cumulative oil recovery and water cut over a specified time period


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Waterflood Performance Prediction** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Predict the recovery evolution for a five-spot pattern with an injection rate of 500 barrels per day."

**🤖 AI Agent:**
> The cumulative oil recovery is projected to reach 15% of the original oil in place by year 5, with a water cut of 12% at that time.

---

**👤 You:**
> "What is the total water volume needed to recover 1 million barrels of oil with an efficiency of 0.8?"

**🤖 AI Agent:**
> To recover 1,000,000 barrels of oil with an injection efficiency of 0.8, a total water volume of 1,250,000 barrels is required.

---

**👤 You:**
> "Evaluate the sweep efficiency for a reservoir with a vertical permeability ratio of 0.5."

**🤖 AI Agent:**
> The total sweep efficiency is calculated at 0.65, consisting of an areal sweep of 0.85 and a vertical sweep of 0.76.


## ❓ FAQ

**Q: How can I forecast oil recovery over time?**
You can use the `predict_recovery_evolution` tool by providing reservoir properties, pattern design, injection rate, relative permeability, and the desired time steps.

**Q: Can I calculate the required water injection volume?**
Yes, the `calculate_injection_requirements` tool determines the total water volume and daily rate needed to meet specific production targets.

**Q: How do I check the reservoir saturation levels?**
The `get_saturation_profile` tool provides the distribution of oil and water saturation at any specific point in the flood cycle.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/waterflood-performance-prediction](https://vinkius.com/en/ai-agent-connect/waterflood-performance-prediction)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Waterflood Performance Prediction** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `waterflood-performance-prediction` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Waterflood Performance Prediction** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "waterflood-performance-prediction": {
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
