# Tracer Survey Interpretation MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/tracer-survey-interpretation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analysis](../categories/data-analysis.md)

Analyze interwell tracer surveys to characterize reservoir connectivity and flow behavior.

## Description
This MCP server provides advanced diagnostic capabilities for reservoir engineering by interpreting interwell tracer surveys. It connects AI agents to specialized transport models to calculate critical reservoir parameters. Using `analyze_tracer_breakthrough`, agents can determine flow velocity and heterogeneity indices from concentration-time data. The `calculate_swept_volume` tool estimates the volume of the reservoir contacted by the tracer, while `evaluate_connectivity` quantifies hydraulic communication between wells. Additionally, `identify_heterogeneity_zones` detects high-permeability thief zones and dispersion characteristics, helping to map reservoir architecture and bypass risks.


## Available Tools (4)
- **analyze_tracer_breakthrough**: Calculates fundamental flow characteristics from concentration-time data
- **calculate_swept_volume**: Estimates the volume of the reservoir contacted by the tracer
- **evaluate_connectivity**: Quantifies the hydraulic communication between the injection and offset wells
- **identify_heterogeneity_zones**: Detects presence of high-permeability channels or thief zones


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tracer Survey Interpretation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the flow velocity and heterogeneity for this tracer profile."

**🤖 AI Agent:**
> The calculated flow velocity is 0.45 m/day with a heterogeneity index of 1.2, indicating relatively uniform flow.

---

**👤 You:**
> "What is the swept volume for a reservoir with 1,000,000 m3 pore volume?"

**🤖 AI Agent:**
> The swept volume is 650,000 m3, resulting in a sweep efficiency of 65%.

---

**👤 You:**
> "Evaluate the connectivity between the injection and offset well."

**🤖 AI Agent:**
> The connectivity score is 0.85, indicating strong hydraulic communication via a channelized flow path.


## ❓ FAQ

**Q: What can I calculate with this MCP?**
You can calculate flow velocity, swept volume, connectivity scores, and identify reservoir heterogeneity zones using tracer concentration profiles.

**Q: How do I identify thief zones?**
Use the `identify_heterogeneity_zones` tool to detect high-permeability channels based on tracer breakthrough speed and dispersion.

**Q: Does it support radioactive tracers?**
Yes, the tools are designed to handle both chemical and radioactive tracer data for comprehensive reservoir characterization.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/tracer-survey-interpretation](https://vinkius.com/en/ai-agent-connect/tracer-survey-interpretation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tracer Survey Interpretation** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tracer-survey-interpretation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tracer Survey Interpretation** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tracer-survey-interpretation": {
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
