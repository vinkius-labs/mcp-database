# Wax Deposition Predictor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wax-deposition-predictor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Predicts wax buildup in oil pipelines and wells to optimize maintenance.

## Description
This MCP server provides critical modeling tools for managing paraffin wax deposition in oil transport systems. It allows AI agents to calculate the Wax Appearance Temperature (WAT) using `calculate_wat`, estimate accumulation speeds with `predict_deposition_rate`, and determine maintenance schedules via `estimate_pigging_interval`. Additionally, it can evaluate fluid dynamics using `analyze_shear_effects` to understand how flow impacts wax layers. These tools help prevent flow restrictions and optimize pigging frequency in both subsea and onshore pipelines.


## Available Tools (4)
- **calculate_wat**: Determines the temperature threshold where wax starts to precipitate
- **analyze_shear_effects**: Evaluates how much the fluid flow (shear) is stripping away or redistributing the wax layer
- **estimate_pigging_interval**: Recommends how often the pipeline should be cleaned to prevent operational failure
- **predict_deposition_rate**: Estimates how fast wax is accumulating at specific points in the system


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wax Deposition Predictor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the wax appearance temperature for a crude oil with a paraffin content of 15%?"

**🤖 AI Agent:**
> The Wax Appearance Temperature for this crude oil composition is 32.5°C.

---

**👤 You:**
> "Calculate the deposition rate for a pipe with a 10% WAT, a temperature profile of [25, 20, 15], a flow rate of 500, and a diameter of 0.5."

**🤖 AI Agent:**
> The predicted deposition rates are: position 0: 0.02 mm/day, position 1: 0.05 mm/day, position 2: 0.08 mm/day.

---

**👤 You:**
> "How often should I run a pig if the deposition rate is 0.05 mm/day and the critical thickness is 2.0 mm?"

**🤖 AI Agent:**
> The recommended pigging interval is 40 days.


## ❓ FAQ

**Q: How do I determine when to clean my pipeline?**
You can use the `estimate_pigging_interval` tool. By providing the calculated deposition rates and the critical thickness threshold, the tool recommends a maintenance interval to prevent operational failure.

**Q: What is the Wax Appearance Temperature (WAT)?**
The WAT is the temperature threshold where wax crystals begin to precipitate from the crude oil. You can find this value using the `calculate_wat` tool by providing the crude oil composition.

**Q: Can this tool account for fluid flow effects?**
Yes, the `analyze_shear_effects` tool evaluates how fluid flow (shear) strips away or redistributes the wax layer based on flow rate, pipe diameter, and viscosity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wax-deposition-predictor](https://vinkius.com/en/ai-agent-connect/wax-deposition-predictor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wax Deposition Predictor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wax-deposition-predictor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wax Deposition Predictor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wax-deposition-predictor": {
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
