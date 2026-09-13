# Pulse Test Interpretation MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pulse-test-interpretation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Analyzes pressure pulse sequences to characterize reservoir permeability, porosity, and geometry.

## Description
This MCP server provides specialized tools for reservoir engineering by interpreting transient pressure pulse tests. It allows AI agents to calculate the permeability-thickness product using `analyze_transmissibility`, determine storage capacity with `analyze_storativity`, identify flow regimes via `calculate_geometry_type`, and quantify propagation delays with `estimate_time_lag_effects`. It transforms raw pressure amplitude and time interval data into actionable reservoir characterization metrics.


## Available Tools (4)
- **calculate_geometry_type**: Identifies the reservoir flow regime based on the pressure response behavior
- **analyze_storativity**: Calculates the porosity-compressibility product to determine the reservoir's storage capacity
- **estimate_time_lag_effects**: Quantifies the delay in pressure propagation to validate the depth or distance of the test observations
- **analyze_transmissibility**: Calculates the permeability-thickness product based on the relationship between pulse amplitude and response attenuation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pulse Test Interpretation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the transmissibility for these pulse data: amplitudes [10, 8, 6], responses [5, 3, 1], and intervals [1, 1, 1]."

**🤖 AI Agent:**
> The calculated permeability-thickness product (kh) is 2.5.

---

**👤 You:**
> "What is the reservoir geometry for a response showing a specific log-log slope?"

**🤖 AI Agent:**
> The identified flow regime is radial with a confidence score of 0.92.

---

**👤 You:**
> "Determine the storage capacity using a khProduct of 15.0 and these pulse sequences."

**🤖 AI Agent:**
> The calculated porosity-compressibility product (phi-c) is 0.045.


## ❓ FAQ

**Q: What can I calculate with these tools?**
You can calculate the permeability-thickness product, the porosity-compressibility product, identify reservoir flow geometry, and estimate time lag effects.

**Q: How do I determine the reservoir flow regime?**
Use the `calculate_geometry_type` tool, which analyzes the slope of the pressure response on a log-log scale to identify radial, linear, or bounded flow.

**Q: What data is required for analysis?**
The tools require sequences of pulse amplitudes, response amplitudes, and the time intervals between consecutive pulses.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pulse-test-interpretation](https://vinkius.com/en/ai-agent-connect/pulse-test-interpretation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pulse Test Interpretation** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pulse-test-interpretation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pulse Test Interpretation** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pulse-test-interpretation": {
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
