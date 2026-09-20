# Bedroom Environment Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/bedroom-environment-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Assess and optimize your bedroom environment for better sleep quality.

## Description
This MCP server provides specialized tools to evaluate your sleeping environment across thermal, acoustic, and sensory dimensions. Use `get_environment_score` for a complete assessment of your room, or specific tools like `get_thermal_profile`, `get_acoustic_assessment`, and `get_sensory_readiness` to pinpoint issues with temperature, noise, light, or air quality. It helps you identify the exact adjustments needed to reach your ideal sleep state.


## Available Tools (4)
- **get_thermal_profile**: Evaluates the sleep-readiness of the current temperature setting
- **get_acoustic_assessment**: Analyzes how noise levels impact sleep continuity
- **get_environment_score**: Provides a comprehensive assessment of the current bedroom environment
- **get_sensory_readiness**: Combines light and air quality to assess sensory-driven sleep triggers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bedroom Environment Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How is my bedroom environment for sleep? Temperature is 22C, noise is 30dB, light is 5lux, AQI is 40, and comfort is mattress 0.9 and bedding 0.8."

**🤖 AI Agent:**
> Your bedroom environment is excellent with an overall score of 92. Your temperature and light levels are within the ideal ranges for deep sleep.

---

**👤 You:**
> "Is my room too noisy for sleep? The noise level is 55dB."

**🤖 AI Agent:**
> The noise level of 55dB poses a medium risk of sleep disruption. It is recommended to use white noise to mask sudden sounds.

---

**👤 You:**
> "Check my thermal profile. The temperature is 28C."

**🤖 AI Agent:**
> Your thermal score is 45. The temperature is too high for optimal sleep. Cool the room down to reach the ideal range.


## ❓ FAQ

**Q: How accurate are the sleep scores?**
The scores are based on physiological sleep research regarding thermal neutrality, acoustic stability, and luminous environments.

**Q: Can I check just the temperature impact?**
Yes, you can use the `get_thermal_profile` tool to specifically evaluate how your current temperature affects sleep readiness.

**Q: What inputs do I need for a full report?**
For a complete report, use `get_environment_score` with temperature, noise level, light level, air quality index, and comfort factors.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/bedroom-environment-scorer](https://vinkius.com/en/ai-agent-connect/bedroom-environment-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bedroom Environment Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bedroom-environment-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bedroom Environment Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bedroom-environment-scorer": {
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
