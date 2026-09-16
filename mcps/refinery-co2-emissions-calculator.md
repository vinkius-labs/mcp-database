# Refinery CO2 Emissions Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/refinery-co2-emissions-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industrial](../categories/industrial.md)

Quantify Scope 1 and Scope 2 emissions, emission intensity, and carbon balance for refinery operations.

## Description
This MCP server provides a specialized calculation engine for quantifying carbon dioxide emissions within refinery operations. It allows AI agents to accurately calculate Scope 1 emissions using `get_scope_1_emissions`, determine indirect emissions via `get_scope_2_emissions`, evaluate efficiency with `get_emission_intensity`, and assess net carbon positions through `calculate_carbon_balance`. It is designed to help industrial operators align with GHG Protocol standards by differentiating between combustion and process emissions.


## Available Tools (4)
- **calculate_carbon_balance**: Determine the net carbon position of the refinery
- **get_emission_intensity**: Determine the efficiency of carbon output relative to production volume
- **get_scope_1_emissions**: Calculate the total direct emissions produced by combustion and chemical processes
- **get_scope_2_emissions**: Calculate the indirect emissions resulting from purchased energy


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Refinery CO2 Emissions Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the Scope 1 emissions for 500 metric tonnes of natural gas with 50 metric tonnes of process emissions."

**🤖 AI Agent:**
> The total Scope 1 emissions are 545.0 metric tonnes.

---

**👤 You:**
> "What are the Scope 2 emissions for consuming 1000 MWh on a renewable grid?"

**🤖 AI Agent:**
> The total Scope 2 emissions are 50.0 metric tonnes.

---

**👤 You:**
> "Determine the carbon balance if total emissions are 1000 tonnes and 1200 tonnes are captured."

**🤖 AI Agent:**
> The net carbon position is -200.0 metric tonnes, meaning the facility is carbon neutral.


## ❓ FAQ

**Q: How are Scope 1 emissions calculated?**
Scope 1 emissions are calculated by summing combustion emissions (fuel consumption multiplied by the specific fuel emission factor) and direct process emissions.

**Q: Can I calculate my refinery's carbon neutrality status?**
Yes, by using the `calculate_carbon_balance` tool, you can determine if your net carbon position is zero or less, indicating carbon neutrality.

**Q: What is emission intensity?**
Emission intensity is the ratio of total emissions to the production volume, which helps compare efficiency across different facilities.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/refinery-co2-emissions-calculator](https://vinkius.com/en/ai-agent-connect/refinery-co2-emissions-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Refinery CO2 Emissions Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `refinery-co2-emissions-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Refinery CO2 Emissions Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "refinery-co2-emissions-calculator": {
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
