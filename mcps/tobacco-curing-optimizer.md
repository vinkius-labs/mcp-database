# Tobacco Curing Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/tobacco-curing-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Generates optimal temperature and humidity schedules for tobacco curing.

## Description
This MCP server provides specialized tools for tobacco producers to manage the biological curing process. By using `generate_curing_schedule`, users can create precise stage-by-stage plans covering yellowing, leaf drying, and stem drying. The server also includes `predict_quality_outcome` to estimate market grades and `calculate_energy_requirements` to forecast barn energy consumption. It accounts for tobacco variety, leaf position, and maturity to ensure optimal leaf quality.


## Available Tools (4)
- **calculate_energy_requirements**: Estimates the total energy cost to run the barn for a specific schedule
- **predict_quality_outcome**: Estimates the final market grade of the cured tobacco
- **generate_curing_schedule**: Generates an optimal stage-by-stage tobacco curing schedule
- **get_stage_constraints**: Retrieves the physiological safety bounds for a specific tobacco type


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tobacco Curing Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a curing schedule for flue-cured tobacco, primings position, maturity level 0.8, and a barn capacity of 500."

**🤖 AI Agent:**
> The generated schedule for your flue-cured primings includes a 48-hour yellowing stage at 35°C, a 72-hour leaf drying stage at 45°C, and a 36-hour stem drying stage at 55°C. Total energy is estimated at 1250 kWh.

---

**👤 You:**
> "What is the predicted quality for a burley tobacco with these parameters: type 'burley', maturity 0.9, and a drying temperature of 42°C?"

**🤖 AI Agent:**
> The predicted quality grade is Premium, with a color score of 8.5, texture score of 8.2, and aroma score of 8.8.

---

**👤 You:**
> "What are the safety temperature limits for dark tobacco?"

**🤖 AI Agent:**
> For dark tobacco, the maximum yellowing temperature is 38°C and the maximum drying temperature is 50°C. The ideal humidity range is 85-95%.


## ❓ FAQ

**Q: How do I create a curing plan?**
Use the `generate_curing_schedule` tool with your tobacco type, leaf position, and maturity level to receive a complete temperature and humidity profile.

**Q: Can I estimate my energy costs?**
Yes, the `calculate_energy_requirements` tool estimates total kWh and peak load based on your specific schedule and barn capacity.

**Q: How is leaf quality predicted?**
The `predict_quality_outcome` tool analyzes your curing parameters against the biological needs of the tobacco variety to estimate color, texture, and aroma scores.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/tobacco-curing-optimizer](https://vinkius.com/ai-agent-connect/tobacco-curing-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tobacco Curing Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tobacco-curing-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tobacco Curing Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tobacco-curing-optimizer": {
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
