# Subsea Completion Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/subsea-completion-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design subsea completion systems including tree architecture, tubing hangers, and control infrastructure.

## Description
This MCP server provides specialized engineering tools for designing subsea completion systems. It allows AI agents to determine the optimal tree architecture using `get_tree_configuration`, select appropriate tubing hanger systems via `evaluate_tubing_hanger`, define necessary control infrastructure with `determine_control_system`, and assess operational logistics through `analyze_intervention_feasibility`. The tools account for critical variables such as water depth, reservoir pressure, temperature, and fluid composition to ensure system integrity and intervention feasibility.


## Available Tools (4)
- **analyze_intervention_feasibility**: Assesses the difficulty and logistical requirements of performing workovers on the proposed design
- **determine_control_system**: Defines the necessary control infrastructure to manage the subsea wellhead
- **evaluate_tubing_hanger**: Recommends the appropriate tubing hanger system based on wellbore stresses and environment
- **get_tree_configuration**: Determines the most suitable subsea tree architecture for a specific well


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Subsea Completion Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What kind of subsea tree should I use for a well at 1500m depth with high intervention frequency and 300 bar pressure?"

**🤖 AI Agent:**
> For a depth of 1500m and high intervention frequency, a horizontal tree is recommended to facilitate easier workovers.

---

**👤 You:**
> "Recommend a tubing hanger for a reservoir with 120C temperature, 400 bar pressure, and sour fluid composition."

**🤖 AI Agent:**
> A heavy-duty hanger with corrosion-resistant seal materials is required due to the high pressure, temperature, and sour fluid conditions.

---

**👤 You:**
> "What control system is needed for a 2500m deep well requiring 5 valve actuations?"

**🤖 AI Agent:**
> For a depth of 2500m, an electro-hydraulic or all-electric control system is required to manage signal latency and response times.


## ❓ FAQ

**Q: How does the tool decide between vertical and horizontal trees?**
The `get_tree_configuration` tool evaluates water depth and expected intervention frequency. For high-intervention wells, it prioritizes horizontal trees to allow easier access to the tubing hanger.

**Q: Can I design control systems for deepwater wells?**
Yes, `determine_control_system` evaluates water depth to recommend whether a hydraulic, electro-hydraulic, or all-electric system is required to manage signal latency.

**Q: How are seal materials selected for the tubing hanger?**
The `evaluate_tubing_hanger` tool analyzes reservoir temperature, pressure, and fluid composition (such as sour or acidic fluids) to recommend the correct seal materials and hanger types.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/subsea-completion-design](https://vinkius.com/en/ai-agent-connect/subsea-completion-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Subsea Completion Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `subsea-completion-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Subsea Completion Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "subsea-completion-design": {
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
