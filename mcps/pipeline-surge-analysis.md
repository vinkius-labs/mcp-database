# Pipeline Surge Analysis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pipeline-surge-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Analyze water hammer effects and transient pressure surges in fluid pipelines.

## Description
This MCP server provides specialized engineering tools for modeling water hammer effects and transient pressure surges in fluid transport pipelines. It allows AI agents to calculate critical parameters such as wave speed using `calculate_wave_speed`, determine maximum pressure rise with `calculate_joukowsky_surge`, identify if a valve closure is sudden or gradual via `analyze_closure_regime`, and assess the risk of column separation using `evaluate_separation_risk`.


## Available Tools (4)
- **analyze_closure_regime**: Determines if a valve closure is "sudden" or "gradual" based on the timing of the pressure wave travel
- **calculate_joukowsky_surge**: Calculates the maximum theoretical pressure rise resulting from an instantaneous velocity change
- **calculate_wave_speed**: Determines how fast a pressure disturbance will propagate through the specific pipe-fluid system
- **evaluate_separation_risk**: Assesses the likelihood of vapor pocket formation (column separation) during a pressure drop


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pipeline Surge Analysis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the wave speed for a pipe with fluid density of 1000 kg/m3, bulk modulus of 2.2e9 Pa, Young's modulus of 200e9 Pa, diameter of 0.5m, and wall thickness of 0.01m."

**🤖 AI Agent:**
> The calculated wave speed is 1443.37 m/s.

---

**👤 You:**
> "What is the Joukowsky surge pressure if the wave speed is 1200 m/s, fluid density is 1000 kg/m3, and the velocity change is 2 m/s?"

**🤖 AI Agent:**
> The maximum pressure rise is 2,400,000 Pa.

---

**👤 You:**
> "Is a valve closure of 2 seconds sudden for a 1000m pipe with a wave speed of 1200 m/s?"

**🤖 AI Agent:**
> Yes, the closure is sudden because the critical time is 0.83 seconds.


## ❓ FAQ

**Q: What is water hammer?**
Water hammer is a pressure surge or wave caused when a fluid in motion is forced to stop or change direction suddenly, such as during rapid valve closure.

**Q: How can I calculate the maximum pressure rise?**
You can use the `calculate_joukowsky_surge` tool to find the maximum theoretical pressure rise based on wave speed, fluid density, and velocity change.

**Q: Can this tool help prevent pipeline damage?**
Yes, by using tools like `evaluate_separation_risk` and `analyze_closure_regime`, engineers can identify dangerous transients and design safer valve operations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pipeline-surge-analysis](https://vinkius.com/en/ai-agent-connect/pipeline-surge-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pipeline Surge Analysis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pipeline-surge-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pipeline Surge Analysis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pipeline-surge-analysis": {
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
