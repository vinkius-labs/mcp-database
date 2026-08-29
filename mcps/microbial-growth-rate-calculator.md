# Microbial Growth Rate Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/microbial-growth-rate-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Calculate specific growth rate, doubling time, and growth yield for microbial populations.

## Description
This MCP server provides essential kinetic modeling tools for microbiologists. It allows AI agents to determine fundamental growth parameters from time-series measurements of cell density or optical density. Use `calculate_growth_kinetics` to find the specific growth rate and doubling time, `calculate_growth_yield` to measure biomass efficiency, `analyze_growth_phase` to identify growth stages, and `validate_measurement_consistency` to ensure data quality for kinetic modeling.


## Available Tools (4)
- **analyze_growth_phase**: Identify which growth phase a specific measurement point belongs to
- **calculate_growth_kinetics**: Determine fundamental growth parameters (specific growth rate and doubling time) from two measurement points
- **calculate_growth_yield**: Determine how efficiently microbes converted substrate into biomass
- **validate_measurement_consistency**: Ensure measurements are suitable for kinetic modeling by checking biological plausibility


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Microbial Growth Rate Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the growth kinetics if the initial OD was 0.1 and the final OD was 0.8 after 4 hours."

**🤖 AI Agent:**
> The specific growth rate is 0.470 and the doubling time is 1.47 hours.

---

**👤 You:**
> "What is the growth yield if the biomass increased by 5.0 units and 10.0 units of substrate were consumed?"

**🤖 AI Agent:**
> The yield coefficient is 0.5.

---

**👤 You:**
> "Identify the growth phase for this data: [{'time': 0, 'value': 0.1}, {'time': 1, 'value': 0.11}, {'time': 2, 'value': 0.12}] with a threshold of 0.5."

**🤖 AI Agent:**
> The current phase is Lag and it is not exponential.


## ❓ FAQ

**Q: How do I calculate the doubling time?**
You can use the `calculate_growth_kinetics` tool by providing the initial and final cell counts or optical density values along with the time interval between them.

**Q: Can I use Optical Density (OD) instead of cell counts?**
Yes, the tools are designed to work with both direct cell counts and Optical Density (OD) measurements.

**Q: How can I check if my growth data is reliable?**
Use the `validate_measurement_consistency` tool to check if your measurements are biologically plausible and suitable for kinetic modeling.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/microbial-growth-rate-calculator](https://vinkius.com/ai-agent-connect/microbial-growth-rate-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Microbial Growth Rate Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `microbial-growth-rate-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Microbial Growth Rate Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "microbial-growth-rate-calculator": {
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
