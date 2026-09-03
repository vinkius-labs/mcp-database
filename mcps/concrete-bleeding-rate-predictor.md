# Concrete Bleeding Rate Predictor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/concrete-bleeding-rate-predictor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Predicts water bleeding rates, total volume, and finishing windows for fresh concrete mixes.

## Description
This MCP server provides professional-grade calculation tools for predicting water bleeding in fresh concrete. It allows AI agents to determine the instantaneous `get_bleeding_rate`, calculate the `get_total_bleeding_volume`, and predict the optimal `get_finishing_window` for mechanical finishing. By analyzing mix proportions, cement fineness, and air entrainment, it helps prevent surface defects and ensures structural integrity during the concrete setting process.


## Available Tools (4)
- **analyze_mix_stability**: Evaluates how the specific combination of aggregates and air entrainment affects the overall bleeding behavior
- **get_bleeding_rate**: Calculates the instantaneous rate of water loss at the surface
- **get_finishing_window**: Predicts the time interval during which the concrete is ready for mechanical finishing
- **get_total_bleeding_volume**: Determines the total amount of water that will migrate to the surface for a specific mix


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Concrete Bleeding Rate Predictor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the bleeding rate for a mix with 300kg cement, 180L water, and 40% fine aggregate at 25°C?"

**🤖 AI Agent:**
> The calculated bleeding rate for this specific mix is 0.45 kg/m²/h.

---

**👤 You:**
> "When is the best time to start troweling this concrete?"

**🤖 AI Agent:**
> Mechanical finishing can begin 3 hours after placement and must be completed by 6 hours to avoid surface damage.

---

**👤 You:**
> "How much total water will bleed from this mix?"

**🤖 AI Agent:**
> The total bleeding volume for this concrete mix is 8.2 kg/m³.


## ❓ FAQ

**Q: What is the purpose of the `get_bleeding_rate` tool?**
The `get_bleeding_rate` tool calculates the instantaneous rate of water loss at the surface in kg/m²/h based on mix proportions and environmental factors.

**Q: How can I find the best time to finish the concrete surface?**
You can use the `get_finishing_window` tool to predict the specific time interval (in hours after placement) when the concrete is ready for mechanical finishing.

**Q: Does the tool account for chemical admixtures?**
Yes, the tools allow you to specify the `admixtureType`, such as water reducers or air entrainers, to ensure accurate predictions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/concrete-bleeding-rate-predictor](https://vinkius.com/ai-agent-connect/concrete-bleeding-rate-predictor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Concrete Bleeding Rate Predictor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `concrete-bleeding-rate-predictor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Concrete Bleeding Rate Predictor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "concrete-bleeding-rate-predictor": {
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
