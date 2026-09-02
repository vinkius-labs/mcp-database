# Concrete Corrosion Predictor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/concrete-corrosion-predictor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [infrastructure](../categories/infrastructure.md)

Estimates reinforcement corrosion rates, spalling time, and remaining service life.

## Description
This MCP server provides specialized tools for structural health monitoring. It allows AI agents to calculate the instantaneous corrosion rate using `calculate_corrosion_rate`, predict when physical damage will occur with `predict_spalling_time`, and estimate the total remaining service life using `estimate_remaining_service_life`. It also evaluates the effectiveness of protective measures via `evaluate_protection_efficiency` based on concrete resistivity, chloride content, and material quality.


## Available Tools (4)
- **predict_spalling_time**: Estimates the time elapsed from the start of corrosion until physical damage (spalling) occurs
- **calculate_corrosion_rate**: Determines the instantaneous corrosion rate of the reinforcement based on environmental and material conditions
- **estimate_remaining_service_life**: Calculates the remaining useful life of the structure before it reaches a critical structural limit
- **evaluate_protection_efficiency**: Assesses how effectively current coatings and concrete quality are mitigating corrosion risk


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Concrete Corrosion Predictor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the estimated corrosion rate for concrete with 5.0 Ωm resistivity, 2% chloride content, 25°C temperature, 60% humidity, and Standard quality?"

**🤖 AI Agent:**
> The estimated corrosion rate is 0.045 mm/year, which is classified as a moderate rate.

---

**👤 You:**
> "How many years until spalling occurs if the corrosion rate is 0.05 mm/year and the cover depth is 40 mm with Porous concrete?"

**🤖 AI Agent:**
> The predicted time until spalling occurs is 12.5 years, representing an elevated risk level.

---

**👤 You:**
> "Calculate the remaining service life for a 10-year-old structure with a 0.03 mm/year corrosion rate, 20mm initial steel section, and a 15% critical loss threshold."

**🤖 AI Agent:**
> The remaining service life is 33.3 years, with a total expected life of 43.3 years. The current structural integrity is rated as fair.


## ❓ FAQ

**Q: How does the tool calculate the corrosion rate?**
The `calculate_corrosion_rate` tool uses concrete resistivity, chloride content, temperature, humidity, and concrete quality to determine the electrochemical degradation speed.

**Q: Can I predict when concrete will start to chip or spall?**
Yes, by using `predict_spalling_time`, you can estimate the years remaining until rust expansion causes physical spalling based on the corrosion rate and cover depth.

**Q: What factors influence the remaining service life?**
The `estimate_remaining_service_life` tool considers the current corrosion rate, the original steel section size, the critical loss threshold, and the current age of the structure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/concrete-corrosion-predictor](https://vinkius.com/ai-agent-connect/concrete-corrosion-predictor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Concrete Corrosion Predictor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `concrete-corrosion-predictor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Concrete Corrosion Predictor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "concrete-corrosion-predictor": {
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
